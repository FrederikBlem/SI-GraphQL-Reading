# Research Assignment: GraphQL

[Assignment PDF.](http://https://github.com/FrederikBlem/SI-GraphQL-Reading/blob/main/A12-GraphQL.pdf "Assignment PDF.")

## Objective 
The objective of this assignment is getting familiar with the implementation of GraphQL as 
an API in service integration.
## Tasks
Your task is to research the public sources and sample implementations of GraphQL and 
formulate answers to the following questions: 
1. **What is GraphQL, what is used for, and why does it contain‘graph’in its title?** 
<br>It is a new API standard that is an alternative to REST, SOAP and RPC/gRPC. The GraphQL language was designed when Facebook required an API powerful enough to fetch data to describe all of Facebook, while retaining enough simplicity such that it would be easy to learn and use. The Query Language is not tied to any specific data source type and allows clients to define the structure required data. The same structure of data will then be returned from the server, meaning that the amount of data that needs to be returned is reduced drastically. Although it doesn't provide graph operations to the extent that might be expected from the name, it gets its name from how its queries operate on the application data graph. 
<br>More on that here: [https://www.apollographql.com/blog/graphql/basics/the-concepts-of-graphql/](https://www.apollographql.com/blog/graphql/basics/the-concepts-of-graphql/). <br>
The application data graph is similar to what you see when operating a Neo4j database, where relationships are the central focus. It seems to be the same for GraphQL and that makes sense with the context of a social media platform like Facebook.

2. **Which known drawbacks of implementing API gateways in service integration could be resolved by GraphQL?**
<br>As mentioned above, it's possible for the client to specify exactly what is needed from the server and to receive the data in the predicted way. With a REST API you'd have to sift through an entire object to get to the desired attribute, while you simply get the object's schema with only the specified attribute in return when using GraphQL query. The solved drawback is wasted data transfer.
<br>Playing on the comparison to Neo4j's relationship-defined paradigm, it's also possible to get the an attribute from all the objects that share the specified type of relationship in your GraphQL query. The solved drawback is yet again wasted data transfer and also eliminating the need for defining and implementing another endpoint in REST for example.
<br>Not being tied to a certain data structure will also help in integration tasks.
<br>The advantages above help keep microservices more lightweight because they can be specific in their queries and not need to transfer large amounts of data.

3. **How does GraphQL compare toRESTful API and gRPC? Which are the appropriate use cases for implementing each of these technologies?**
<br>
