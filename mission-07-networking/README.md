# Mission 7: How Computers Communicate

## Objective

Understand basic networking concepts, observe network connectivity and DNS information using Terminal, and explain what happens when a website is opened in a browser.

---

## Task 7.1: Explain Network Concepts

A computer network connects devices so they can exchange data and share resources.

| Concept | Explanation | Example |
|---|---|---|
| LAN (Local Area Network) | A network covering a small area, such as a home, lab or office. | Hostel Wi-Fi network |
| MAN (Metropolitan Area Network) | A network covering a city or a large campus area. | Network connecting buildings across a large campus |
| WAN (Wide Area Network) | A network covering large geographical areas. | Internet |
| DNS (Domain Name System) | Translates a domain name into an IP address. | Resolving google.com |
| Router | Connects networks and forwards data between them. | Wi-Fi router |
| Protocol | A set of rules that devices follow to communicate. | HTTP, HTTPS and TCP/IP |
| Packet Switching | Data is divided into smaller packets that travel across a network. | Sending a photo over the Internet |
| Client-Server | A client requests a service and a server provides it. | Browser requesting a webpage from a server |

---

## Task 7.2: Observe Network Information

I used macOS Terminal to test network connectivity and perform a DNS lookup.

### 1. Connectivity test

Command used:

```bash
ping -c 4 example.com
```

Explanation:

- `ping` sends test packets to another computer or server.
- `-c` specifies the number of packets to send.
- `4` tells the command to send four packets.
- `example.com` is the destination domain.

A connectivity test helps check whether a computer can communicate with another device or server over a network. It can also display response time and packet loss.

### 2. DNS lookup

Command used:

```bash
nslookup example.com
```

Explanation:

A DNS lookup displays information about a domain name, including its associated IP address and the DNS server that provided the response.

### 3. Answers to the assignment questions

**What does a connectivity test help you check?**

A connectivity test checks whether my computer can communicate with another device or server over a network. It can also show response time and packet loss.

**What information does a DNS lookup display?**

A DNS lookup displays information about a domain name, including its associated IP address and the DNS server that provided the response.

**What is the role of DNS when you enter a website name in a browser?**

DNS translates a website's domain name into an IP address so that the browser can locate the correct server.

### Network observations

- Connectivity test: [Record whether packets were received or timed out.]
- DNS lookup: [Record whether an IP address was returned.]
- Tools used: Terminal, ping and nslookup.

**Privacy note:** Personal IP addresses, Wi-Fi names and other identifying network information have not been included.

---

## Task 7.3: What Happens When You Open a Website?

The following steps explain what happens when I enter google.com into a browser.

1. **User enters a website address:** I type google.com into my browser. The browser acts as the client and starts requesting the website.

2. **DNS lookup:** The browser needs the server's IP address. DNS translates the domain name into its corresponding IP address.

3. **Network connection:** My computer sends data through the local network and router towards the destination server. Routers forward packets between networks.

4. **Client sends request:** The browser sends an HTTP or HTTPS request to the server using network protocols such as TCP/IP.

5. **Server sends response:** The server receives the request, processes it and sends a response containing the requested webpage data.

6. **Browser displays the website:** The browser receives the response, processes the HTML, CSS and JavaScript, and displays the webpage to the user.

### Basic communication flow

Browser → DNS → Router/Network → Server → Response → Browser

DNS finds the IP address, while the server provides the requested webpage data.

---

## What I Learned

Through this mission, I learned:

1. The difference between LAN, MAN and WAN.
2. How DNS translates domain names into IP addresses.
3. The role of routers in forwarding network data.
4. How protocols help devices communicate.
5. How packet switching works.
6. The difference between a client and a server.
7. How to test network connectivity using ping.
8. How to perform DNS lookups using nslookup.
9. What happens behind the scenes when a website is opened.

## Difficulties Faced

- Initially, I needed to understand the purpose of command-line flags such as `-c` in the ping command.
- I learned the difference between a connectivity test and a DNS lookup.
- Understanding how DNS, routers, clients and servers work together required connecting several networking concepts.

## Tools and Commands Used

| Tool / Command | Purpose |
|---|---|
| macOS Terminal | Execute networking commands |
| `ping -c 4 example.com` | Test network connectivity |
| `nslookup example.com` | Perform a DNS lookup |

## Conclusion

This mission helped me understand how computers communicate over networks and how websites work behind the scenes. I also gained practical experience using Terminal commands to observe network connectivity and DNS information.

I now have a better understanding of the networking concepts that make Internet communication possible.