# REACT
COURS ET TP REACT
le lien de LAPI backeg sur githib est : https://github.com/jeouit/api-backend-main/tree/main


la documentation de API Backend est 
A- Cette API est exposé en deux modules: Article and Customer, via REST. Ci-dessous les endpoints:

pour customers : les endpoint sans accessibles sans authentification
- Get all customers : localhost:8080/customers
- Get customer by id : /customers/{id}
- Post : /customers
- Put : /customers/{id}
- Delete : /customers/{id}

Pour articles : il faut une authentification pour accéder à article, c'est un plus dans le TP qui veux utiliser jwt
- Get all articles : /articles
- Get customer by id : /articles/{id}
- Post : /articles
- Put : /articles/{id}
- Delete : /articles/{id}

B- Security : 
/customers est non sécurisé 
/articles est sécurisé avec jwt.

C- For authentication :
There are two users : admin/admin and client/client

for admin user, he has the role ADMIN_ROLE and the following authorities : 
        GET_ALL_ARTICLES, 
        GET_ARTICLE_BY_IDENTITY,
        CREATE_ARTICL,
        UPDATE_ARTICLE,
        DELETE_ARTICLE,
        SEARCH_ARTICLE

for the client user, he has the role CLIENT_ROLE and the following authorities : 
        GET_ALL_ARTICLES, 
        GET_ARTICLE_BY_IDENTITY,
        SEARCH_ARTICLE

D- /auth/signin to get a jwt token
