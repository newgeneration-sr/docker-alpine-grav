# Grav

# Auto configuration parameters :

None

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