# Mission 07: How Computers Communicate

## 1. Mission Title
**Mission 07: How Computers Communicate**

## 2. Task / Objective
The objective of this mission is to understand basic computer networking concepts, learn how devices communicate over networks, practise networking commands in Terminal, and understand what happens when a website is opened in a browser.

## 3. Work Completed
- Learned the differences between LAN, MAN and WAN.
- Understood DNS, routers, protocols and packet switching.
- Learned the client-server communication model.
- Used the `ping` command to test network connectivity.
- Used `nslookup` to perform DNS lookups.
- Studied the steps involved in opening a website such as google.com.
- Documented the networking concepts and commands.

## 4. Commands / Tools Used

**Commands used:**

```bash
ping -c 4 example.com
```

Used to send four test packets to example.com and observe network connectivity and response times.

```bash
nslookup example.com
```

Used to find DNS information and the IP address associated with a domain name.

**Tools used:**
- macOS Terminal
- `ping`
- `nslookup`

## 5. My Understanding

**LAN (Local Area Network):** A network that covers a small area, such as a home, laboratory or office.

**MAN (Metropolitan Area Network):** A network that covers a city or a large campus area.

**WAN (Wide Area Network):** A network that covers large geographical areas. The Internet is an example.

**DNS (Domain Name System):** Translates human-readable domain names into IP addresses.

**Router:** Connects different networks and forwards data between them.

**Protocol:** A set of rules that devices follow to communicate. Examples include HTTP, HTTPS and TCP/IP.

**Packet Switching:** A method in which data is divided into smaller packets before being transmitted across a network.

**Client-Server Model:** A system in which a client requests a service and a server responds to that request.

### What happens when I open google.com?

1. I enter `google.com` into my browser.
2. DNS translates the domain name into an IP address.
3. My computer connects through the local network and router.
4. The browser sends an HTTP or HTTPS request to the server.
5. The server processes the request and sends a response.
6. The browser processes the webpage data and displays the website.

**Basic communication flow:**

Browser → DNS → Router / Network → Server → Response → Browser

## 6. Difficulties Faced
- Understanding the differences between LAN, MAN and WAN.
- Learning how DNS translates domain names into IP addresses.
- Understanding the purpose of the `-c` option in the ping command.
- Connecting the roles of DNS, routers, clients and servers into one complete process.

## 7. How I Resolved Them
- Studied each networking concept with simple real-world examples.
- Practised `ping` and `nslookup` in Terminal.
- Observed the command outputs to understand their purpose.
- Broke the process of opening a website into smaller steps to understand how the different components work together.

## 8. Evidence / Files
- `mission-07-networking/README.md`
- `evidence/mission-07-networking/network-commands.png`

The screenshot contains the networking commands and their outputs.

## 9. Commit Details
- **Branch:** `update-about`
- **Commit message:** `Complete Mission 7: Networking`
- **Commit hash:** `0cb518e`
- **Remote branch:** `origin/update-about`

The mission documentation and networking evidence were added to the project repository.