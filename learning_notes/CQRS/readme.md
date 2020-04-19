@link: https://martinfowler.com/bliki/CommandQuerySeparation.html
@link: https://martinfowler.com/bliki/CQRS.html
@link: http://udidahan.com/2009/12/09/clarified-cqrs/
@link: http://codebetter.com/gregyoung/2010/02/16/cqrs-task-based-uis-event-sourcing-agh/


CQRS Command and Query Responsibility Segregation
Starting with CQRS, CQRS is simply the creation of two objects where there was previously only one. The separation occurs based upon whether the methods are a command or a query (the same definition that is used by Meyer in Command and Query Separation, a command is any method that mutates state and a query is any method that returns a value).

When most people talk about CQRS they are really speaking about applying the CQRS pattern to the object that represents the service boundary of the application. Consider the following pseudo-code service definition.

CustomerService

void MakeCustomerPreferred(CustomerId)
Customer GetCustomer(CustomerId)
CustomerSet GetCustomersWithName(Name)
CustomerSet GetPreferredCustomers()
void ChangeCustomerLocale(CustomerId, NewLocale)
void CreateCustomer(Customer)
void EditCustomerDetails(CustomerDetails)

 

Applying CQRS on this would result in two services


CustomerWriteService

void MakeCustomerPreferred(CustomerId)
void ChangeCustomerLocale(CustomerId, NewLocale)
void CreateCustomer(Customer)
void EditCustomerDetails(CustomerDetails)

CustomerReadService

Customer GetCustomer(CustomerId)
CustomerSet GetCustomersWithName(Name)
CustomerSet GetPreferredCustomers()

That is it. That is the entirety of the CQRS pattern.