## 3. Setup Summary

### 3.1 pfSense Firewall & Network Segmentation

![pfSense Interfaces](images/pfsense%20DHCP%20setup.png)  
*pfSense interface configuration showing WAN, ECORP LAN, and Attack LAN networks with DHCP enabled.*

---

### 3.2 Firewall Rules

![Firewall Rule 1](images/pfsense%20firewall%20rule1.png)  
*Firewall rule allowing traffic to all devices on the ECORP network.*

![Firewall Rule 4](images/pfsense%20firewall%20rule4.png)  
*Firewall rule blocking all remaining traffic from ECORP subnets.*

![Firewall Rule 5](images/pfsense%20firewall%20rule5.png)  
*Attack LAN rule allowing traffic to ECORP LAN subnets.*

![Firewall Rule 7](images/pfsense%20firewall%20rule7.png)  
*Attack LAN rule blocking traffic to WAN subnets.*

---

### 3.3 Windows 11 Domain Join

![AD Setup](images/ADsetup1-Win11.png)  
*Windows 11 client joining the `ECORP.local` Active Directory domain.*

---

### 3.4 Kali Linux (Attack LAN)

![Kali ifconfig](images/kali1.png)  
*Kali Linux attack VM configured on the Attack LAN (showing IP via ifconfig).*

---

### 3.5 Metasploitable Target

![Metasploitable ifconfig](images/metasploitable.png)  
*Metasploitable vulnerable Linux target on the ECORP LAN with IP confirmed.*
