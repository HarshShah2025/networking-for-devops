# 🚀 What is Subnetting?

**Subnetting** = Dividing a big network (IP range) into smaller parts (subnets).

## 🔧 Why do we need subnetting?

- To organize networks (e.g., frontend, backend, DB all get different subnets)
- To save IP addresses (don’t waste unused IPs)
- To add security (block access between subnets if needed)
- To reduce traffic in each network

## 📦 Real Life Analogy:

Imagine an apartment building with 256 rooms (IPs).

Subnetting means:
➜ Grouping rooms by floor (subnet)  
➜ You can then control who can visit which floor.

## 📘 Example:

You have this network: `192.168.1.0/24`  
(That means: 256 IPs — from `192.168.1.0` to `192.168.1.255`)

Now you want 4 subnets:

You break it into 4 parts → each gets 64 IPs

Subnets become:

- `192.168.1.0/26`
- `192.168.1.64/26`
- `192.168.1.128/26`
- `192.168.1.192/26`

## 🧠 Quick Notes:

- `/24` = 256 IPs  
- `/26` = 64 IPs  
- `/28` = 16 IPs  
- `/30` = 4 IPs (used for point-to-point links)

## 📌 In DevOps:

You'll use subnetting in AWS VPCs, Kubernetes clusters, Cloud networking, etc.
