# Task-4-Cyber-security-firewall
Cyber Security Internship - Task 4: Setup and Use a Firewall on Windows

### Objective
Configure and test basic Windows Firewall rules to allow or block network traffic.

### Tools Used
- Windows Defender Firewall with Advanced Security
- Command Prompt
- PowerShell

### Task Performed

#### 1. Blocked Telnet Port 23
Created an inbound firewall rule:

- Rule Name: Block Telnet Port 23
- Protocol: TCP
- Local Port: 23
- Action: Block
- Profiles: Domain, Private, Public

#### 2. Tested Port 23
Used the following PowerShell command:

```powershell
Test-NetConnection localhost -Port 23
```

Result:

```text
TcpTestSucceeded : False
```
