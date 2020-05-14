# smart-document-understanding
What is smart document understanding?
Smart Document Understanding (SDU) trains IBM Watson™ Discovery to extract custom fields in your documents. Customizing how your documents are indexed into Discovery improves the answers that your application returns.

For more info visit: 
https://cloud.ibm.com/docs/discovery?topic=discovery-sdu

The above project uses various web pages as its documents to answer different sets of questions.
Here are the instructions on how to use the above chatbox in your IBM Cloud.
Step 1: Create and IBM Cloud Account (if you dont have)
Step 2: Create the following services, IBM Watson - Assistant, Discovery, Functions.
Step 3: Follow the in-built steps in Assistant to create your first chatbox. 
        After creating, click on Import Skill and add the file skill - The COVID-19 Expert.json
Step 4: Follow the in-build steps to create your discovery
        Copy your API key and URL(On the Launch Watson Discovery page)
        Click on Connect a data source -> Web Crawl and add the following web pages:
        https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html
        https://www.cdc.gov/coronavirus/2019-ncov/prevent-getting-sick/how-covid-spreads.html   
        https://www.cdc.gov/coronavirus/2019-ncov/prevent-getting-sick/prevention.html
        https://www.cdc.gov/coronavirus/2019-ncov/prevent-getting-sick/social-distancing.html
        https://www.cdc.gov/coronavirus/2019-ncov/if-you-are-sick/quarantine-isolation.html
        https://www.ndtv.com/coronavirus/india-covid-19-tracker
        Click next and finish the steps.
        Copy your Environment ID, Configuration ID, Collection ID from the View API Details(Next to Delete Icon) 
Step 5: Follow the in-built steps to create your Action and copy and paste the code from Ask_Discovery.js file.
        In the parameter add the following one-by-one:
        iam_apikey:"<Your API KEY>"
        environment_id: "Your id"
        configuration_id:"Your id"
        collection_id:"Your id"
        url:"Your id"
        Save.

Thats it your done, open your watson assistant and click Try it.
Feel free to contact me and tell me where to improve.  
