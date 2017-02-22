# System and/or Process Synchronization using the Queue and Pump Pattern 

## Definition
In lots of scenarios the need for data synchronization between systems or process araises, in most of the cases the synchronization needs to be 
as reliable as possible the system generating the events needs to ensure that the other party receives the messages and/or events, this common
scenario could be hard to accomplish when using straight communication between the two system. A simple store and forward mechanismn can be 
accomplish by introducing a queue and a message pump. 
The coordination works as follows the message producer puts the messages on a queue and the message pump picks messages up the queue and attent to 
send them over upon delivery the message pump marks messages as delivered.

## Structure 
- Producer: Process or System that generates events or messages and queues them for delivery or synch 
- Message Queue: Data Structure that keeps the messages or events for later processing, could be persistent or not depending on needs 
- Message Pump: Send the messages to the thrid party system and upon successful delivery marks the messages on the queue as sent 

## Sample 