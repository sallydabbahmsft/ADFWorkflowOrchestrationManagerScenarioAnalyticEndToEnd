[**Back to the previous step**](/RunADFPipelines/1_Create_Airflow_environment_in_Workflow_Orchestration_Manager.md)

# Create ADF Pipeline

[What is the Copy Activity:]([https://learn.microsoft.com/en-us/azure/databricks/lakehouse/medallion](https://learn.microsoft.com/en-us/azure/data-factory/quickstart-hello-world-copy-data-tool))

in this step we want to create copy activity that will copy local file to my Azure Blob Storage account, if you wish to run different pipeline you might want to skip this step.


## Create Copy Activity

 Download the *dimension_customer.csv* file from the [Dataset Folder](/Dataset/).
   

1. From ADF studio, in **Author** tab, select **New Pipeline** , **Activities** drop down list will open, drag and drop copy activity:

     ![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/f6c1ed51-2c9a-43eb-8c10-91b36536bff6)
   
2 . In **Source** tab, select local file: 

   ![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/70a42526-4a9f-4d7c-b098-516c837b3422)

   
3. In **Destination** tab, add your blob storage as a dataset and save it as .csv file.

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/62489c78-f77e-459e-93d3-c7e75e7d03b8)


5. click on **Publish all**


