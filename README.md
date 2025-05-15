a. How many data your publlsher program will send to the message broker in one
run? 
> During a single execution, the publisher program transmits 5 pieces of data to the message broker.

b. The url of: "amqp://guest:guest@localhost:5672" is the same as in the subscriber
program, what does it mean?
> The identical URL indicates that both the publisher and subscriber components are connecting to the same message broker instance for their communication.

Running RabbitMQ as message broker
![img](image.png)

Sending and processing event.
![img](image2.png)
The screenshot demonstrates the complete workflow: the publisher establishes a connection to the message broker via AMQP, generates and transmits 5 user creation events, which are then received by the separate subscriber service that processes and outputs the event data.

Monitoring chart based on publisher.
![img](image3.png)

The spike on the graph indicates that the publisher sends several messages at a time and after done sending the message, the graph goes down again, indicating that the job has decreased and eventually gets to 0 again.