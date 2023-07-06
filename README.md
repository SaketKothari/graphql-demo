# [graphql-demo](https://www.apollographql.com/docs/apollo-server/getting-started)
* A query language (Alternative to REST API)
* GraphQL is a flexible Query Language that you can use to fetch data from a server, as well as mutate (change) data as well.
* It can be used as an alternative to a REST API, which can suffer from a few drawbacks as your application scales.
* In this repo, I set up a GaphQL server, and then make queries & mutations to that server from the browser.

#

### Disadvantages of REST API
1) Overfetching of data (Getting back more data)
2) Underfetching (Getting back less data)
3) Multiple round trips
4) Versioning and backward compatibility

#

### How GraphQL works
* **Schema Definition Language (SDL)**: In GraphQL, you define a schema using the Schema Definition Language (SDL). The schema defines the types of data available in your API 
and the relationships between them. It includes object types, fields, arguments, and directives.

* **Querying Data**: With GraphQL, clients can request exactly the data they need and nothing more. The client sends a query to the GraphQL server specifying the fields and relationships it wants to retrieve.
The server responds with a JSON object that matches the structure of the query.

* **Resolving Data**: The server's job is to resolve the requested data and return it to the client. When a query is received, the server determines the fields that need to be resolved and invokes the appropriate resolver functions.
Resolvers are responsible for fetching the data from various sources (databases, APIs, etc.) and returning the requested data.

* **Single Endpoint**: Unlike REST APIs that typically have multiple endpoints for different resources, GraphQL has a single endpoint (e.g., /graphql). This means that clients can retrieve all the required data with a single request, reducing the
  number of round trips and improving efficiency.

* **Mutations**: GraphQL also supports mutations, which are used for creating, updating, and deleting data. Mutations follow a similar structure to queries but use different keywords like "mutation" instead of "query". They allow clients to modify data on the server using defined mutation operations.

* **Strong Typing**: GraphQL enforces a strong typing system, meaning that the types of the data are explicitly defined in the schema. This helps catch errors early and provides better documentation and validation for clients.

* **Subscriptions**: GraphQL supports real-time data updates through a feature called subscriptions. Clients can subscribe to specific events or data changes and receive updates whenever those events occur. Subscriptions are typically implemented using websockets or other similar technologies.

#

### Test the queries - Postman of GraphQL
https://studio.apollographql.com/sandbox/explorer/

Once the server is running, you can access the GraphQL Playground at http://localhost:4000/graphql. The GraphQL Playground provides an interactive interface for testing and exploring your GraphQL API.

``` npm pkg set type="module" (to use ES6)  ```

#

### Resources

Here are some resources to learn more about GraphQL:

- [Apollo Server Documentation](https://www.apollographql.com/docs/apollo-server/)
- [GraphQL Official Website](https://graphql.org/)
- [GraphQL Learning Resources](https://graphql.org/learn/)
- [Apollo GraphQL Community](https://community.apollographql.com/)

  
