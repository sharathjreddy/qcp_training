Setup Instructions:   
  
Create a Custom Object (with tab) -   
Label: Partner Discount  
API Name: Partner_Discount  
  
Record Name:  
Partner Discount #  
Data Type: Auto Number   
Format: {00000000}  
Starting value: 1  
  
Create 2 Fields -   
Account : Lookup to Account object  
Discount : Percent(3,2)  
  
Create atleast one record -   
a. Account - select the Account associated with the Quote that you are testing   
b. Discount - Enter a Discount value   

SBQQ__Quote__c:  
Add field **SBQQ__PartnerDiscount__c** to **Line Editor** field set 
    
Create a Custom Script called **negotiated-discount** :  
  Paste the code in the file **negotiated-discount** into the **Code** field \
  **Quote Fields:** \
  SBQQ__Account__c  
    
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'negotiated-discount' 

Search for the Quote Q-00021 and open it in the Quote Line Eidtor. 
