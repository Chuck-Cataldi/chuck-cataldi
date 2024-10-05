...
sequenceDiagram
    participant A as Attacker
    participant B as Botnet (Zombies)
    participant C as Target Web Server
    participant D as ISP
    participant E as Firewall

    A->>B: Send attack command
    B->>C: Send flood of requests
    C->>C: Handle incoming requests
    C--)D: Notify unusual traffic
    D->>E: Activate DDoS protection
    E->>C: Start filtering traffic
    B->>C: Continue sending requests
    E-->>C: Allow legitimate traffic
    C->>C: Stabilize performance
    C--)D: Analysis post-attack
...
