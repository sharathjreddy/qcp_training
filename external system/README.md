Setup Instructions:   

Deploy the Apex class **CPQB_ExtPricing** in your Salesforce Org      
    
Create a Custom Script record called **external-pricing** :  
  Paste the code in the file **external-pricing** into the **Code** field \
  **Quote Fields:**     
  
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'external-pricing' 


Search for the Quote Q-00021 and open it in the Quote Line Editor. 
Add the Products **10KWHBATTERY** and **4PORTUSBHUB** respectively. The **Special Price** fields should be overridden to **201** and **301** respectively.  




