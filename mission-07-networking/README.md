# Mission 7 — How computers communicate

## 1. Mission title

Mission 7 — How computers communicate

## 2. Task / objective

Explain basic network types and concepts, observe connectivity and DNS information, and describe what happens when a website opens.

## 3. Work completed

### Task 7.1 — Network concepts

| Concept | Explanation | Example |
|---|---|---|
| LAN | A local area network connects devices over a small area, such as a home, lab or office | Devices sharing a home router |
| MAN | A metropolitan area network covers a city or a large campus area | A university campus network linking several buildings |
| WAN | A wide area network covers large geographical areas and often connects multiple smaller networks | The internet |
| DNS | Domain Name System translates a domain name into network addresses used to locate a server | Mapping `example.com` to an address |
| Router | A networking device that forwards data between networks and chooses suitable paths | A home router connecting a laptop to the internet |
| Protocol | A set of rules that devices follow to communicate consistently | HTTP or HTTPS governs web requests and responses |
| Packet switching | Information is divided into packets that can travel across network links and arrive for reassembly | A web response carried in many packets |
| Client-server | A client requests a service and a server processes and returns it | A browser requesting a webpage from a web server |

### Task 7.2 — Observe network information

The `ping` connectivity test to `example.com` sent three packets and received three replies. It reported 0% packet loss, so the network route and the example host were reachable at the time of the test. The round-trip observations varied and ranged from about 127 ms to 301 ms.

The DNS lookup returned the addresses `172.66.147.243` and `104.20.23.154` for `example.com`. A DNS lookup lists network addresses associated with a domain name. DNS therefore lets a person enter a familiar name in a browser while the browser obtains addresses it can use to locate the server.

No personal IP address, Wi-Fi name or other private network information was published.

### Task 7.3 — What happens when a website opens?

1. The user enters a website address in a browser, and the browser acts as the client.
2. The browser asks DNS to translate the domain name into an IP address.
3. The browser uses a network protocol, usually HTTPS, to prepare a request for the server.
4. The request travels through the computer's network interface and local router toward the destination network.
5. Routers and switches forward the request's packets across the network.
6. The web server receives the request, processes it and sends a response containing the webpage or an error.
7. The browser receives the response, verifies and assembles the data, and displays the webpage to the user.

## 4. Commands / tools used

- `ping -c 3 example.com` — tested public example-domain connectivity and packet loss.
- `dig +short example.com` — looked up DNS addresses for the example domain.
- Browser — represented the client in the website-opening explanation.

## 5. My understanding

A network allows devices to exchange information using shared rules. DNS turns names into addresses, routers move packets between networks, and the client-server model separates the requester from the service provider. The browser, DNS, local network and server work together whenever a webpage opens.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- `evidence/mission-07-networking.txt`
- Privacy-safe connectivity and DNS observations

## 9. Commit details

- Commit message: `Explain networking concepts and website communication`
- Status: Committed and pushed successfully to `main`.
