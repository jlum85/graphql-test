# Graphql

Exemple d'utilisation de GraphQL avec Node.js et Express

## Dépendances

```bash
npm install express graphql express-graphql
```

## Requête

http://localhost:3000/graphql

```js
{
	posts {
	    title
	    description
        author {
            name
            age
        }
	}
}
```

## Résultat

```js
{
  "data": {
    "posts": [
      {
        "title": "First post",
        "description": "Content of the first post",
        "author": {
          "name": "Flavio",
          "age": 36
        }
      },
      {
        "title": "Second post",
        "description": "Content of the second post",
        "author": {
          "name": "Roger",
          "age": 7
        }
      }
    ]
  }
}
```

## from

https://flaviocopes.com/graphql-node-express/
