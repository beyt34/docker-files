## REDIS
docker run  --name redis  -p 6379:6379  -d  --restart unless-stopped redis


## MONGO
docker run  --name mongodb  -p 27017:27017  -d  --restart unless-stopped mongo


## SQL SERVER
docker run  --name sqldb  -e  "ACCEPT_EULA=Y"  -e  "SA_PASSWORD=Password12*"  -p 1433:1433  --restart unless-stopped  -d mcr.microsoft.com/mssql/server


## GRAYLOG
git clone https://github.com/beyt34/docker-files.git

cd graylog

docker-compose build

docker-compose up -d


## KIBANA
cd kibana

docker-compose build

docker-compose up -d
