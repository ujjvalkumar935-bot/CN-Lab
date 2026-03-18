# CN-Lab

🎯 Objective

- To understand the working of CS/CD protocol
- To simulate data transmission using a hub-based network
- To observe collision detection and retransmission

---
.

Working:

- Carrier Sense: Device checks if the channel is free
- Multiple Access: Multiple devices can send data
- Collision Detection: If two devices send data at the same time, collision occurs
- After collision, devices wait for a random time and retransmit

In this experiment, a Hub is used, which increases chances of collision because it broadcasts data to all devices.


⚙️ Step-by-Step Procedure

1. Open Cisco Packet Tracer
2. Add 1 Hub in the center
3. Add 4 PCs (PC0, PC1, PC2, PC3)
4. Connect all PCs to the hub using Copper Straight-Through cables
5. Assign IP addresses:
   - PC0 → 192.168.1.1
   - PC1 → 192.168.1.2
   - PC2 → 192.168.1.3
   - PC3 → 192.168.1.4
6. Switch to Simulation Mode
7. Send data (Simple PDU) between multiple PCs at the same time
8. Observe collision in the simulation panel

---

💻 Configuration Commands

ping 192.168.1.2
ping 192.168.1.3
ping 192.168.1.4

---

📊 Observations / Results

- Collisions occur when multiple PCs transmit simultaneously
- Hub broadcasts data to all connected devices
- Some packets initially fail due to collision
- Retransmission happens after random delay
- Successful communication is achieved after retransmission

"Simulation Result" (result.png)

«📌 Upload simulation/collision screenshot as "result.png"»

---

✅ Conclusion

The experiment successfully demonstrates the working of CS/CD protocol in a hub-based network.
It shows that:

- Collisions occur in shared medium networks
- CS/CD helps detect and recover from collisions
- Efficiency decreases as number of devices increases

---
