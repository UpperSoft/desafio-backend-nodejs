# Desafio Back-end UpperSoft


Abaixo você encontrará todos as informações necessárias para iniciar o seu teste.

## Avisos antes de começar

- Crie um repositório no seu GitHub.
- Faça seus commits no seu repositório.
- Envie o link do seu repositório para o email **alexandre@uppersoft.com.br**.
- Qualquer dúvida referente a especificação do Desafio, abra uma issue e fique a vontade para perguntar, nós apreciamos isso.
- Você poderá consultar o Google, Stackoverflow ou algum projeto particular na sua máquina.
- Dê uma olhada nos [Materiais úteis](#materiais-úteis).
- Fique tranquilo, respire, assim como você, também já passamos por essa etapa. Boa sorte! :)

*Corpo do Email com o link do repositório do desafio*

>Seu Nome
>
>Breve descrição 
>
>Link do repositório
>


## Objetivo: Pokedéx API

Você é um desenvolvedor de software no mundo de Pokémon e quer desenvolver uma aplicação para auxiliar aqueles que se aventuram a serem treinadores Pokémon. Seu objetivo hoje é criar uma API REST onde os aventureiros possam consultar dados valiosos sobre os pokémons existentes.

Você pode consumir a rota abaixo para receber os dados dos 151 pokémons originais (pokédex):

https://raw.githubusercontent.com/Biuni/PokemonGO-Pokedex/master/pokedex.json

Mas são muitos dados! Para simplificar a vida dos treinadores, você vai criar rotas onde eles possam consultar dados específicos de interesse. Após refletir, você concluiu que os seguintes endpoints são necessários:

Método | Endpoint | Descrição
:--------- | :------: | :-------:
| (GET) | /api/v1/pokemon | retorna os nomes de todos os pokémons existentes. |
| (GET)  | /api/v1/pokemon/{nome-pokemon} | retorna os dados do pokémon especificado. |
| (POST) | /api/v1/advantage/{nome-pokemon} | retorna a lista dos pokémons que são fracos contra o pokémon informado.
| (POST)  | /api/v1/weakness/{nome-pokemon} | retorna a lista dos pokémons que são fortes contra o pokémon informado.


Requisitos:

 - Use EXPRESS.JS para criar o servidor
 - Crie um arquivo chamado README.md contendo as instruções de execução. (Justifique as suas escolhas.)
 - Não baixe os dados da pokédex na  forma de arquivo! A pokédex deve ser consultada via http request ao iniciar o servidor ou em cada requisição (fica a seu critério escolher).
 - Os dados devem ser retornados em formato JSON
 - Faça um tratamento de erros básico (ex.: usuário informa pokémon que não existe)
 - {nome-pokemon} não deve ser case-sensitive, ou seja, enviar “Ivysaur” ou “ivysaur” deve trazer o mesmo resultado.


## O que será avaliado e valorizamos :heart:
- Documentação
- Código limpo e organizado (nomenclatura, etc)
- Ser consistente e saber argumentar suas escolhas
- Apresentar soluções que domina
- Versionamento de código (repositório, branches, padrões de commit etc)
- Manutenibilidade do Código
- Tratamento de erros
- Cuidado com a segurança
- Arquitetura (estruturar o pensamento antes de escrever)
- Modularização (divisão do código camadas)

De acordo com os critérios acima, iremos avaliar seu teste para avançarmos.

## O que NÃO será avaliado :warning:
- Autenticação

## O que será um Diferencial
- Uso de Docker
- Persistência de dados em Banco de Dados (NoSQL ou SQL)
- Testes de [integração](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing)
- Testes [unitários](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing)
- Uso de Design Patterns
- Documentação
- Proposta de melhoria na arquitetura
- Frontend


## Materiais úteis
- https://expressjs.com/
- https://medium.com/xp-inc/criando-uma-api-node-em-10-passos-com-express-js-52b2d612a8a9
- https://axios-http.com/docs/api_intro
- https://developer.mozilla.org/pt-BR/docs/Web/HTTP/CORS