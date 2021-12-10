# Research Assignment: GraphQL

[Assignment PDF.](http://https://github.com/FrederikBlem/SI-GraphQL-Reading/blob/main/A12-GraphQL.pdf "Assignment PDF.")

## Objective 
The objective of this assignment is getting familiar with the implementation of GraphQL as 
an API in service integration.
## Tasks
Your task is to research the public sources and sample implementations of GraphQL and 
formulate answers to the following questions: 
1. **What is GraphQL, what is used for, and why does it contain‘graph’in its title?** 
<br>It is a new API standard that is an alternative to REST, SOAP and RPC/gRPC. The GraphQL language was designed when Facebook required an API powerful enough to fetch data to describe all of Facebook, while retaining enough simplicity such that it would be easy to learn and use. The Query Language is not tied to any specific data source type and allows clients to define the structure required data. The same structured will then be returned from the server, meaning that that amount of data that needs to be returned is reduced drastically. Although it doesn't provide graph operations to the extent that might be expected from the name, it gets its name from how its queries operate on the application data graph. 
<br>More on that here: [https://www.apollographql.com/blog/graphql/basics/the-concepts-of-graphql/](https://www.apollographql.com/blog/graphql/basics/the-concepts-of-graphql/). <br>
The application data graph is similar to what you see when operating a Neo4j database, where relationships are the central focus. It seems to be the same for GraphQL and that makes sense with the context of a social media platform like Facebook.
2. **Which known drawbacks of implementing API gateways in service integration could be resolved by GraphQL?**
<br>My answer.
3. **How does GraphQL compare toRESTful API and gRPC? Which are the appropriate use cases for implementing each of these technologies?**
<br>My answer.
