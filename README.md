![image](image.jpeg "image")

# Introduce

The server of the [День тижня](https://apps.lametric.com/apps/%D0%B4%D0%B5%D0%BD%D1%8C_%D1%82%D0%B8%D0%B6%D0%BD%D1%8F/11056) application for **LaMetric Time** device.


# Docker

Build image:
```bash
docker build --build-arg TIMEZONE=$(grep ^TIMEZONE .env | cut -d '=' -f2) -t weekday .
```

Run container:
```bash
docker run -d -p 80:80 --name weekday-app weekday
```
