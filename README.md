## validation-rules
Validation rules for every occasion

Original Salesforce Documentation [Example Validation Rules](https://developer.salesforce.com/docs/atlas.en-us.usefulValidationRules.meta/usefulValidationRules/fields_useful_field_validation_formulas.htm).

MDK-1/4/19: Initial Entry

I've built this repository so that known good validation rules can be available, well documented, and deployable.  I can also branch a rule for whatever purpose I want and use it for other purposes without altering the original rule.

This is a public repository, so I plan on making this available to anyone that had a need to access this.  At this point I still don't know enough about Git and Github to determine whether I can build sub-repositories.  I consider this an experiment in that.

Eventually, this will expand to Triggers, their unit tests, and code.  The new Salesforce DX is supposed to allow for the reuse of Metadata (Process Builder, Flows, and other automation that can be stored, reused, and redeployed in other Salesforce Orgs I am hoping.  DX is smoking new, and I'm still learning about it.

### Conditionally make a field required by using a validation rule.

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
