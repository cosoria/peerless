# Outbox Pattern 
----

## Definition
This pattern is exactly like the local outbox that your preferred email client has to handle sending messages on a disconnected manner.
This pattern aim to solve the problem of temporal coupling between operation or system and to prevent the lost of important biz events, 
it could be also use to minimize the *Premature Send* scenario as messages are queue for later delivery.

## Structure 
- Producer
- Outbox (Queue) 
- Consumer 

## Sample 