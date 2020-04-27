# Create an application to predict your insurance premium cost with Auto AI 

### Summary


### Description

### Example Flow Diagram - TODO (Need to change)
<br>
<p align="center">
  <img src="docs/app-architecture.png">
</p>
<br>

### TODO - Flow Description
1. The user creates an Auto AI Project within IBM Watson Studio


## Included components
*	[IBM Watson Studio](https://console.bluemix.net/docs/services/blockchain/howto/ibp-v2-deploy-iks.html#ibp-v2-deploy-iks) 
*	[IBM Watson Machine Learning](https://console.bluemix.net/docs/services/blockchain/howto/ibp-v2-deploy-iks.html#ibp-v2-deploy-iks)
*	[IBM Cloud Object Storage](https://console.bluemix.net/docs/services/blockchain/howto/ibp-v2-deploy-iks.html#ibp-v2-deploy-iks) store smt

## Featured technologies
+ [artificial-intelligence](https://developer.ibm.com/technologies/artificial-intelligence/) Build and train models, and create apps, with a trusted AI-infused platform.
+ [Python](https://www.python.org/) Python is an interpreted, high-level, general-purpose programming language.

## Watch the Video - TODO

<!-- [![](docs/ibpVideo.png)](https://www.youtube.com/watch?v=ny8iif6ZXRU) -->

## Prerequisites

This Cloud pattern assumes you have an **IBM Cloud account**. Go to the 
link below to sign up for a free trial account - no credit card required. 
  - [IBM Cloud account](https://tinyurl.com/y4mzxow5)


# Steps TODO
1. [Clone the repo](#step-1-clone-the-repo)
2. [Explore the data](#step-2-explore-the-data)
3. [Create IBM Cloud services](#step-3-create-ibm-cloud-services)
4. [Create and Run Auto AI experiment](#step-4-create-and-run-auto-ai-experiment)
5. [Create a notebook from your model](#step-5-create-a-notebook-from-your-model)
6. [Run the application](#step-6-run-the-application)

## Step 1. Clone the repo

Clone this repo onto your computer in the destination of your choice:
```
git clone https://github.ibm.com/Horea-Porutiu/AoT-AutoAI.git
```
This will give you access to the data files in the `data` directory. These data sets 
are from Kaggle and `data.boston.gov`.

## Step 2. Explore the data

## Step 3. Create IBM Cloud services

First login to your IBM Cloud account. Use the video below for directions on how 
to create IBM Watson Studio Service.

![watsonStudio](https://media.github.ibm.com/user/79254/files/e493eb80-8626-11ea-87b5-f1c7cf8d50e0)
* After logging into IBM Cloud, click `Proceed` to show that you have read your data rights.

* Click on `IBM Cloud` in the top left corner to ensure you are on the home page.

* Within your IBM Cloud account, click on the top search bar to search for cloud services and offerings. Type in `Watson Studio` and then click on `Watson Studio` under `Catalog Results`.

* This will take you to the Watson Studio service page. There you can name the service as you wish. I named it mine
`Watson-Studio-freetrial`. You can also choose which data center to create your instance in. The gif above shows mine as 
being created in Dallas.

* For this guide, we will choose the `Lite` service, which is free. This has limited compute, but will be enough
to understand the main functionality of the service.

* Once you are satisfied with your service name, and location, and plan, click on create in the bottom-right corner. This will create your Watson Studio instance. 

![createProj](https://media.github.ibm.com/user/79254/files/db5a4d00-862d-11ea-96ce-0872b828932d)

* To launch your Watson Studio service, go back to the home page by clicking on `IBM Cloud` in the top-left corner. There you will see your services, and under there you should see your service name. This might take a minute or two 
to update. 

* Once you see your service that you just created, click on your service name, and this will take you to your 
Watson Studio instance page, which will say `Welcome to Watson Studio. Let's get started!`. Click on the `Get Started` button.

* This will take you to the Watson Studio tooling. There you will see a heading that says `Start by creating a project` and a button that says `Create Project`. Click on `Create a Project`. Next click on `Create an Empty project`.

* On the create a new project page, name your project. I named mine `insurance-demo`. We also need to associate a IBM Cloud Object store instance, so that we can store our data set.

* Under `Select Storage service` click on the `Add` button. This will take you to the IBM Cloud Object Store service page. Leave the service on the `Lite` tier and then click the `Create` button at the bottom of the page. You will be prompted to name the service, and choose the resource group. Once you are happy with the naming, and the resource group on `Confirm`. 

* Once you've confirmed your IBM Cloud Object Store instance, you will be taken back to the project page. Click on `refresh` and you should see your newly created Cloud Object Store instance under `Storage`. That's it! Now you can click `Create` at the bottom right of the page to create your first IBM Watson Studio project :) 
 
![addData](https://media.github.ibm.com/user/79254/files/09409100-8630-11ea-804e-ad92728b7f26)

* Once you've created your project, click on the `Add to project` at the top-right of your Watson Studio project page. This will pop up an image with different assets you can choose to add to your project. Click on `Auto AI experiment`.

* This will take your to a page which says `New AutoAI expriment` at the top-left. Name your experiment as you want. I named mine `auto-ai-insurance-demo`.

* Next, we need to add a Watson Machine Learning instance before we can create our Watson AutoAI experiment. On the right side of the screen click on
`Associate a Machine Learning instance`. 

* Same as before, select the `Lite` Tier, and click on the `Create` button at the bottom of the page. Name your instance as you wish. I named mine `machine-learning-free`. Choose the location and the resource group and then click on `Confirm` when you are happy with your instance details.

* Once you create your machine learning service, you will be taken back to the new AutoAI experiment page. Click on 
`Reload` on the right side of the screen. You should see your newly created machine learning instance. Great job! Click on `Create` on the bottom right part of your screen to create your first AutoAI experiment!

## Step 4. Create and Run Auto AI experiment

Next, create watson machine learning.

![machineLearn](https://media.github.ibm.com/user/79254/files/09409100-8630-11ea-804e-ad92728b7f26)

Next, run exp.

![machineLearn](https://media.github.ibm.com/user/79254/files/05ad0a00-8630-11ea-94e7-cd47ae3ac941)

Next, watch as it completes.

![compl](https://media.github.ibm.com/user/79254/files/004fbf80-8630-11ea-9c69-e97b12c39bbe)

## Step 5. Create a notebook from your model
## Step 6. Run the application




## Related Links TODO
<!-- * [Hyperledger Fabric Docs](http://hyperledger-fabric.readthedocs.io/en/latest/)
* [IBM Code Patterns for Blockchain](https://developer.ibm.com/patterns/category/blockchain/) -->

## License
This code pattern is licensed under the Apache Software License, Version 2. Separate third-party code objects invoked within this code pattern are licensed by their respective providers pursuant to their own separate licenses. Contributions are subject to the [Developer Certificate of Origin, Version 1.1 (DCO)](https://developercertificate.org/) and the [Apache Software License, Version 2](https://www.apache.org/licenses/LICENSE-2.0.txt).

[Apache Software License (ASL) FAQ](https://www.apache.org/foundation/license-faq.html#WhatDoesItMEAN)

