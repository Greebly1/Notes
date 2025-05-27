An [[Active Directory]] feature that allows extra control over user accounts and computers

# How to use
Group Policy is configured and managed through the [[Group Policy Management]] utility
- Make sure to update users group policy using [[gpupdate]]

# How to view
To view a local machine and user's group policy use [[gpresult]]

# Local Group Policy
Group policy can also be used in local machines on [[Local Windows Account]]s not just in an active directory domain.
To do this use [[Local Group Policy Editor]]

# Features
### 🔒 Security & Access Control
- **Password policies** (length, complexity, expiration)
- **Account lockout thresholds**
- **[[UAC]] settings** 
- **Configure [[Windows Defender]]**
- **Configure #Firewalls**

### 🖥️ Desktop & User Environment
- **Set desktop backgrounds / wallpapers**
- **[[Redirect folders]]** (e.g., Documents, Desktop to a network share)
- **Map network drives automatically**
- **Deploy printers**
- **Hide specific drives in File Explorer**

### 🔧 System Management
- **Deploy software via [[MSI Package]]s**
- **Control Windows Updates (WSUS settings)**
- **Set scripts to run at logon/logoff or startup/shutdown**
- **Disable removable storage (e.g., USB drives)**
- **Prevent automatic restarts after updates**