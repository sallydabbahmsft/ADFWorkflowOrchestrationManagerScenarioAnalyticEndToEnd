
[**Back to the previous step**](/RunADFPipelines/2_Create_the_ADF_pipeline.md)

# Connect ADF to Airflow 

To run ADF pipelines from Airflow, you need to add a connection in Airflow that enables the execution of ADF pipelines as requested.
we need to register our ADF workspace in Azure Active directory 

Navigate to Azure Active Directory (AAD). Click on the Manage tab on the left side. Go to App Registrations. Search for your ADF app and select it. In the Overview tab, copy your credentials.

## Access Airflow UI:

1. Navigate to the Manage tab. Select Apache Airflow. Click on the Monitor button for your Airflow instance. This will open the Airflow UI.

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/5c6a8c5c-0e50-46f9-90ed-f9eb55bbb265)


2. Configure Connections in Airflow UI:

In the Airflow UI, go to the Admin tab. Click on the Connections tab to see a list of possible connections in Airflow. 

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/4a7f8993-b571-4af6-aaf4-50c39b9f7bd2)



3. Edit azure_default connecttion

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/b389fbeb-0735-46e9-bd93-42a3de165811)

4. Edit the connection Type and choose Azure Data Factory and fill in the required details. Obtain Client ID and Client Secret from AAD and tenant id and subscription id from ADF workspace overview:
![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/8975f6a7-dc15-4004-b8b8-0212016224d2)

Change connection id to **azure_data_factory**

Note: To ensure it works, you need to specify the Client ID of your ADF workspace and the password retrieved from Azure Active Directory.

5. click on Test button if its successfully connected then click on save.

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/10afbef1-a66e-4349-92e2-6765d57f190a)





[**Go to the next step**](/RunADFPipelines/4_Write_DAG_code.md)
