# systogether-quickbooks

##Description
SysTogether syncs Salesforce with Quickbooks Online

#Table of Contents

#Installation

#Usage
SysTogether includes an Apex wrapper that makes it easy to interact with Quickbooks.

````apex
Account a = new Account();
a.Name = 'Test Customer';
st4qb.Obj obj = new st4qb.Obj(a);
obj.save();
a = (Account)obj.get('sfRecord');
system.debug(a.Quicbooks_Id__c);
update a;
````

#Contributing
