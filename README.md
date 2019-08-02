# Azure Hours Databricks Day - 8/2/2019
Welcome to our landing page for our Databricks 101 tour for US EDU Azure Hour. We'll walk through three different tasks and familiarize ourselves with Azure Databricks. 

Keep in mind that our objective is **just** to familiarize ourselves, not to go very deep. Additional information on the Azure Databricks platform (like all our platforms in Azure) can be found on our [docs.microsoft.com](https://docs.microsoft.com/en-us/azure/azure-databricks/) site.

## Getting Started
1. Refer to the [Lab 1 PDF guide](Databricks_Labs/Lab_1_Getting_Started_with_Spark.pdf) to get setup on reading both the older Resilient Distributed Dataset and the newer Dataframe data constructs in Spark. [NOTE: Refer to the Setup Guide to setup the prerequisite storage accounts and clusters](Databricks_Labs/Setup_Guide.pdf)
2. Now, download the ["Databricks_Labs.zip" file for Databricks](Databricks_Labs\Databricks_Labs.zip) and import the "Dataframes.ipynb" file into your Databricks workspace
3. Follow the directions in the "Dataframes" notebook to get familiar with the Dataframes API and the dataframe construct in Spark.


## Streaming and Real-Time Machine Learning
1. We're going to be using the [Microsoft Docs](https://docs.microsoft.com/en-us/azure/azure-databricks/databricks-sentiment-analysis-cognitive-services) link to discern the sentiment of real-time, inbound tweet.
2. Setup your [Twitter API](https://docs.microsoft.com/en-us/azure/azure-databricks/databricks-sentiment-analysis-cognitive-services#create-a-twitter-application)
3. Replace the variables in the imported notebooks called "SendTweetsToEventHub" and "AnalyzeTweetsFromEventHub"
   1. **For the SendTweetToEventHub notebook:** Lines 8-11 should be the values of **Your Event Hub Namespace**, **Event Hub** you created inside the namespace container, the **SAS Policy Name** you should create on the Event Hub (not the namespace) -- TIP: give it "Manage" rights, and then the **SAS Policy Key** in that order.
   2. **For the AnalyzeTweetsFromEventHub imported notebook:** Lines 8-11 should be the values of **Your Event Hub Namespace**, **Event Hub** you created inside the namespace container, the **SAS Policy Name** you should create on the Event Hub (not the namespace) -- TIP: give it "Manage" rights, and then the **SAS Policy Key** in that order.

        AND 

        Lines 8-11 __in Cell #5__ should be the values of **Your Event Hub Namespace**, **Event Hub** you created inside the namespace container, the **SAS Policy Name** you should create on the Event Hub (not the namespace) -- TIP: give it "Manage" rights, and then the **SAS Policy Key** in that order.
    

## Batch Machine Learning
