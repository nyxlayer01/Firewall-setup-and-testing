# Step 8 — Summary: How a Firewall Filters Traffic

A firewall filters network traffic by inspecting packets and applying rules to decide whether to allow or block them.  
The filtering process can be based on several criteria:

1. **Source and Destination IP Address**  
   - Allows or blocks traffic from specific hosts or networks.

2. **Protocol Type**  
   - Rules can be set for TCP, UDP, ICMP, etc.

3. **Port Number**  
   - Controls access to specific services (e.g., allow port 22 for SSH, block port 23 for Telnet).

4. **Connection State (Stateful Firewalls)**  
   - Tracks if a packet is part of an existing connection or a new request.

5. **Direction of Traffic**  
   - **Inbound rules** control incoming connections.  
   - **Outbound rules** control outgoing connections.

By enforcing these rules, the firewall acts as a gatekeeper, ensuring only trusted and authorized traffic passes through while blocking unwanted or malicious connections.
