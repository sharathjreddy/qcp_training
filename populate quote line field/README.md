Setup Instructions: 

SBQQ__QuoteLine__c:\
Create field **Warranty End Date** \
Replace **Additional Discount** with **Warranty End Date** in **Line Editor** field set 
  
Create a Custom Script called **warranty-end-date** :\
  Paste the code in the file **warranty-end-date** into the **Code** field \

  **Quote Line Fields:** \
  SBQQ__ProductFamily__c
  
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'warranty-end-date' 

Search for the Quote Q-00021 and open it in the Quote Line Editor. 
