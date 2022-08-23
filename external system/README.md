Setup Instructions:   

Deploy the Apex class **CPQB_ExtPricing** in your Salesforce Org      
    
Create a Custom Script record called **external-pricing** :  
   a. Paste the code in the file **external-pricing** into the **Code** field \
   b. Enter **SBQQ__ProductCode__c** in the **Quote Line Fields** field.
  
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'external-pricing' 

Add the URL **https://qcp-pricing-api.herokuapp.com** to **Remote Site Settings**. 

Search for the Quote Q-00021 and open it in the Quote Line Editor. 
Add the Products **10KWHBATTERY** and **4PORTUSBHUB** to the Quote   
The **SBQQ__SpecialPrice__c** fields should be overridden to **201** and **301** respectively.  
The **SBQQ__SpecialPriceType__c** fields will be set to 'Custom'   
The **SBQQ__SpecialPriceDescription__c** fields will be set to 'Price received from External System'    






