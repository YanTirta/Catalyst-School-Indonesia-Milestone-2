# **Reproducing the Snapshot**
Auditing the Snapshot is simply reproducing a snapshot directly from blockchain data and comparing it with the officially published snapshot data.

### **Getting the Registration Deadline slot number**

<img width="670" alt="Reproducing the snapshot 1" src="https://github.com/user-attachments/assets/1a3bae6e-2b2a-4b0f-9be9-f3e1afe962d9">

### **Running the Raw snapshot**
The first part of the snapshot accumulates raw registration and staked ada information and validates it according to [CIP-15](https://cips.cardano.org/cip/CIP-15) and [CIP-36](https://cips.cardano.org/cip/CIP-36).  

*Note: Multiple delegations, as specified by CIP-36, are not supported.  These will be detected as invalid registrations.  Only registrations that contain a single voting key are supported and valid.*

<img width="672" alt="Reproducing the snapshot 2" src="https://github.com/user-attachments/assets/7a88cf8f-8d12-4941-81ea-4a276e27e20e">

### **Processing the snapshot with Fund 10 parameters**
This filters registrations for minimum allowed voting power:

<img width="672" alt="Reproducing the snapshot 3" src="https://github.com/user-attachments/assets/5d838496-e9c5-4693-846e-0f1823a0721d">

### **Official Snapshot Artifacts**
As soon as the official snapshot artifacts that will be used for Fund 10 are available, they will be linked to here.

It is possible to run the snapshot independently until they are published.
