# Automatic Agent for Troubleshooting OmniPCX Enterprise

This repository contains all the files which are part of development of Automatic Agent for Troubleshooting OmniPCX Enterprise.

Following are the **repositories**.

## 1) Initial Setup and Test.
### 1. **Initial Setup**
This repository gives information about setting up Haystack Framework in your PC and testing the scripts in your PC or any cloud platform like Google Colab

- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/01-Initial%20Setup



## 2) Data Files

This is a repository for all **Data** required to Implement Automatic Agent for Troubleshooting OmniPCX Enterprise.

- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data

### 1. **Config_files**	

- This repository is about the configuration file used in FastAPI Backend, the excel file links a document name(in Txt or PDF) to URL link in shared OneDrive Folder.

- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Config_files

- In case, URL link expires, create a OneDrive Folder for 195 ( 45 Troubleshooting Guides in PDF + 150 PDFs of former 45 docs but **split**), share all the files publicly and update the links in column **section_link_actual** for sections	and **doc_link** for whole Troubleshooting Guides. (There are 150 rows in excel file.)

### 2. **Input Troubleshooting Guides in PDF**
- This repository is about **PDF version** of **Troubleshooting Guides for OmniPCX Enterprise**.

- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Input%20Troubleshooting%20Guides%20in%20PDF

- **First** sub-repository - **TS_Guide_45_Docs_original** : This contains **45 unique PDF** files for **Troubleshooting Guides for OXE**.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Input%20Troubleshooting%20Guides%20in%20PDF/TS_Guide_45_Docs_original

- **Second** sub-repository - **TS_Guide_150_Docs_split** : This contains **150 split PDF** files for Troubleshooting Guides of former sub-repository. Splitting is done on the basis of **section** of a **Troubleshooting Guide**.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Input%20Troubleshooting%20Guides%20in%20PDF/TS_Guide_150_Docs_split




### 3. **Input Troubleshooting Guides in txt format**
- This repository is about **cleaned .txt version** of **Troubleshooting Guides for OmniPCX Enterprise**.

- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Input%20Troubleshooting%20Guides%20in%20txt%20format

- **First** sub-repository - **Troubleshooting_Guides_45_cleaned** : This contains  **cleaned 45 unique .txt format** **Troubleshooting Guides for OXE** . The files in this sub-repository corresponds to **45 PDF** listed in previous repository.
- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Input%20Troubleshooting%20Guides%20in%20txt%20format/Troubleshooting_Guides_45_cleaned

- **Second** sub-repository - **TS_Guide_150_Docs_split** : This contains **150 split in .txt format** Troubleshooting Guides of former sub-repository. Splitting is done on the basis of **section** of a **Troubleshooting Guide**. The files in this sub-repository corresponds to **150 PDF (split)** listed in previous repository.
- Link : https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Input%20Troubleshooting%20Guides%20in%20txt%20format/TroubleShooting_Guides_section_cleaned_and_splited

- **Note**: For any experimentation or implemnetation of Chatbot over ElasticSearch using Haystack use the **150 split files in .txt files.** 

### 4. **Haystack_input_files**	
- This repository is about **annotated files** for **Fine-Tuning and Evaluation**.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Haystack_input_files

- **First** sub-repository - Training (Fine-Tuning):  This contains file for Fine-tuning process.


- **Second** sub-repository -  Evaluation : This contain files for evaluation of a Fine-Tuned Model.
- file eval_raw.json is download from Haystack Tool.
- file eval_with_title.json, eval_with_title_long.json and eval_with_title_short.json are generated using Python (explained in repository 'Evaluation')


### 5. **Final Fine-Tuned Model** 
- This repository gives link for Fine-Tuned Model (roBERTa_base_sqaud2) used in Final ChatBot API.

Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Final%20Fine-Tuned%20Model

### 6. **Presentation for Automatic Agent for TS OXE**
- This repository has Powerpoint Presentation of Automatic Agent for OXE Troubleshooting.
Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Data/Presentation%20for%20Automatic%20Agent%20for%20TS%20OXE

## 3) Development Repositories

### 1. **Annotation**

- This repository gives information how to proceed with Annotation and Guidelines for Question framing.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/02-Annotation

### 2. **Finetuning**
- This repository is about fine-tuning a pre-trained model using a annotated json file.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/03-Finetuning
- It is recommended to implement **Fine-Tuning** in **Google Colab** or **Amazon Web Service**.


### 3. **Evaluation**
- This repository gives information about Evaluation of a Fine-Tuned Model.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/04-Evaluation
- It is recommended to implement **evaluation** in **Google Colab**.

### 4. **FastAPI_Integration**
- This repository gives link for Fine-Tuned Model (roBERTa_base_sqaud2) used in Final ChatBot API.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/05-FastAPI_Integration


### 5. **Rainbow_sdk_NodeJS**
- This repository has source code and guide to integrate Rainbow Node JS with Haystack QA API and implement using Development Rainbow Platform.
- Link: https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/06-Rainbow_sdk_NodeJS



