
Setup Instructions:   
  
SBQQ__Quote__c:  
Create field **Has_Warranty__c** of type Boolean   
Add field **Has_Warranty__c** to **Line Editor** field set 

SBQQ__QuoteLine__c:  
Create field **Warranty_End_Date__c** of type Date   
Add field **Warranty_End_Date__c** to **Line Editor** field set

Create a Custom Script called **parent-script** :  
  Paste the code in the file **parent-script** into the **Code** field \
  Add the values **SBQQ__ProductFamily__c** and **Warranty_End_Date__c** to the **Quote Line Fields** field   
  Add the value **Has_Warranty__c** to the **Quote Fields** field 
 
 Create a Custom Script called **child-script** :  
 Paste the code in the file **child-script** into the **Code** field  
 (Note that this code will NOT be transpiled successfully - you will get an error message)  
    
In the Managed Package configuration, the value of the **Quote Calculator Plugin** should match the Custom Script name - 'parent-script' 

Search for the Quote Q-00021 and open it in the Quote Line Editor  
Hit the Calculate button  
a. If the **Warranty End Date** field for SMARTPHONE6 is blank, it will be populated with a date one year and one day from today   
b. The **Has Warranty** field on the Quote will be checked 

