# API Test Cases — ReqRes API

## GET /users?page=1
TC01 — Response status should be 200  
TC02 — Response time < 1s  
TC03 — “page” field equals 1  
TC04 — “data” array length > 0  
TC05 — Validate user fields: id, email, first_name, last_name  

## GET /users/{id}
TC06 — Valid user ID returns 200  
TC07 — Invalid user ID returns 404  
TC08 — Response matches schema  

## POST /users
TC09 — Valid POST returns 201  
TC10 — Missing name returns error (negative)  
TC11 — Validate fields in response: id, createdAt  

## PUT /users/{id}
TC12 — Valid PUT returns 200  
TC13 — Update timestamp should change  

## DELETE /users/{id}
TC14 — Valid DELETE returns 204  
TC15 — Deleting invalid user returns 404  

## Negative Tests
TC16 — Invalid method returns 405  
TC17 — Wrong content-type returns 400  
TC18 — Numeric values in string fields rejected  
TC19 — Missing body returns 400  
TC20 — SQL injection-style payload blocked  
