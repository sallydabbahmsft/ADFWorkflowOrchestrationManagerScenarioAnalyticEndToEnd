[**Back to the previous step**](/RunADFPipelines%20-%20How%20To%20Proceed/1_Create_Airflow_environment_in_Workflow_Orchestration_Manager.md)

# Create ADF Pipeline

[What is the Copy Activity:]([https://learn.microsoft.com/en-us/azure/databricks/lakehouse/medallion](https://learn.microsoft.com/en-us/azure/data-factory/quickstart-hello-world-copy-data-tool))

in this step we want to create copy activity that will copy local file to my Azure Blob Storage account, if you wish to run different pipeline you might want to skip this step.


## Create Copy Activity

 Download the *dimension_customer.csv* file from the [Fabric samples repo](https://github.com/microsoft/fabric-samples/blob/689e78676174d4627fc3855165bde9100cb4d19e/docs-samples/data-engineering/dimension_customer.csv).
   

1. From ADF studio, in **Author** tab, select **New Pipeline** , **Activities** drop down list will open, drag and drop copy activity:
   
   
2 . In **Source** tab, select local file: 
     ![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/f6c1ed51-2c9a-43eb-8c10-91b36536bff6)

   
3. Select **Continue** and select the file, in my case its .csv file (you can d.

## Ingest Sample data

HowYou will learn how to import data from Csv files using a Data Flow Gen 2 in MS Fabric.

1. Download the *dimension_customer.csv* file from the [Fabric samples repo](https://github.com/microsoft/fabric-samples/blob/689e78676174d4627fc3855165bde9100cb4d19e/docs-samples/data-engineering/dimension_customer.csv).
   
2. In the **Lakehouse explorer**, you see options to load data into lakehouse. Select New Dataflow Gen2.
   ![Dataflow Gen2](https://github.com/sallydabbahmsft/FabricScenarioAnalyticEndToEnd/assets/105279899/bbbd7e7e-57dc-40d1-8b17-0e5b2bb178ff)

3. On the new dataflow pane, select Import from a Text/CSV file.
   
4. On the Connect to data source pane, select the Upload file radio button. Drag and drop the dimension_customer.csv file that you downloaded in step 1. After the file is uploaded, select Next.
   ![Connection Setting](https://github.com/sallydabbahmsft/FabricScenarioAnalyticEndToEnd/assets/105279899/c9dd00e9-39a2-4c8d-a733-777c7ff66a79)
   
5. From the **Preview file data** page, preview the data and select Create to proceed and return back to the dataflow canvas.
   
6. In the **Data destination** pane, click on **Settings** 
  ![datadestination](https://github.com/sallydabbahmsft/FabricScenarioAnalyticEndToEnd/assets/105279899/c7da1f90-5ec7-46d9-9609-956cae1f2919)

   
7. If needed, from the **Connect to data destination** screen, sign into your account. Select **Next**.
   
