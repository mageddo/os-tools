Verify simple UDP server for development porpuses

__Features__
* Setup a UDP server
* Print all received messages as plain text


__Using__

Download latest version and run it

```bash
jar udp-server-*.jar 
2018-05-27T14:58:29.247 - starting at 3333
```

Send some packets to the server

```bash
echo "it's `date`" > /dev/udp/127.0.0.1/3333
```

__Options__

```bash
jar udp-server-*.jar <port> <bufferSizeInBytes>
``` 

__Build from source__

```bash
./gradlew clean build && java -jar udp-server/build/libs/udp-server-*.jar 
```
