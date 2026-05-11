# Modul 9 (Publisher) Reflection

## 1. How much data your publisher program will send to the message broker in one run?
Program publisher mengirim 5 data/event ke message broker dalam sekali jalan, karena pada kode publisher di modul ada lima kali pemanggilan publish_event untuk user berbeda: Amir, Budi, Cica, Dira, dan Emir. Modul juga menjelaskan bahwa saat cargo run dijalankan di publisher, publisher mengirim 5 events ke message broker lalu event itu diproses oleh subscriber.


## 2. The url of: "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, what does it mean?
URL tersebut berarti program publisher terhubung ke RabbitMQ sebagai message broker memakai protokol AMQP. guest pertama adalah username, guest kedua adalah password, sedangkan localhost:56732 berarti broker RabbitMQ berjalan di komputer sendiri dan menerima koneksi lewat port 5672. Di modul juga disebutkan bahwa default RabbitMQ memakai username dan password guest, serta listen di port 5672.

## Running RabbitMQ as message broker.
![Image of Running RabbitMQ](media/running.png)

## Sending and Processing Event.
![Process in Terminal](media/terminal.png)