# 🎫 Help Desk Ticket Scenarios
## IT Help Desk & Active Directory Lab

This section documents realistic Tier 1 / Tier 2 IT support tickets handled within the hybrid Active Directory lab environment.

Each ticket demonstrates structured troubleshooting, documentation, and resolution workflows similar to enterprise IT support environments.

---

# 🎫 Ticket #001 – Account Lockout

**Priority:** High  
**Department:** IT Support  

### Issue
User reports inability to log into domain-joined workstation.

### Impact
User cannot access domain resources or company applications.

### Troubleshooting Steps
1. Checked Active Directory Users & Computers.
2. Identified account was locked due to failed login attempts.
3. Reviewed account lockout policy.
4. Unlocked user account.
5. Verified successful login on client machine.

### Root Cause
Multiple incorrect password attempts triggered domain lockout policy.

### Resolution
Account unlocked and user instructed on password best practices.

**Status:** Closed

---

# 🎫 Ticket #002 – Password Reset Request

**Priority:** Medium  
**Department:** IT Support  

### Issue
User forgot password and requested reset.

### Impact
User unable to authenticate to domain.

### Troubleshooting Steps
1. Verified user identity.
2. Reset password in Active Directory.
3. Enabled "User must change password at next login".
4. Confirmed successful login.

### Root Cause
User password expired.

### Resolution
Password reset and policy enforced.

**Status:** Closed

---

# 🎫 Ticket #003 – Add User to Security Group

**Priority:** Medium  
**Department:** IT Support  

### Issue
User requires access to shared department drive.

### Impact
User unable to access required resources.

### Troubleshooting Steps
1. Verified existing group membership.
2. Identified missing security group.
3. Added user to appropriate AD security group.
4. Forced policy update (`gpupdate /force`).
5. Confirmed folder access.

### Root Cause
User not assigned correct group-based permissions.

### Resolution
Access granted using role-based access control (RBAC).

**Status:** Closed

---

# 🎫 Ticket #004 – Domain Join Failure

**Priority:** High  
**Department:** IT Support  

### Issue
New workstation unable to join domain.

### Impact
Device cannot authenticate to domain.

### Troubleshooting Steps
1. Verified DNS server configuration.
2. Tested connectivity to Domain Controller.
3. Confirmed domain credentials.
4. Re-attempted domain join.
5. Restarted workstation.

### Root Cause
Incorrect DNS server configuration.

### Resolution
Updated DNS settings to point to Domain Controller.

**Status:** Closed

---

# 🎫 Ticket #005 – RDP Access Issue

**Priority:** Medium  
**Department:** IT Support  

### Issue
User unable to remote into server.

### Impact
User unable to perform remote administrative tasks.

### Troubleshooting Steps
1. Verified RDP enabled on server.
2. Checked firewall rules.
3. Confirmed user added to Remote Desktop Users group.
4. Tested RDP connection.

### Root Cause
User missing RDP permissions.

### Resolution
User added to proper security group and access verified.

**Status:** Closed

---

# 🎫 Ticket #006 – DNS Resolution Failure

**Priority:** High  
**Department:** IT Support  

### Issue
User unable to access internal domain resources.

### Impact
Network resources unavailable.

### Troubleshooting Steps
1. Ran `ipconfig /all`.
2. Identified incorrect DNS server.
3. Updated DNS configuration.
4. Tested resolution using `nslookup`.
5. Confirmed connectivity restored.

### Root Cause
Incorrect DNS configuration.

### Resolution
Updated client DNS settings to correct domain controller IP.

**Status:** Closed

---

# 🎫 Ticket #007 – Account Deprovisioning

**Priority:** Medium  
**Department:** IT Support  

### Issue
Employee termination – remove system access.

### Impact
Security risk if account remains active.

### Troubleshooting Steps
1. Disabled user account in Active Directory.
2. Removed from all security groups.
3. Documented deprovisioning actions.
4. Confirmed account disabled.

### Root Cause
User offboarding process initiated.

### Resolution
Account securely disabled and access removed.

**Status:** Closed

---

## 🎥 Tickets Demonstrated in Video

For the 3-minute walkthrough, the following scenarios are demonstrated:

- Ticket #001 – Account Lockout
- Ticket #003 – Add User to Security Group

These examples showcase:
- Active Directory troubleshooting
- Group-based access control
- Ticket lifecycle documentation
- End-to-end resolution workflow
