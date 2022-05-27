# api app usando mongo db e graphql
este app foi criado em base de video aulas que podem ser reproduzidas [aqui](https://www.youtube.com/watch?v=7RoHxSGVAdU&list=PLPXWI3llyMiK9uw7tfljM2hnQl2qu6CeT)

### No momento a aplicação não starta
tive q fazer alguns ajustes:
* primeiro que a versão instalada por padrão do graphql não funcionou direito, voltei pra outra versão e agora funciona (era o graphql 16.4.0 daí mudei para o graphql 15.7.2)
* mudei um import tbm para usar o PubSub no StartServer (adicionei a dependencia do "graphql-subscriptions": "^2.0.0")
* adicionei um argumento para expor a porta do container para o host

### para utilizar esta aplicação
instale as dependencias
```shell
yarn
```

inicie o mongo pelo docker
```shell
docker pull mongo
docker run -p 27017 --name mongo -d mongo:latest
```

inicie o app
```shell
yarn dev
```