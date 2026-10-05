# Task 5 — AI Fact-Checker

**Student:** Igilik Korkem  
**Group:** SW 1-24  

## Purpose

The purpose of this task was to verify information provided by an AI assistant using real commands.

## Prompt 1

I asked the AI assistant:

> "How do I view and clear the DNS cache on Windows? Give exact commands."

The AI suggested:

```cmd
ipconfig /displaydns
```

to display the DNS cache and:

```cmd
ipconfig /flushdns
```

to clear the DNS cache.

## Testing

I tested the commands in Windows Command Prompt.

### Command 1

```cmd
ipconfig /displaydns
```

The command worked successfully and displayed DNS cache information.

### Command 2

```cmd
ipconfig /flushdns
```

The command worked successfully and cleared the DNS resolver cache.

## Prompt 2

My second question was:

> "What is DNS over HTTPS?"

The AI explained that DNS over HTTPS (DoH) sends DNS queries through HTTPS, which encrypts the DNS traffic between the client and the DoH server.

## Verification

I did not accept the AI answer without testing it. I verified the commands directly in Windows Command Prompt.

## AI Verification Result

The commands provided by the AI worked successfully on my Windows computer.

The result of the test was:

**Verified successfully.**

## Screenshot

![Task 5 Screenshot](screenshots/task5.png)

## What the AI got wrong or unclear

The AI's commands were correct in my test. I verified them by running both commands in Windows Command Prompt and checking the actual output.

Therefore, instead of claiming that the AI was wrong, I can explain exactly how I verified the information:

1. I copied the suggested command.
2. I ran it in Windows Command Prompt.
3. The command executed successfully.
4. I compared the result with the AI's explanation.

## Conclusion

AI can be useful for learning DNS commands, but its answers should be tested with real tools. This task demonstrated that verification is important because an AI answer alone is not proof that a command will work on a particular system.
