
Setup Instructions:   
  
SBQQ__Quote__c:  
Create field Has_Warranty__c of type Boolean 
Add field **Has_Warranty__c** to **Line Editor** field set 

SBQQ__QuoteLine__c:  
Create field Warranty_End_Date__c of type Date 
Add field **Warranty_End_Date__c** to **Line Editor** field set

Create a Custom Script called **parent-script** :  
  Paste the code in the file **parent-script** into the **Code** field \
  Add the values **product familty** and **Warranty End Date** to Quote Line Fields field 
  Add the value **Has Warranty** to Quote Fields field 
 
 Create a Custom Script called **child-script** :  
 Paste the code in the file **child-script** into the **Code** field \
  
    
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'parent-script' 

Search for the Quote Q-00021 and open it in the Quote Line Eidtor. 
