# Pneumonia-Detection-Kubeflow
Built using Kubeflow, this ML pipeline effectively detects pneumonia in medical images from Kaggle's dataset. By automating data preprocessing, model training, and evaluation, the pipeline showcases the synergy between advanced technology and healthcare.

**Architecture Diagram:**<br><br>
![architecture diagram](images/architecture_diagram.svg) <br>

***Note: Following the given steps may incur you charges!! I have used the google cloud's free trial resources for all the provisions. If possible I encourage you to do the same!***

**Used Components:**
+ kubeflow 1.7 - Jupyter Notebook
- Google cloud storage bucket
* kubernetes 1.27
+ Google compute engine 

**Steps Involved:**
1. Create a VM instance of minimum 32gb ram and 6 core
1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/lasaljaywardena/pneumonia-chest-x-ray-dataset) and upload it to gcs bucket
1. Create a service account with storageobjectviewer permission and download the keys.json (I recommand you to follow some tutorial)
1. SSH to the VM instance and follow this [doc](https://charmed-kubeflow.io/docs/get-started-with-charmed-kubeflow) for kubeflow set up
1. Once Kubeflow is installed, go to the dashboard and Create your Jupyter Notebook (choose custom image as tensorflow-full)
1. Finally Create a ML pipeline with Kubeflow pipeline

# 1. Local Machine Setup:
You can either create your own custom keys with Puttygen or use Google Cloud CLI on your local machine to create a ssh access to the VM you just created. If you are unsure of what i mean, Please refer internet on how to setup remote access on your VM.
> I prefer using a linux os such as Ubuntu for this step

> If you are using a window's pc you can install Oracle VM virtual box and install ubuntu 20.04 or later
***(The doc that I shared earlier requires you to have proxy access to kubeflow dashboard. So this step is mandatory!!)***

# 2.
