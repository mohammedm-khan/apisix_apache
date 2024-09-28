# Setting Up APISIX with Docker Compose and Keycloak latest zip Distribution powered by Quarkus

## Running Apache APISIX with Docker Compose on Ubuntu

To run **APISIX**, use the following Docker Compose command:

```bash
sudo docker-compose up -d

```

## Open Keycloak's configuration file and change the port
1. Download quarkus zip
2. Since apisix-dashboard runs on port 9000, keycloak management port we should modify.
3. Open keycloack.conf under conf directory with text editor.
4. Change Keycloak management port to 9007, by default it is 9000.
5. Run Keycloack authorization server in dev mode by follwing command. 
```
management.http.port=9007

sudo ./bin/kc.sh start-dev

```
