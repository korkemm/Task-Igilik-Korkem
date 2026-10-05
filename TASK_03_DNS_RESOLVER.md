# Task 3 — Be the Resolver

**Student:** Igilik Korkem  
**Group:** SW 1-24  

## Step 1 — Root Servers

I used:

```cmd
nslookup -type=NS .
```

One root server I selected was:

**`[ROOT SERVER NAME]`**

## Step 2 — Root to .com

I asked the root server which servers handle `.com`:

```cmd
nslookup -type=NS com. [ROOT SERVER]
```

One `.com` TLD server returned was:

**`[TLD SERVER NAME]`**

## Step 3 — TLD to Authoritative Server

I asked the `.com` TLD server which name servers are authoritative for `example.com`:

```cmd
nslookup -type=NS example.com [TLD SERVER]
```

Authoritative server:

**`[AUTHORITATIVE SERVER NAME]`**

## Step 4 — Final IP Address

Finally, I asked the authoritative server for the IP address:

```cmd
nslookup example.com [AUTHORITATIVE SERVER]
```

Final IP address:

**`[FINAL IP ADDRESS]`**

## Q1. DNS Resolution Path

My DNS resolution path was:

```text
My computer
     ↓
Root DNS Server
[ROOT SERVER]
     ↓
.com TLD Server
[TLD SERVER]
     ↓
Authoritative DNS Server
[AUTHORITATIVE SERVER]
     ↓
IP Address
[FINAL IP]
```

## Q2. How many servers did you ask?

I asked approximately **[NUMBER] DNS servers** before receiving the final answer.

## Q3. Why is there no single server that knows every domain?

There is no single server that knows every domain because the DNS system is distributed and hierarchical. Different DNS servers are responsible for different domains and parts of the DNS hierarchy.

## Q4. Bonus

The `dig +trace` command can show the DNS resolution process automatically, starting from the root and continuing through the TLD and authoritative servers.

The manual method helped me understand the individual steps of the same process.

## Screenshot / Drawing

My DNS resolution path drawing is included in the submission materials.

![Task 3 Screenshot](screenshots/task3.png)

## Conclusion

This task showed me how DNS resolution works from the root of the DNS hierarchy to the authoritative server that provides the final answer.
