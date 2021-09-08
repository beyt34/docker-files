------------
REDIS
------------
docker run --name redis -p 6379:6379 -d --restart unless-stopped redis

------------
MONGO
------------
docker run --name mongodb -p 27017:27017 -d --restart unless-stopped mongo

------------
SQL SERVER
------------
docker run --name sqldb -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=Password12*" -p 1433:1433 --restart unless-stopped -d mcr.microsoft.com/mssql/server


------------
cd C:\Projects\ME\docker-files

cd C:\Projects\ME\docker-files\graylog

cd C:\Projects\ME\docker-files\kibana

docker-compose up -d

