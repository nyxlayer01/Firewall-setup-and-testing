# Firewall Setup and Testing (UFW on Linux)

## Objective
Configure and test basic firewall rules using UFW to allow and block specific network traffic.

## Step 1 — Check Current Firewall Status
```bash
sudo ufw status
```
Expected Output: `Status: inactive` or `Status: active`

## Step 2 — Enable UFW
```bash
sudo ufw enable
```
Expected Output: `Firewall is active and enabled on system startup.`

## Step 3 — Block Port 23 (Telnet)
```bash
sudo ufw deny 23/tcp
```
Expected Output: `Rule added`

## Step 4 — Test Telnet Connection 

Test:
```bash
telnet localhost 23
```
Expected: It will refuse to connect.

## Step 5 — Allow SSH (Port 22)
```bash
sudo ufw allow 22/tcp
```
Expected Output: `Rule added`

## Step 6 — Test SSH Connection

Test:
```bash
ssh localhost
```
Expected: Successful SSH login prompt

## Step 7 — Remove Port 23 Block Rule
```bash
sudo ufw delete deny 23/tcp
```
Expected Output: `Rule deleted`

## Step 8 — View Final Rules

```bash
sudo ufw status verbose
```
Expected: Only allowed ports listed (e.g., `22/tcp ALLOW`)

## Summary
- UFW was enabled.
- Port 23 was blocked and tested.
- SSH was allowed for secure access.
- Telnet block rule was removed, restoring the original state.
