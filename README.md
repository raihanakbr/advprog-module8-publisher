# Understanding publisher and message broker
1. How many data your publisher program will send to the message broker in onerun?

According to main.rs and function main in that file, my publisher program will send 5 messages in one run. It can be seen from the number of publish_event function calls.

2. The url of: `amqp://guest:guest@localhost:5672` is the same as in the subscriber program, what does it mean?

It means both subscriber and publisher are connecting to the same server.

- Running RabbitMQ
![RabbitMQ](https://cdn.discordapp.com/attachments/874575252808667149/1231990729052786809/image.png?ex=6638f7c7&is=662682c7&hm=de464023d3afffe82e70a7449c9334bb12da2a47666273438bf46c7c1abf0d5d&)

- Subscriber Terminal
![Subscriber](https://media.discordapp.net/attachments/874575252808667149/1231994315023061044/image.png?ex=6638fb1e&is=6626861e&hm=72f2d443903487e5f7ee79be24783ca01c844dd78e3c74336c6fdedfe01654a8&=&format=webp&quality=lossless&width=1440&height=106)
It can be seen from the image that there are 5 incoming messages that are caught by the subscribers from the publisher.
