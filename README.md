# Understanding publisher and message broker
1. How many data your publisher program will send to the message broker in onerun?

According to main.rs and function main in that file, my publisher program will send 5 messages in one run. It can be seen from the number of publish_event function calls.

2. The url of: `amqp://guest:guest@localhost:5672` is the same as in the subscriber program, what does it mean?

It means both subscriber and publisher are connecting to the same server.