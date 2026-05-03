# REACT
COURS ET TP REACT
la documentation de API Backend est 

A- This is a REST API that exposes two models, Article and Customer, via REST. Here are the endpoints:

For customers :
- Get all customers : localhost:8080/customers
- Get customer by id : /customers/{id}
- Post : /customers
- Put : /customers/{id}
- Delete : /customers/{id}

For articles :
- Get all articles : /articles
- Get customer by id : /articles/{id}
- Post : /articles
- Put : /articles/{id}
- Delete : /articles/{id}

B- Security : 
/customers is not secured. 
/articles is secured by jwt.

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
