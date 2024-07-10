[**Back to the Readme section**](/README.md)

# Prerequisites
1. **Azure subscription**: If you don't have an Azure subscription, create a free account before you begin.
2. **Azure Data Factory**: Create or select an existing Data Factory instance in the region where the Workflow Orchestration Manager preview is supported.

# Create the environment
To create a new Workflow Orchestration Manager environment:

1. Go to the **Manage hub** and select Airflow (Preview) > + New to open the Airflow environment setup page.

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/729e83aa-486a-4d41-9a91-cbaa26292dc2)

2. Enter information and select options for your Airflow configuration.

![image](https://github.com/sallydabbahmsft/ADFWorkflowOrchestrationManagerScenarioAnalyticEndToEnd/assets/105279899/81ebaa2b-c841-491d-958e-001da317d523)




3. When you use Basic authentication, remember the username and password specified on this page. You need them to sign in later in the Airflow UI. The default option is Azure AD. It doesn't require creating a username and password for your Airflow environment. Instead, it uses the signed-in user's credential for Azure Data Factory to sign in and monitor directed acyclic graphs (DAGs).

 Select create - it might take around 20 minutes to set-up the airflow emnviroment


[**Go to the next step**](/Analytics%20-%20How%20To%20Proceed/2_Create_the_ADF_pipeline.md)
