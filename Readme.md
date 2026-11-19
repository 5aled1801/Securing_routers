# Cisco Router Security Lab 🔐

A Cisco Packet Tracer networking lab focused on securing Cisco routers and controlling device access through password protection, privilege-level authentication, and remote management configuration.

## 📌 Project Overview

This project demonstrates fundamental Cisco router security configurations using Cisco Packet Tracer.

The lab focuses on protecting router access through console authentication, privileged EXEC mode security, local user authentication, and remote access configuration.

## 🖥️ Network Topology

The Packet Tracer topology includes:

- Cisco Routers
- Cisco 2960 Switch
- End Devices (PCs)
- Console connection for router configuration
- Ethernet connections for network communication

## 🔐 Security Configurations

### 1. Console Password Protection

Configure a password to protect physical console access.

```cisco
enable
configure terminal

line console 0
password YOUR_PASSWORD
login
exit
```

### 2. Privileged EXEC Mode Protection

Secure privileged mode using an encrypted enable secret.

```cisco
enable
configure terminal

enable secret YOUR_SECRET
```

### 3. Local User Authentication

Create local users for device authentication.

```cisco
username admin secret YOUR_SECRET
```

Enable local authentication on the console:

```cisco
line console 0
login local
```

### 4. Remote Access Configuration

Configure VTY lines for remote device access.

```cisco
line vty 0 4
password YOUR_PASSWORD
login
```

## 🛠️ Tools & Technologies

- Cisco Packet Tracer
- Cisco IOS CLI
- Networking Fundamentals
- Router Security
- Console Access
- Telnet
- Local Authentication

## 🎯 Learning Objectives

- Understand Cisco router access security.
- Configure console password authentication.
- Protect privileged EXEC mode.
- Create local user accounts.
- Configure VTY lines.
- Understand remote device management.

## 📂 Project Files

```text
cisco-router-security-lab/
│
├── securing-router.pkt
└── README.md
```

## 🚀 How to Run

1. Download or clone this repository.
2. Install Cisco Packet Tracer.
3. Open `securing-router.pkt`.
4. Select a router.
5. Open the CLI tab.
6. Review and test the security configurations.

## 🔒 Security Best Practices

- Prefer `enable secret` over `enable password`.
- Use `secret` when creating local user accounts.
- Use strong, unique passwords.
- Restrict remote management access to trusted networks.
- Never publish real passwords or authentication credentials.

## 👨‍💻 Author

Khaled Hassan

---

**Educational Project | Cisco Packet Tracer | Network Security**