Setup Instructions: 

SBQQ__Quote__c:
Create field **Warranty End Date** \
Add field **SBQQ__PartnerDiscount__c** in **Line Editor** field set 
  
SBQQ__Quote__c:\
Add field **Markup (%)** to **Line Editor** field set
  
Create a Custom Script called **negotiated-discount** :  
  Paste the code in the file **negotiated-discount** into the **Code** field \
  **Quote Fields:** \
  SBQQ__Account__c  
    
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'negotiated-discount' 

Search for the Quote Q-00021 and open it in the Quote Line Eidtor. 
