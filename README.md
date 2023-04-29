# Run MQTT Broker with Docker Compose

## Run
```bash
docker-compose up -d
```

## MQTT Client Account
- username : admin
- password : admin

## Generate Password File
```bash
mosquitto_passwd -U ./password/password_file
```

## Example Publish and Subscribe MQTT
### Subscribe
```bash
mosquitto_sub -h <URL> -p <MQTT PORT> -t <TOPIC> -u <USERNAME> -P <PASSWORD>    
```

### Publish
```bash
mosquitto_pub -h <URL> -p <MQTT PORT> -t <TOPIC> -u <USERNAME> -P <PASSWORD> -m <MESSAGE>
```