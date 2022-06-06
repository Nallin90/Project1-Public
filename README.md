# Project 1
>##### _Description:_
>>Create a backend of an online store to buy products. Users can register an account and login to add items into a cart. Then they can can place orders based on the items in their cart. The information that contains the users, items, carts, the items in those carts, and the orders are all stored in their respective tables.

#### _Features Implemented:_
- _**Register**_ - Users are able to be registered
- _**Login/Logout**_ -Registered users are able to be logged in or out
- _**Get Users**_ - Registered users are able to get all users and their carts
- _**Shop (Get Items)**_ - Users can view all the items available in the store
- _**Carts**_ - Registered users can add selected items to their cart
- _**Checkout**_ - Registered users can add items from the cart to their placed orders


>#### _Technologies Used:_
>- _**DBeaver**_
>- _**Spring Framework**_ (Spring Boot, Spring Data, Spring Web)
>- _**Logback**_
>- _**Postgresql**_

#### _Getting Started:_

- Compile and run ProjectoneApplication
- Open PostMan and use each url with the associated method next to it while copying the information under as the JSON for POST and PUT operations
  - For ***Register*** : **POST** http://localhost:8085/user/register 
    - {
      "email": "funky@gmail.com",
      "password": "funky"
      }
  - For ***Login***: **POST** http://localhost:8085/login
    - {
      "email": "fancyman@fancy.com",
      "password": "fancy"
      }
  - For ***Logout*** : **POST** http://localhost:8085/logout
  - To ***Get All Users*** (Must be logged in first): **GET** http://localhost:8085/user/all
  - To ***Get All Items*** : **GET** http://localhost:8085/shop
  - To ***Get a single Item*** : **GET** http://localhost:8085/shop/29
  - To ***Add an item into the shop*** : **POST** http://localhost:8085/shop
    - {
      "itemName": "Character Skin 5",
      "price": "9.99"
}
  - To ***Add an item into the cart*** : **PUT** http://localhost:8085/user/cart/add
      - { "itemId": 46 }
  - To ***Add a cart to an order*** : **POST** http://localhost:8085/user/order/add

