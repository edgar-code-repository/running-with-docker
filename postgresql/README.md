POSTGRESQL
---------------------------------------------------------------------------------------------------------


**Se genera archivo Dockerfile para levantar PostgreSQL dentro de un contenedor:**

```

    FROM postgres:9.4

    ENV POSTGRES_USER=user
    ENV POSTGRES_PASSWORD=pass2020


```

**Se construye imagen a partir de archivo Dockerfile:**

```

    docker build -t postgres_server .

```

**Se levanta contenedor a partir de la imagen anterior:**

```

    docker run -d -p27017:27017 postgres_server

```

**Se levanta contenedor persistiendo datos en un volumen:**

```

    docker run -d -p 6432:5432 postgres_server

```

---------------------------------------------------------------------------------------------------------
