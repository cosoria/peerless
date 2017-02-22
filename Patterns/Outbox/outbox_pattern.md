# Outbox Pattern 

## Definition
This pattern is exactly like the local outbox that your preferred email client has to handle sending messages on a disconnected manner.
This pattern aim to solve the problem of temporal coupling between operations and/or system. It also aims prevent the lost of important biz events, 
it could be use to minimize the *Premature Send* scenario since the messages are queue for later delivery the system can quickly delete the messages 
from the queue reverting all actions. 

## Structure 
- Producer: Process or System that generates events or messages
- Outbox (Queue): Data Structure that keeps the messages or events for later processing, could be persistent or not depending on needs 
- Consumer: Although not part of the pattern itself the consumer or consumers read from the queue and process messages or events 

## Sample 
