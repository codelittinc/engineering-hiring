# GraphQL

## Basic

1. **Which benefits does a GraphQL client bring to a project?**
   - GraphQL's declarative model helps you create a consistent, predictable API you can use across all of your clients. As you add, remove, and migrate back-end data stores, that API doesn't change from the client's perspective. Even with many other advantages, GraphQL's single greatest benefit is the developer experience it provides. It's straightforward to add new types and fields to your API, and similarly straightforward for your clients to begin using those fields. This helps you design, develop, and deploy features quickly.
2. **Is GraphQL a Database Technology?**
    - No. GraphQL is often confused with being a database technology. This is a misconception, GraphQL is a query language for APIs - not databases. In that sense it’s database agnostic and can be used with any kind of database or even no database at all.
3. **What is GraphQL?**
    - GraphQL is a query language created by Facebook in 2012 which provides a common interface between the client and the server for data fetching and manipulations. The client asks for various data from the GraphQL server via queries. The response format is described in the query and defined by the client instead of the server: they are called client‐specified queries. The structure of the data is not hardcoded as in traditional REST APIs - this makes retrieving data from the server more efficient for the client.
4. **How to do Error Handling in GraphQL?**
    - A successful GraphQL query is supposed to return a JSON object with a root field called "data". If the request fails or partially fails (e.g. because the user requesting the data doesn’t have the right access permissions), a second root field called "errors" is added to the response: `{"data": { ... }, "errors": [ ... ]}`
5. **Explain the main difference between REST and GraphQL**
    - The main and most important difference between REST and GraphQL is that GraphQL is not dealing with dedicated resources, instead everything is regarded as a graph and therefore is connected and can be queried to app exact needs.