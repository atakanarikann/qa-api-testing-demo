# API Bug Reports — ReqRes API

## BUG-01 — POST /users accepts empty body
Expected: 400  
Actual: 201 created  

## BUG-02 — GET /users/{id} returns incorrect schema on invalid ID
Expected: “user not found”  
Actual: Empty object  

## BUG-03 — PUT /users/{id} accepts malformed JSON

## BUG-04 — DELETE returns 204 even when user does not exist

## BUG-05 — POST accepts numeric “name”

## BUG-06 — Response time spikes over 1.5s occasionally

## BUG-07 — Missing rate limiting

## BUG-08 — PUT endpoint does not validate field types
