``` mermaid
sequenceDiagram
    Attacker->>+ Bot: The attacker sends a command to the bots which has them attack the server
    Bot->>+Control Server: all the bots go to the server to breach it
    Attacker->>+ Bot: After the breach the hacker then sends the attack signal to the bots which leads them to send a bunch of repeated requests to the server
    Bot-->>+ Webserver: It starts sending signals to overload the amount of requests it can receive.
    Webserver-->>-Control Server: This makes it so that way too many requests are coming in and so the server is no longer able to operate the request system which ends up shutting down processes and the site in general.
```
## Documentation
The attacker starts by sending a command the bots to attack the server. The bots then all go to the server and start attacking it. The bots then go breach the server. After it's breached the hacker the hacker sends an attack signal to the bots which has them send a bunch of repeated requests to the server. Afterwards the amounts of requests that the server can handle is reached which causes the request system to shut down which shuts down the web server and people can no longer use the site.