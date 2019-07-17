# Watson-Assistant-Testing-Tools
collection of Jupyter Notebook in Python that can be used to test your Watson Assistant workspace

## Performance Testing (single-workspace)
This notebook can be used for Regression testing and Blind testing. 

1. **Regression Test Scope**: This can be used to test a set of testing phrases that are not part of the training set in Watson Assistant (WA). The idea is that you would re-run this test over time after the improvement phase, to check the health status of your workspace, and make sure that the workspace is still behaving in a consistent manner. 
2. **Blind Test Scope**: Simply analyse a set of testing phrases that are not part of the training set in Watson Assistant. This can be a one-off task requested by stakeholders. 

## Performance Testing (multiple-workspaces "Spray")
This notebook can be used for Regression testing and Blind testing in projects where multiple-workspaces (multiple-skills) are used. Specifically, it evaluates the <a href="https://medium.com/ibm-watson/ibm-watson-conversation-multiple-workspace-orchestration-d51f003f5d11">SPRAY</a> method: each testing phrase is sent to each sub-workspace/skill, individually.

## K-Fold Cross Validation 
This notebook will allow the user to perform a K-fold cross validation test on your Watson Assistant workspace 


## Optimal Threshold Analysis 
This notebook can be used to search for the optimal value of the confidence level threshold to use in your Waston Assistant workspace.

## N-Gram Testing 
This notebook will be used for diagnosis of incorrect intent detection problem. We want to use unigrams, bigrams and trigrams to do so.

The idea is that each intent is sensitive to particular words/combination of words. The scope is to find a fast way to detect why, for instance, a testing phrase didn't trigger the right intent.This notebook will help the user understanding why which words and in which positions are the most important in the intent detection phase. 

---------------------
# How to run the Notebooks 
## Locally 
The notebooks are using Python 3.6. It is recommended to install Anaconda for Python 3.x since it is compatible with most of the packages. Please download and install Anaconda from: 

https://www.anaconda.com/download


## Using Watson Studio 
If you have an instance of <a href ="https://dataplatform.cloud.ibm.com/">Watson Studio</a>, you can upload the notebooks directly into your project. 
Go to the "asset" tab of your project, and in the notebook section click on "add new notebook" and follow the instruction. 
When choosing the run time, choose a default Python runtime. 
<br>
Make sure to use the <a href="https://github.ibm.com/Erika-Agostinelli1/Watson-Assistant-Testing-Tools/tree/master/For%20Watson%20Studio">notebooks optimised for Watson Studio </a> in the folder "For Watson Studio", because they will explain step by step how to set up the access token, how to store and save your datasets using Watson Studio. 
