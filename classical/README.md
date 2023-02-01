![Header](https://github.com/Azure/mlops-v2/blob/main/documentation/repositoryfiles/mlopsheader.jpg)

# Azure MLOps (v2) Pattern: Azure Machine Learning - Classical Machine Learning

This repository includes all use case specific codebase to be deployed as the inner loop for the [MLOps v2](https://github.com/Azure/mlops-v2) solution accelerator.

The repo itself functions as a standalone entity that agnosticly holds all Azure Machine Learning - Classical Machine Learning requirements for this architectual pattern.


## 📐 Pattern Architectures: Key concepts

This repository follows the architecture linked below:

| Link                                                    | AI Pattern                                                              |
| ------------------------------------------------------- | ----------------------------------------------------------------------- |
| [Pattern AML CML](https://github.com/Azure/mlops-v2/blob/main/documentation/architecturepattern/AzureML_CML_Architecture.png) | Azure Machine Learning - Classical Machine Learning                     |


## 👤 Getting started

Please visit [MLOps v2](https://github.com/Azure/mlops-v2) for the initial deployment of this inner loop pattern.

## Upload data (required manual step between deployment of infrastructure and rest of MLops lifecycle)

- navigate to the `data` folder in this repo and locate the `nyc_taxi.parquet` file

- Navigate to Azure Portal and open the storage account created in the feature store resource group, it should start with `st...` not the one with `stlog...`

- Click on "Container" and then click on "+ Container", name the container `nyctaxi` and upload the data `nyc_taxi.parquet` file to this new container

In real world projects: you would have these existing data containers as an output from another data engineering process and then you would use Feathr to point to that data location (and do feature enfgineering from there)


## ‼️ Feedback or Issues

Please visit [MLOps v2](https://github.com/Azure/mlops-v2) and file an **issue** or go to Microsofts internal SharePoint site to hand in any feedback.


## Contributing

This project welcomes contributions and suggestions. To learn more visit the contributing section in the [MLOps v2](https://github.com/Azure/mlops-v2) solution accelerator.

Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
trademarks or logos is subject to and must follow
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
