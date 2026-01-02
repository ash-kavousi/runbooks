# IPv4 & IPv6 Fundamentals

An **IP address** is a unique identifier assigned to each device connected to a network. A good analogy is a **postal address**: it helps data reach the correct destination.

## IPv4 (Internet Protocol version 4)

**IPv4** uses a **32-bit** address. It is written in **dotted-decimal** format, made of four numbers separated by dots:

`192.168.10.25`

Each of the four parts is called an **octet** because it contains **8 bits**. With 8 bits, you can represent 256 values (0–255), so **255** is the largest value possible in one octet.

With 32 bits total, IPv4 provides about **2^32 ≈ 4.3 billion** unique addresses.

## Network and host portions (subnet masks)

An IPv4 address can be thought of as two parts: a **network** part and a **host** part. The **subnet mask** defines where that split happens (for example `255.255.255.0`).

This split helps devices and routers determine whether a destination is on the local network or must be reached through routing.

## Classful addressing (historical background)

In the early days of IPv4, addresses were grouped into fixed “classes” to simplify allocation. This is called **classful addressing**. It is important historically, but modern networks use classless addressing.

- **Class A:** 1.0.0.0 – 126.255.255.255 (default mask `255.0.0.0`)
- **Class B:** 128.0.0.0 – 191.255.255.255 (default mask `255.255.0.0`)
- **Class C:** 192.0.0.0 – 223.255.255.255 (default mask `255.255.255.0`)
- **Class D:** multicast (224.0.0.0 – 239.255.255.255)
- **Class E:** experimental/reserved (240.0.0.0 – 255.255.255.255)

With default masks, the maximum hosts per network were typically:

- Class A: 16,777,214  
- Class B: 65,534  
- Class C: 254  

## Private vs public IPv4

As the internet grew, the IPv4 pool started to run out. To extend IPv4, special ranges were reserved as **private IP addresses**. Private addresses can be reused across different networks because they only need to be unique inside a local network.

The trade-off is that private IP addresses are **not routable on the public internet**. For internet access, private addresses typically use NAT (explained below).

Private ranges:

- `10.0.0.0` – `10.255.255.255`
- `172.16.0.0` – `172.31.255.255`
- `192.168.0.0` – `192.168.255.255`

A **public IP address** is globally unique and routable on the internet, usually assigned by your ISP.

## NAT (Network Address Translation)

**NAT** allows many private devices to share one public IP address. A router translates internal private addresses to a public address when traffic goes out to the internet, and then maps responses back to the correct internal device.

NAT helps conserve public IPv4 addresses and reduces direct exposure of internal addressing, but it does not replace proper firewall rules and security controls.

## Subnetting

**Subnetting** is the process of dividing a larger network into smaller networks (subnets). It helps allocate IP addresses efficiently, reduces unnecessary broadcast traffic, improves performance, and supports segmentation for better security and management.

## Classless addressing: VLSM and CIDR

Classful addressing wasted many IP addresses because it forced fixed network sizes. In modern networks, **classless addressing** is used, where the subnet mask (prefix length) can be chosen to fit the required number of hosts and subnets.

- **VLSM (Variable Length Subnet Masking):** use different subnet sizes within the same overall network.
- **CIDR (Classless Inter-Domain Routing):** uses prefix notation like `192.168.10.0/24` for allocation and routing.

## IPv6 (Internet Protocol version 6)

**IPv6** was designed to solve IPv4 exhaustion and improve scalability. IPv6 uses a **128-bit** address space, providing an extremely large number of unique addresses (**2^128**).

IPv6 addresses are written in hexadecimal and separated by colons. Example:

`2001:0db8:85a3:0000:0000:8a2e:0370:7334`

IPv6 is written as eight groups (often called **hextets**). Each hextet represents 16 bits and ranges from `0000` to `FFFF` (where `FFFF` equals 65,535 in decimal).

## IPv4 vs IPv6 (summary)

- **Address size:** IPv4 is 32-bit; IPv6 is 128-bit.
- **Format:** IPv4 is dotted-decimal; IPv6 is colon-separated hexadecimal.
- **Address space:** IPv6 provides vastly more addresses than IPv4.
- **NAT:** common in IPv4; less necessary in IPv6 (though still used in some cases).
- **Operations:** IPv6 supports cleaner large-scale allocation and routing.

## Wrap-up

IPv4 is still widely used, but limited. Private addressing and NAT helped IPv4 scale, while IPv6 provides the long-term solution with a huge address space. Many networks run both during the transition (**dual-stack**).




