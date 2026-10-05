# Task 4 — Cache and TTL

**Student:** Igilik Korkem  
**Group:** SW 1-24  

## Step 1 — First Lookup

I used:

```cmd
nslookup -debug google.com
```

The first TTL value I observed was:

**`[FIRST TTL]`**

## Step 2 — Second Lookup

After waiting approximately 5–10 seconds, I ran the command again:

```cmd
nslookup -debug google.com
```

The second TTL value was:

**`[SECOND TTL]`**

### Q1. What happened to the TTL?

The TTL value decreased after waiting because the cached DNS record had less time remaining before it expired.

## Step 3 — DNS Cache

I checked the Windows DNS cache using:

```cmd
ipconfig /displaydns
```

This command displayed DNS information currently stored in the local DNS cache.

## Step 4 — Flush DNS Cache

I cleared the cache using:

```cmd
ipconfig /flushdns
```

After flushing the cache, I performed the lookup again:

```cmd
nslookup google.com
```

### Q2. What changed after flushing the cache?

After flushing the DNS cache, previously cached DNS information was removed from my computer. A new DNS lookup was required.

### Q3. Why do websites set a short TTL before moving to a new server?

A short TTL allows DNS information to expire faster. This helps users receive the new server address sooner after a website changes its server or IP address.

### Q4. Screenshot

![Task 4 Screenshot](screenshots/task4.png)

## Conclusion

DNS caching improves performance because repeated queries can use stored information. TTL controls how long DNS information remains valid in the cache. Flushing the cache removes stored DNS information and forces new lookups.
