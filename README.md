# Pirple Homework #1

In this step we needed to create a new endpoint hello that returned a message defined by us.

I refactored the code so the https server only start if the certificate files exists. They are not in the repository, so if you want to create them you should run this before starting the server:
```
mkdir hello
cd hello
openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem
```

Also I made the hello endpoint to return different messages depending if your're using http or https