Setup Instructions: 

SBQQ__QuoteLine__c:\
Create field **Warranty End Date** \ 
Replace **Additional Discount** with **Warranty End Date** in **Line Editor** field set 
  
SBQQ__Quote__c:\
Add field **Markup (%)** to **Line Editor** field set
  
Create a Custom Script called **psp-example** :\
  Paste the code in the file **psp-example** into the **Code** field \
  **Quote Fields:** \
  SBQQ__MarkupRate__c \
  SBQQ__CustomerDiscount__c \
  **Quote Line Fields:** \
  SBQQ__ProductFamily__c \
  
In the Managed Package configuration, the value of the Quote Calculator Plugin should match the Custom Script name - 'psp-example' 
