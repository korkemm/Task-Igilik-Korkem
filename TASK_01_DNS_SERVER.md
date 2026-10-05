# DNS Practical Workshop

**Student:** Igilik Korkem  
**Group:** SW 1-24  
**Operating System:** Windows 11  

## Workshop Goal

The goal of this workshop is to understand how the Domain Name System (DNS) works in practice.

During this workshop, I:

- identified my DNS server;
- checked DNS records;
- manually followed the DNS resolution path;
- investigated DNS cache and TTL;
- used an AI assistant to learn about DNS;
- tested AI-generated commands using real tools.

## Tools

The main tools used in this workshop were:

- Windows Command Prompt;
- `ipconfig`;
- `nslookup`;
- DNS cache commands;
- AI assistant.

## DNS

DNS stands for Domain Name System. It translates human-readable domain names such as `google.com` into IP addresses.

DNS can contain different types of records:

| Record | Purpose |
|---|---|
| A | IPv4 address |
| AAAA | IPv6 address |
| CNAME | Alias for another domain |
| MX | Mail server |
| NS | Authoritative name server |
| TXT | Text information |

## Tasks

### Task 1 — Who is my DNS server?

I identified the DNS server used by my computer and checked the IP address returned for `google.com`.

### Task 2 — Record Detective

I investigated A, MX, NS and TXT records for `gmail.com`.

### Task 3 — Be the Resolver

I manually followed the DNS hierarchy from the root server to the `.com` TLD and then to the authoritative server.

### Task 4 — Cache and TTL

I investigated DNS caching and observed how the TTL value changes over time.

### Task 5 — AI Fact-Checker

I asked an AI assistant DNS-related questions and tested the suggested commands in Windows.

## Conclusion

This workshop helped me understand that DNS is a distributed system rather than one central database. Different DNS servers are responsible for different parts of the domain hierarchy. I also learned that DNS caching and TTL values help improve performance, while tools such as `nslookup` allow users to investigate DNS information directly.
