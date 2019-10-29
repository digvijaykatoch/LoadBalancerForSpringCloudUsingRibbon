# Load Balancer For Spring Cloud Using Ribbon

Working example of load balancing using spring cloud and ribbon. Modified as per my need. Heavily borrowed from official spring documentation.

## Installation

Run the user module separately first. It runs on port 8888.
Run the hi-user module next. If using IntelliJ, make sure to click "Run in Parallel" so that other instances of same server can be run on different ports.

```bash
From within IDE:
spring-boot:run for default 8090 port. 
OR
Set vm option as -Dserver.port=9092/9999. Then enter
spring-boot:run as Command-Line option.
From terminal:
mvn spring-boot:run
OR
SERVER_PORT=9999 mvn spring-boot:run
```

## Usage

Test if up:
```
http://localhost:8888
http://localhost:8090 or 9020 or 9999
```
See in action:
```
http://localhost:8888/hi?name=robinhood
```
Modify the above name parameter again and again to see different greetings.
