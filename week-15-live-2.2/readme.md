in this we are going to connect the database using volumes and also do the network thingy

``` bash
docker run -d -v volume_db:/data/db --name mongo --network my_custom _network -p 27017:27017 mongo
```

```bash
docker run -d -p 3000:3000 --name db _demo_app --network my_custom_network mongo_app
```
