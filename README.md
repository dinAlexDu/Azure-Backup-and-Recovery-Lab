# Azure Backup and Recovery Lab

This repository contains a hands-on lab for configuring and recovering backups using **Azure Backup**.  
The goal of this lab is to demonstrate how to protect virtual machines in Azure using robust backup and recovery strategies. It walks through the process of setting up a **Recovery Services Vault**, configuring **Backup Policies**, performing VM backups, and restoring VMs from recovery points.

---


## 🛠️ Objectives

- **Learn how to configure Azure Backup for virtual machines.**
- **Protect virtual machines with customized backup policies.**
- **Restore virtual machines from recovery points to ensure business continuity.**
- **Test connectivity and validate VM functionality after restoration.**

---

## 📂 Repository Structure

```plaintext
Azure-Backup-and-Recovery-Lab/
├── images/              # Screenshots used in the documentation
├── README.md            # This file
└── ...
```

---

## ⚙️ Configuration Steps
1. Create a Resource Group
  - Name: BackupLabRG
  - Region: West Europe
2. Create a Storage Account
  - Type: Standard
  - Name: backupstorageaccttest
3. Set Up a Recovery Services Vault
  - Name: BackupVault
  - Associated Resource Group: BackupLabRG
4. Configure Backup Policy
  - Frequency: Daily backup at 11:00 PM.
  - Retention: 180 days.
5. Backup Virtual Machines
  - VMs: VM1-Backup, VM2-Backup
6. Restore a Virtual Machine
  - Type: Create a new VM.
  - Restored VM name: VM2-Restored.

---

## 🖼️ Screenshots

Below are the screenshots that illustrate the steps:

1. **Backup Items Overview**
   ![Backup Items Overview](images/backup-items.png)

2. **Trigger Backup Now**
   ![Trigger Backup Now](images/backup-now.png)

3. **Backup Policy Creation**
   ![Backup Policy Creation](images/backup-policy-creation-final.png)

4. **Recovery Vault Creation**
   ![Recovery Vault Creation](images/recovery-vault-creation.png)

5. **Resource Group Creation**
   ![Resource Group Creation](images/resource-group-creation.png)

6. **Restore Configuration**
   ![Restore Configuration](images/restore-configuration.png)

7. **Restored VM Overview**
   ![Restored VM Overview](images/restored-vm-overview.png)

8. **Restore Job Progress**
   ![Restore Job Progress](images/restore-job-progress.png)

9. **Select VMs for Backup**
   ![Select VMs for Backup](images/select-vms-backup.png)

10. **Storage Account Creation**
    ![Storage Account Creation](images/storage-account-creation.png)

11. **Restored VM with Public IP**
    ![VM2 Restored Overview with Public IP](images/vm2-restored-overview-with-public-ip.png)

12. **SSH Login to Restored VM**
    ![SSH Login to Restored VM](images/vm2-restored-ssh-login.png)

13. **VMs Overview**
    ![VMs Overview](images/vms-overview.png)

---

## 🛠️ Tools Used
  - Azure Portal: For VM backup and recovery configuration.
  - SSH: For connecting to restored VMs.
  - PowerShell: For command-line operations.

---

🚀 Next Steps
Explore more advanced scenarios, such as cross-region restore and backup encryption.
Test disaster recovery scenarios using Azure Site Recovery.
Learn how to automate backups using Azure PowerShell or Azure CLI.
