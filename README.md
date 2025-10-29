Karuta-docker
=====

Docker files related to deploy the backend + fileserver with MariaDB

#### How to use

Provided you have all the needed docker executables:

`docker compose up -d`

Will create all the containers and start the service.
A few folders will be created:

```
 ./
  + data    -- fileserver data will go here
  + db_data -- MariaDB files will be there
  + logs    -- Tomcat logs will end up here
```

If the location need to be somewhere else, modifying `docker-compose.yml` will be required

##### Note:
A proxy in front will be needed: Apache/Nginx

There is some configuration/architecture to be explored...