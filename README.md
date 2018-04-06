### Authors: Yan Zhang and Ilia Karmanov

# Machine Learning Model Deployment via Azure CLI

It is often a non-trivial task to deploy machine learning (ML) models. In [this repo](https://github.com/ilkarman/DeepLearningFrameworks), we aim to create a Rosetta Stone of deep-learning frameworks by using common code for several different network structures. We mainly show the network training and evaluation process across many different frameworks. With this work, we further introduce a model deployment approach for a trained machine learning model. As an example, we show how to deploy the trained Keras (tensorflow) model, which is one of the deep learning models from above mentioned deep learning framework comparison work. We deploy the model on Azure Container Service (ACS) as a web service via Azure CLI [Machine Learning Model Management](https://docs.microsoft.com/en-us/azure/machine-learning/preview/model-management-cli-reference). Comparing with a previous [ACS deployment tutorial](https://github.com/Azure/ACS-Deployment-Tutorial), this approach simplifies the model deployment process by using a set of model management commands.  

Docker container is one effective approach to overcome the dependency problems for ML model deployment, but it is never a straightforward process. With this model management tool, it is convenient to initialize your Azure machine learning environment with a storage account, ACR registry, App Insights service, and other Azure resources by executing a single CLI command. You can also easily scale ACS Kubernetes cluster, as introduced in the blog post [Scaling Azure Container Service Clusters](https://blogs.technet.microsoft.com/machinelearning/2018/03/20/scaling-azure-container-service-cluster/).

Source code and full documentation are available at [Keras_TF_CNN_DeployModel.ipynb](Keras_TF_CNN_DeployModel.ipynb).


# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
