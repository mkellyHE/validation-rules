It's possible to conditionally make a field required by using a validation rule.

Resolution	
The following Validation Formula can be used as a reference.

    AND(Account_Market = "Corporate", Test = "")

This will give an error message if "Test" has no value when Account Market is "Corporate". 
 

Create validation rule in Salesforce Classic
 
1. Click Setup.
2. Under "Build," click Customize | [the object you need to modify] | click Validation Rules. 
3. Click New.
4. Enter the Validation Rule name.
5. Set the Validation Formula as per the suggestion above, feel free to adapt to your needs.
6. Set the error message that the User will receive. 
7. Click Save.
