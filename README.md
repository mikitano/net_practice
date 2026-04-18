_This project has been created as part of the 42 curriculum by mkitano_

# NetPractice

## 📌 Description

NetPractice is a project from the 42 curriculum designed to introduce the fundamental concepts of computer networking through hands-on exercises.

The main goal is to configure small-scale networks by correctly assigning IP addresses, subnet masks, and routing rules so that devices can communicate with each other.

Throughout the project, we learn how data travels across networks, how routers forward packets between different subnets, and how incorrect configurations (such as invalid gateways or mismatched masks) can break communication.

This project emphasizes **understanding over memorization**, requiring the student to analyze logs, debug routing issues, and reason about network behavior.

---

## ⚙️ Instructions

### ▶️ Running the project

1. Download and extract the project files.
2. Open the file:

```bash
index.html
```

3. The NetPractice interface will open in your browser.

---

### 🧪 How to use the interface

- Enter your login to save your configurations.
- Each level presents a **broken network**.
- Your goal is to fix it by modifying only the allowed fields.

Buttons available:

- **Check again** → verifies your solution
- **Get my config** → exports your configuration

---

### 📤 Submission

You must:

- Complete **10 levels**
- Export each configuration using **Get my config**
- Place the 10 files at the **root of your repository**

Example:

```bash
level1.json
level2.json
...
level10.json
```

---

### ⚠️ Evaluation rules

- You must solve **3 random levels during defense**
- External tools are **not allowed**
- A simple calculator (like `bc`) is allowed

---

## 🧠 Key Concepts Learned

This project covers essential networking fundamentals:

### 🌐 TCP/IP Addressing

- IP addresses identify devices in a network
- Each device must have a unique IP within its subnet

### 📏 Subnet Mask

- Defines the size of the network
- Determines which IPs belong to the same subnet
- Example:
  - `255.255.255.0` → /24
  - `255.255.255.224` → /27

---

### 🚪 Default Gateway

- Used when a host wants to communicate **outside its subnet**
- Must be the **IP of the router interface connected to the host**

---

### 🔀 Routing

- Hosts use:
  - direct delivery (same subnet)
  - routing table (other networks)

- If no route matches:
  - the **default route** is used

---

### 🖧 Routers

- Connect different networks
- Each interface belongs to a different subnet
- Responsible for forwarding packets

---

### 🔌 Switches

- Connect devices within the same network
- Forward packets to all ports (basic behavior in NetPractice)

---

### 📡 OSI Model (Simplified View)

- Focus mainly on:
  - Layer 2 → Data Link (switching)
  - Layer 3 → Network (IP + routing)

---

## 🧩 Problem-Solving Approach

A consistent method to solve exercises:

1. Identify subnets using the subnet mask
2. Check if hosts are in the same network
3. Verify IP validity (not network/broadcast)
4. Ensure correct gateway configuration
5. Validate routing tables
6. Use logs to debug issues

---

## 📚 Resources

### 📖 Learning Materials

- Practical Networking (YouTube) – _Networking Fundamentals playlist_ (about TCP/IP addressing, default gateway, routers and
  switches, OSI layers)
- Practical Networking (YouTube) – _Subnetting Mastery playlist_ (about subnet mask)
- TCP/IP addressing documentation

---

### 🤖 AI Usage

AI was used in this project for:

- Debugging configuration logs
- Structuring this README

All generated content was reviewed and fully understood before use.

---

### 📌 Concepts Covered

- TCP/IP addressing
- Subnet masks
- Default gateway
- Routing tables
- Routers and switches
- Packet forwarding
- OSI layers (basic understanding)

---

## 🚀 Final Notes

NetPractice is less about memorizing rules and more about:

👉 understanding how networks behave
👉 learning how to debug logically
👉 building intuition for routing

Mastering these concepts will make future networking and system projects significantly easier.
