# api app usando mongo db e graphql
este app foi criado em base de video aulas que podem ser reproduzidas [aqui](https://www.youtube.com/watch?v=7RoHxSGVAdU&list=PLPXWI3llyMiK9uw7tfljM2hnQl2qu6CeT)

### No momento a aplicação não starta, o erro é o seguinte:
```js
$ npx nodemon --exec babel-node src/index.js -e js,gql
[nodemon] 2.0.16
[nodemon] to restart at any time, enter `rs`
[nodemon] watching path(s): *.*
[nodemon] watching extensions: js,gql
[nodemon] starting `babel-node src/index.js`
/home/diego/projetos/api-example/node_modules/@graphql-toolkit/schema-merging/index.cjs.js:117
    const comment = graphql.getDescription(node, { commentDescriptions: true });
                            ^

TypeError: graphql.getDescription is not a function
    at pushComment (/home/diego/projetos/api-example/dist/schema-merging/src/typedefs-mergers/comments.js:32:21)
    at collectComment (/home/diego/projetos/api-example/dist/schema-merging/src/typedefs-mergers/comments.js:8:5)
    at /home/diego/projetos/api-example/dist/schema-merging/src/typedefs-mergers/merge-nodes.js:15:17
    at Array.reduce (<anonymous>)
    at mergeGraphQLNodes (/home/diego/projetos/api-example/dist/schema-merging/src/typedefs-mergers/merge-nodes.js:10:18)
    at mergeGraphQLTypes (/home/diego/projetos/api-example/dist/schema-merging/src/typedefs-mergers/merge-typedefs.js:65:25)
    at Object.mergeTypeDefs (/home/diego/projetos/api-example/dist/schema-merging/src/typedefs-mergers/merge-typedefs.js:20:22)
    at mergeTypes (/home/diego/projetos/api-example/node_modules/merge-graphql-schemas/index.cjs.js:24:26)
    at Object.<anonymous> (/home/diego/projetos/api-example/src/graphql/typeDefs.js:5:18)
    at Module._compile (node:internal/modules/cjs/loader:1105:14)

Node.js v18.1.0
[nodemon] app crashed - waiting for file changes before starting...
```