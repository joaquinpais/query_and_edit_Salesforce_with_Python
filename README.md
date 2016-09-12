# query_and_edit_Salesforce_with_Python
Example of how to query, analyse, and insert Salesforce data using Python.

This workbook originates from a user request to have a field on each Lead / Contact record in Salesforce with a total of the number of calls they have received. The purpose of this workbook is to use the Simple-Salesforce Python package to extract all completed Tasks with a subject containing the word 'call', then total these up for each Lead/Contact and populate a custom field 'Number_Of_Calls__c' on each Lead/Contact record. (I.e. this workbook is to populate the total for all calls already recorded in the database. After this a workflow is switched on which will add 1 to the total every time a new call is recorded.)

If you are a Salesforce admin you can use this workbook with your own credentials on your Salesforce org - the only prerequisite is to add custom fields with field name 'Number_Of_Calls__c' to the Lead and Contact objects.

(Yes this would be perfectly possible using CSV exports and the dataloader, but it's more fun in Python!)

For more information you can find schema details for the Task object here:

  https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_erd_activities.htm

And Simple-Salesforce documentation can be found here:

  https://pypi.python.org/pypi/simple-salesforce
