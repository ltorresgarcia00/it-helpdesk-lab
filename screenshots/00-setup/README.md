## 🐧 Ubuntu VM Setup (UTM)

This section documents the initial setup of the Ubuntu virtual machine used as the foundation for the IT Help Desk lab. The VM is hosted using **UTM (QEMU)** on an Apple Silicon Mac and will later be used to deploy a ticketing system and supporting services.

---

### 🛠️ Environment Details
- **Host OS:** macOS (Apple Silicon)
- **Virtualization:** UTM (QEMU ARM64)
- **Guest OS:** Ubuntu 25.10
- **Network Mode:** Shared (NAT)
- **Memory:** 6 GB RAM
- **Disk:** ~20 GB virtual disk

---

### 🔄 System Update & Preparation
After installation, the system was fully updated to ensure all packages and security patches were current.

```bash
sudo apt update && sudo apt upgrade -y
