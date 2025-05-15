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

Monitoring chart based on publisher.
![img](image3.png)