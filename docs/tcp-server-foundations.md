# TCP Server Foundations

## Scenario

The coursework included a TCP server exercise based on a pharmaceutical-company ordering system.

The server was designed to accept connections from client systems representing pharmacy branches.

## Socket Workflow

The implementation followed the standard server-side TCP sequence:

```text
socket()
   ↓
bind()
   ↓
listen()
   ↓
accept()
   ↓
recv()
   ↓
process data
   ↓
send()
```

## Network Information

The program also displayed the connecting client's:

- IP address
- source port

This demonstrates the relationship between an application process and the network socket it uses.

## Analyst Relevance

A security analyst investigating a network service may need to understand:

- which process opened a listening socket
- what local port is exposed
- which remote host connected
- whether the connection is expected
- what data flow is occurring

### Example Investigation

```text
Unexpected network connection
        ↓
Identify local listening port
        ↓
Map port to process
        ↓
Review parent process / command line
        ↓
Identify remote IP and source port
        ↓
Determine whether communication is legitimate
```

The coursework did not implement a security monitoring system, but it provides the low-level networking foundation needed to understand that investigation flow.