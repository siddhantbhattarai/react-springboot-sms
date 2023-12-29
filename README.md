# react-springboot-sms
 This GitHub repository features a React-Spring Boot Student Management System, Dockerized for consistency. With MySQL as the database, the Jenkins pipeline automates CI/CD, deploying the app on Amazon EC2. Ideal for learning full-stack development and deployment practices.
# Deployment
```
git clone https://github.com/siddhantbhattarai/react-springboot-sms.git
```
```
cd react-springboot-sms
```
```
cd sms-client
docker build -t react-sms-client .
```
```
cd sms-server
docker-build -t springboot-sms-server .
```
```
docker-compose up -d
```

![Screenshot from 2023-12-29 09-13-26](https://github.com/siddhantbhattarai/react-springboot-sms/assets/94698034/1b361608-0554-4b22-82fd-c3be78f641f0)
![Screenshot from 2023-12-29 09-13-33](https://github.com/siddhantbhattarai/react-springboot-sms/assets/94698034/393fe50e-031d-4a4e-b2d9-05ebd10e81ae)
![Screenshot from 2023-12-29 09-13-46](https://github.com/siddhantbhattarai/react-springboot-sms/assets/94698034/c1fed067-7c57-4bc3-809b-8adbc47c1a6d)
![Screenshot from 2023-12-29 09-14-19](https://github.com/siddhantbhattarai/react-springboot-sms/assets/94698034/81df22ed-1643-47b0-beb5-0183221c5a8f)
