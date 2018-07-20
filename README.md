# apollo-tutorial-kit

Followed along a tutorial from medium. Press [here](https://blog.apollographql.com/tutorial-building-a-graphql-server-cddaa023c035) 
to check it out.


## Getting started

```bash
git clone https://github.com/Benluv/GraphQL-test.git
cd apollo-starter-kit
npm install
npm start
```

Then open [http://localhost:3000/graphiql](http://localhost:3000/graphiql)

When you paste this on the left side of the page:

```graphql
{
  testString
}
```

and hit the play button (cmd-return), then you should get this on the right side:

```json
{
  "data": {
    "testString": "It works!"
  }
}
```

What follows are multiple examples that can be applied to the code in this repo:

```json
{
  author(firstName: "Edmond", lastName: "Jones") {
    firstName
    lastName
  }
}
```

```json
{
  author(firstName: "Edmond", lastName: "Jones") {
    firstName
    lastName
    posts {
      title
      views
    }
  }
}
```

```json
query FortuneCookieQuery {
  getFortuneCookie
}
```
