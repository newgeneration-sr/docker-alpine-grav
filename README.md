# Grav

# Auto configuration parameters :

None

# Compose file exemple

```

version: '3.1'

services:

  grav:
    image: dotriver/grav
    environment:
    ports:
      - 8080:80
    volumes:
      - grav-data:/var/www/grav/
    networks:
      default:
    deploy:
      resources:
        limits:
          memory: 256M
      restart_policy:
        condition: on-failure
      mode: global

volumes:
    grav-data:

```