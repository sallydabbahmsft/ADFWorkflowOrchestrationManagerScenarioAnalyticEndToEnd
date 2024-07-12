[**Back to the previous step**](/RunADFPipelines/3_Connect_to_ADF_from_Airflow_UI.md)

# Azure Data Factory Operators in Airflow 

  we have two operators 
  1. ### AzureDataFactoryRunPipelineOperator
      we use the AzureDataFactoryRunPipelineOperator to execute a pipeline within a data factory. By default, the operator will periodically check on the status of the executed pipeline to terminate with a “Succeeded” status. This functionality can be disabled for an asynchronous wait – typically with the AzureDataFactoryPipelineRunStatusSensor – by setting wait_for_termination to False.

      Below is an example of using this operator to execute an Azure Data Factory pipeline.
      <img width="31111119" alt="image" src="https://github.com/user-attachments/assets/fb747b81-f8b5-46fb-8886-d8d8cb96d5b7">


    
  2. ### AzureDataFactoryPipelineRunStatusAsyncSensor
      we use the **AzureDataFactoryPipelineRunStatusAsyncSensor** (deferrable version) to periodically retrieve the status of a data factory pipeline run asynchronously. This sensor will free up the worker slots since polling for job status happens on the Airflow triggerer, leading to efficient utilization of resources within Airflow.

      Example
     <img width="31111119" alt="image" src="https://github.com/user-attachments/assets/a74fca6a-1d84-4cca-ba64-7ca84ac6f61c">

# DAG Code
