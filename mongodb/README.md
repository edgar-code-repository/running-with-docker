MONGODB
---------------------------------------------------------------------------------------------------------

**Se baja imagen de MongoDB:**

```

    docker pull mongo:4

```

**Se levanta contenedor a partir de la imagen anterior:**

```

    docker run -d -p27017:27017 mongo:4

```

**Se levanta contenedor persistiendo datos en un volumen:**

```

    docker run -v /my/own/dir:/data/db -d -p27017:27017 mongo:4

```

**Se accede a Mongo via consola:**

```

    sudo docker exec -it <container_id> mongo    

```

---------------------------------------------------------------------------------------------------------