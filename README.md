# CustomersAPI

 This API is to demonstrate the following Use Cases:

-> List existing customers in the system: 
* GET Method -> retrieves the list of customers and also added query parameter to fetch from the last modified date.

-> Retreive and update customers via a mobile application:
* GET & PUT Method supports the individual(/Customers/{id}) as well bulk(/customers ) updation/retrieving the customers

-> Extension of the API to support resources such as orders and products: 
* It would be very simple to re-use the existing call structures, rename the /customers to /orders (for example), define an order object and alter the !includes. 
  The same can be applicable for Products as well. 


#Comments on design decisions:

* Used selection RAML which effectively inherits the concept of collection in RAML that inherits resourceType and traits for any future resources ( such as orders, Products ). It is one of the way to re-use the RAML design for future enhancements.
* Didnt explain Securities in detail as we can try the same from API Manager.
