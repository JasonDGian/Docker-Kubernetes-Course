# 📌 MySQL server.
This container configuration allows the use of a MySQL databaser server as if it were pre-insalled in the local system.
   
```docker
docker run --name myServer -p 3306:3306 -e MYSQL_ROOT_PASSWORD=1234 -d mysql
```
   
This sample command will start a MySQL server instance with these details: 
- **Container name:**  "myServer.
- **Listening port on host:**  3306.
- **Listening port on container:**  3306.
- **MYSQL_ROOT_PASSWORD environtment variable:**  1234
- **Terminal mode:** Detached.
- **Image:** MySQL.
   
https://hub.docker.com/r/mysql/mysql-server

## 🔹 Connecting Dbeaver to MySqL.

1. Open dBeaver and click on new connection.
2. Selecy MySQL.
3. Enter the ROOT password ("1234" if you ran the command as is in the above section).
4. Set the port as 3306
5. Name the database. **Only if attaching to a specific known database**
6. Click on `Test Connection`.
    If "Public Key Retreival is not allowed" error is shown read below.
7. If the connection is confirmed then click on Accept _et voilá_.


### ▫️ Public Key Retrieval is not allowed.
This errors shows up when try using the option `useSSL=false`. If that does not work use the option `useSSL=false&allowPublicKeyRetrieval=true`.
This is not a secure thing to do in normal applications but in this case we are trying to connect from our localhost to a docker container.
![imagen](https://github.com/user-attachments/assets/7ff815b8-a401-4435-a555-f4dc2fe7e449)
![imagen](https://github.com/user-attachments/assets/1a83911d-f9d4-4baa-9fbb-0762954e7ff3)

