## Annotation using haystack tool

1) Log on to Annotation tool site - https://annotate.deepset.ai/

![alt text](02-Annotation/images/anno1.jpg "annotation1")

**Annotation account Credential -**

**Mail - asma.trabelsi@al-enterprise.com**

**Password - December@2020**

2) In the next page, create a project by clicking on "Create Project"
![alt text](02-Annotation/images/anno2.jpg "annotation2")

3) Give a name to your project and select **Answer category** in **Annotation mode**.
![alt text](02-Annotation/images/anno3.jpg "annotation3")

4) The project is created and click on right arrow button as shown to go to **Project Page**.
![alt text](02-Annotation/images/anno4.jpg "annotation4")

5) In the next page , go to **Import** tab and click on **Documents** for import.
![alt text](02-Annotation/images/anno5.jpg "annotation5")

6) Select TXT Upload, click on the upload icon. Upload document/documents of your choice.
![alt text](02-Annotation/images/anno6.jpg "annotation6")

7) Go back to **Documents** tab, we see our document is uploaded and a **id** is generated. Click on the arrow button at extreme right, to view the document and create pairs of QAs of the document.
![alt text](02-Annotation/images/anno7.jpg "annotation7")

8) Click on **ADD CUSTOM QUESTION** button.
![alt text](02-Annotation/images/anno8.jpg "annotation8")

9) Now go to a desired passage and highlight your answer by operating Left-key of mouse. For eg. we start from 'In' and end at 'on'.
![alt text](Annotation/images/anno9.jpg "annotation9")

10) A new window pops up, write your question in box and change **Answer Category** depending on length of Answer, for example , here we have 'LONG answer'
![alt text](02-Annotation/images/anno10.jpg "annotation10")

11) Hit 'Submit' button to make the QA pair.
![alt text](02-Annotation/images/anno11.jpg "annotation11")

12) We see a question and its corresponding answer being 'Highlighted'.
![alt text](02-Annotation/images/anno12.jpg "annotation12")

13) If you want to edit your question, click the button on right side of the question and edit the question.
![alt text](02-Annotation/images/anno13.jpg "annotation13")

14) If you want to delete this QA pair, click on the right button of the question. At first click on **Remove my answer**.
![alt text](02-Annotation/images/anno14.jpg "annotation14")

15) Next, click on **Delete**.
![alt text](02-Annotation/images/anno15.jpg "annotation15")

16) For exporting your QA pairs of your project go to **Export labels**. You will see the list of Question-Answer. Click on **Export Answers**.
    - 'Export table in excel' is used to keep a directory of your questions.
    - 'Export in SQuAD format' is used for **Fine-tuning** and **Evaluation** purpose. 

To know how to design Question for Troubleshooting Guides, refer to Question-Answering Guide. 
    - https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Annotation/Question-Answering%20Guideline