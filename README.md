![docker build automated](https://img.shields.io/docker/cloud/automated/dotriver/grav)
![docker build status](https://img.shields.io/docker/cloud/build/dotriver/grav)
![docker build status](https://img.shields.io/docker/pulls/dotriver/grav)

# Grav

Grav documentation (here)[https://learn.getgrav.org/]

# Auto configuration parameters :

```
- GRAV_VERSION : 1.7.13
```

# Compose file exemple

```

version: '3'
services:
  grav:
    image: dotriver/grav
    ports:
      - 8080:80
    volumes:
      - grav-data:/var/www/grav/
    networks:
      default:
volumes:
    grav-data:

```
