# docker-realms-wiki

This is realms-wiki in docker.

### Run command

```
docker run --name wiki \
-v /home/luna/wiki:/data/config \
-v /home/luna/wiki:/data/db/ \
-v /home/luna/wiki:/data/repo/ \
-p 5000:5000 \
-d kee7a/realms-wiki:latest
```

### Exposed ports: 

```
5000 - web server port
```

### Exposed volumes 

```
/data/config - settings json file
/data/db - database file
/data/repo - user repo filled with wiki files
```

### Expected Files

```
data/config/realms-wiki.json

data/db/wiki.db

data/repo/
```

