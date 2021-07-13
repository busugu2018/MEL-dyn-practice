# MEL-dyn-practice

Mule Expression Language Examples

These examples introduce some basic implementations of Mule Expression Language (MEL). Each example includes a step-by-step guide for creating the flow in Studio’s visual editor or in XML. You can also jump straight to the complete code for all six examples, which you can copy and manipulate further in your own applications.



Example 1 – Accessing Properties

This example creates a simple web service that takes an HTTP request that includes a username parameter and returns a greeting using that username.
In this example, you can use MEL to:
 - Access an inbound property
 - Dynamically set the payload



Example 2 – Dynamic Routing by Evaluating a Condition

In the previous example, if your call to the service doesn’t include a username parameter, it results in an error. You can prevent this from happening by adding some flow control components. This example includes a Choice Router that verifies if the required parameter is being passed.
In this example, you can use MEL to:
 - Evaluate conditions in a choice component
 - Access an inbound property
 - Dynamically set the payload



Example 3 – Variable Assignment and Evaluating Conditions

In this example, the service saves a CSV file with user data besides just returning a greeting. The call to the service now includes two parameters, username and age. The service stores these two parameters and adds a third boolean parameter that evaluates if the user is above a certain age (if age is > 18).
In this example, you uses MEL to:
 - Set a flow variable in the message
 - Generate an output based on evaluating the input
 - Access an inbound property
 - Dynamically set the payload




Example 4 – Using Xpath
In all the previous examples, calls to the service were made via GET requests that included query parameters. In this example, the service you create is an API that accepts POST requests with XML bodies. The required XML includes two parameters, username and age. The service stores these two parameters and adds a third boolean parameter that evaluates if the user is above a certain age (if age > 18)
In this example, you use MEL to:
 - Set a flow variable in the message
 - Generate an output based on evaluating the input
 - Parse an XML input through an xpath query
 - Dynamically set the payload





Example 5 – Working with Java Objects

This example is just like example 4, except that the service now receives JSON inputs rather than of XML.
The JSON input includes two parameters, username and age. The service stores these two parameters and adds a third boolean parameter that evaluates if the user is above a certain age (if age>18). Mule first transforms the JSON object into a Java object so that MEL expressions can access the object’s attributes.
In this example, you can use MEL to:
 - Set a flow variable in the message
 - Generate an output based on evaluating the input
 - Access a Java object’s attributes
 - Dynamically set the payload

