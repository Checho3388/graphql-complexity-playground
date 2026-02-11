# `graphql-complexity` Playground 🚀

A live, interactive environment to explore the [**graphql-complexity**](https://github.com/Checho3388/graphql-complexity) library in action.

This playground runs a [FastAPI](https://fastapi.tiangolo.com/) server integrated with [Strawberry GraphQL](https://strawberry.rocks/) to demonstrate how to implement cost-based analysis for your GraphQL API.

---

## ⚡ Live Demo
No installation required. You can access the hosted GraphiQL interface directly:

👉 **[Launch Playground on Railway](https://graphql-complexity-playground-production.up.railway.app/)**

---

## 🧐 What is this for?
In GraphQL, a single query can be deeply nested or request a massive amount of data, potentially leading to "Denial of Service" (DoS) scenarios. 

`graphql-complexity` protects your server by:
1.  **Parsing** the incoming query.
2.  **Calculating** a "cost" based on field depth and multipliers.
3.  **Rejecting** the query before execution if it exceeds your defined limit.
