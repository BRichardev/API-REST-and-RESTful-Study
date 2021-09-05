<p align="center">
<img src="https://img.shields.io/badge/Insomnia-5849be?style=for-the-badge&logo=Insomnia&logoColor=white">
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">
<img src="https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white">
<img src="https://img.shields.io/badge/Yarn-2C8EBB?style=for-the-badge&logo=yarn&logoColor=white">

# 🚀 Primeiro Passos

```
Para fazer com que o projeto funcione siga esse passo a rísca:
Clone este projeto e em seu terminal baixe as dependências essas sendo
npm install yarn
yarn init -y
npm install express
```

### Links importandos
Link para o Insomnia: [Insomnia Download](https://insomnia.rest/download)

<h1 align="center">Exemplo em foto de como seu package.json deve ficar</h1>
<p align="center">
  <img src="img/Captura de Tela (135).png" width="900" title="package.json exemplo">
</p>


# API, REST e RESTFUL

## API
Cliente (Cliente)<br />
Garçom (pedidos, levar seus pedidos, para a cozinha) (API) <br />
Cozinha (Server) <br />

Aplication Programming Interface - API é basicamente um<br />
conjuntos de rotinas e padrões estabelecidos por uma aplicação,<br />
para que outras aplicações possam utilizar as funcionalidades<br />
desta aplicação

- Responsável por estabelecer comunicação entre diferentes serviços
- Meio de campe entre as tecnologias
- Intermediador para troca de informações

## REST

Restaurante<br />
Limpinho,<br />
Que te atenda bem,<br />
te de aquli que vc pediu<br />

Cliente,<br />
Gritando,<br />
Xingando<br />

Boas práticas

A tranferência de dados,é geralmente usando o protoclo HTTP
HTTP - Um acrônimo/significado para REpresentational Stete Transfer<br />
(Transferência de Estado Representativo)<br />

Será feita a transferência de dados de uma maneira simbólica,
figurativa, representativa, de maneira didática<br />

O REST, delimita algumas obrigações nessas tranferências de dados.<br />

Resources seria então, uma entidade, um objeto.<br />

### 6 NECESSIDADES (Constraints) para ser RESTful

- _Client-server_: Separação do cliente e do armazenamento de dados<br />
 (servidor), dessa forma, poderemos ter uma portabilidade do nosso sistema,<br />
 usando o React para WEB e React Native para o smartphone, por exemplo.<br />

 - _Stateless_: Cada requisição que o cliente faz para o servidor
 deverá conter todas as informações necessárias para o servidor entender
 e reponder (RESPONSE) a requisição (REQUEST).<br />
 Exemplo: A sessão do usuário deverá ser enviada em todas as requisições, para saber<br />
 se aquele usuário está autenticado e apto a usar os serviçços, e o servidor não pode<br />
 lembrar que o cliente foi atutenticado na requisição anterior. Nos nossos, cursos temos por<br />
 padrão usar os tokens para as comunicações.

 - _Cacheable_: As respostas para um requisição, deverão ser explicitas ao dizer aquela resquição, pode ou não ser cacheada pelo cliente.

 - _Layered System_: O cliente acessa um endpoint, sem precisar saber da complexidade, de quais passos estão sendo<br /> necessários para o servidor responder requisição, ou quais outras camadas o servidor estará lidando, para que a requisição seja respondida

 https://graph.facebook.com/youtube = endpoint// a url que seria o caminho que o servidor faz para achar esse link<br />

 - _Code on demand (optional)_: Dá a possibilitade da nossa aplicação pegar códigos, como o javascript por exemplo, e executar no cliente 

## RESTFUL

RESTful, é a aplicação dos padrões REST.<br />

## BOAS PRÁTICAS

- Utilizar verbos HTTP para nossa requisições.<br />
- Utilizar plural ou singular na criação dos endpoints? _NÃO IMPORTA!_ user um padrão!!<br />
- Não deixar barra no final do endpoint<br />
- Nunca deixe o cliente sem resposta

### Usar Verbos HTTP

// Verbos HTTP<br />
// GET: Receber dados de um Resource<br />
// POST: Enviar dados ou informações para serem processados por um Resource<br />
// PUT: Atualizar dados de um Resource<br />
// DELETE: Deletar um Resource

### STATUS DAS RESPOSTAS

- 1xx: Informação
- 2xx: Sucesso
    - 200: OK
    - 201: CREATED
    - 204: Não tem conteúdo PUT POST DELETE
- 3xx: Redirection
- 4xx: Cliente Error
    - 400: Bad Request
    - 404: Not Found!
- 55x: Server Error
    500: Internal Server Error
