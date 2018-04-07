# rspi3-mongodb
Mongodb docker image


$ docker run -d \
--name rpi3-mongodb3 \
--restart unless-stopped \
-v /data/db:/data/db \
-v /data/configdb:/data/configdb \
-p 27017:27017 \
-p 28017:28017 \
andresvidal/rpi3-mongodb3:latest \
mongod --auth
