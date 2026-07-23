# Mission 08 - Following the Path of Network Traffic

## Objective
Learn how data moves across a network and why understanding that path helps SOC analysts investigate suspicious activity.

---

## Lesson Summary

When one computer communicates with another, the data doesn't travel all at once. It's broken into packets that travel across the network before being reassembled at the destination.

Think of it like mailing a large book:
- Split the book into several envelopes (packets).
- Each envelope contains sender and recipient information.
- The envelopes travel through the network.
- The receiving computer puts them back together.

Key Terms:
- Source IP – The device sending the traffic.
- Destination IP – The device receiving the traffic.
- Protocol – The communication method (TCP, UDP, ICMP).
- Port – Identifies the service or application being used.
- Packet – A small piece of data traveling across the network.

---

## Scenario

You observe the following network connection:

- Source IP: 192.168.1.25
- Destination IP: 142.250.190.78
- Protocol: TCP
- Destination Port: 443
- Time: 2:13 AM

---

## Questions & Answers

### 1. What information can you learn from the source and destination IP addresses?

The source IP tells me which device initiated the communication, while the destination IP identifies the server or device receiving the traffic. This helps determine where the traffic originated and where it was going.

---

### 2. Why is port 443 important?

Port 443 is used for HTTPS traffic, allowing secure and encrypted communication between devices and websites.

---

### 3. Does traffic at 2:13 AM automatically mean something malicious happened?

No. Activity during unusual hours is not enough to determine malicious behavior. It could be a scheduled task, software update, backup, or legitimate user activity. Additional evidence is required before making conclusions.

---

### 4. What additional information would you want before deciding whether this traffic is suspicious?

- Who owns the source device.
- Whether the user normally works at that time.
- The reputation of the destination IP.
- Whether similar connections occur regularly.
- Other related events before or after the connection.
- Whether the amount of traffic is normal.

---

## What I Learned

I learned that network traffic should always be investigated using evidence instead of assumptions. Understanding IP addresses, ports, protocols, and timing helps SOC analysts determine whether activity is normal or requires further investigation.
