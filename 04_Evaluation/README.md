# This reposistory consist of preparing the evaluation file and executing the file to evaluate a Fine-Tuned Model.

## 1) Preparation of Evaluation file.

a) **Download** the evaluation file (.json) from your project from Haystack tool https://annotate.deepset.ai/

b) This file doesn't have **[title]** corresponding to its **[context]**, we need to add **[title]** **(document name)** to each **context**. 

Note: [title] field is necessary for Evaluation.

c) Get the **document name** for the **[document_id]** shown below and create a **python dictionary**.

![alt text](04-Evaluation/images/doc_id.png "Document ID for a document in Haystack")

d) Create a dictionary like below **'document_id':'document_name'**

![alt text](04-Evaluation/images/doc_id2.png "Dictionay for document_id and document name")

e) **Execute** the **'File_preparation_for_evaluation.ipynb'** , this will **generate** the original evaluation file (.json file) with **[title]**, also it will generate **separate** **(.json )** **file** for **'LONG'** and **'SHORT'** answer for evaluation.


## 2) Evaluation of Fine-Tuned Model.

It is recommended to evaluate a fine-tuned model in **Google Colab** 

Steps- 

a) Change the runtime to **GPU**.

![alt text](04-Evaluation/images/doc_id3.png "Change Runtime Type - 1")

![alt text](04-Evaluation/images/doc_id4.png "Change Runtime Type - 2")

b) Install the **required packages** for **Haystack Framework**

c) One can **reuse** the **same notebook** for evaluating **overall** all question and **questions with long and short answer separately**, just **uncomment** the **required one** and **comment out** the **'not' required ones**.

In the screenshot below, we are using overall evaluation file and hence we have commented the other two.

![alt text](04-Evaluation/images/doc_id6.png "Document Store for Overall and Separate LONG + SHORT")

d) **Mount** your Google Drive (One can **store** **Fine-Tuned Model** and **upload Evaluation File** in **Drive** to save time).

![alt text](04-Evaluation/images/doc_id5.png "Mount your Google Drive")

Note: **Upload** both the **Fine-Tuned Model** and **Evaluation Files** on **Drive** and **refresh** the files in **Colab** and **update** the location in the **code**.

e) **Update** the **location paths** for **Model** and **Evaluation File accordingly**.





f) **Evaluation logs** are generated on running each evaluation for **Reader + Retriever** along with **different combination** of parameters **top-k-reader** and **top-k-retriever**.

g) **Save** these logs in any editor of your choice for further analysis.


