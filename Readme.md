#### Setup


`git clone git@github.com:michaelchemani/mw-consumer.git`

`cd mw-consumer && java -jar target/consumer-1.0-SNAPSHOT.jar` -> will bootstrap the consumer

retail -> `git checkout kafka-producer-poc`

ecom -> `git checkout kafka-consumer-poc`

'cd ecom/www/backend/public && php -S localhost:8888' -> will launch e-com internal API

Since we do not handle authentication yet, you ecom store id will have to hardcoded.

Edit `ecom/www/backend/public/consume.php` update your store id line 26 and 30.


#### Run that

Create products using retail-cli (`retail seed -p 100 -b 0 -c 0`)