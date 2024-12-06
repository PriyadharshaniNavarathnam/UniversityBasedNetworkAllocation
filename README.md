# University Network Design for IT Centre and Department Building

This project involves designing and implementing a robust computer network for the IT Centre and Department buildings of the University. The network ensures secure communication, optimal resource utilization, and access restrictions as per requirements.

---

## Project Objectives
- To design a structured computer network with VLANs and subnets.
- To configure routers, switches, and WiFi access points for seamless connectivity.
- To implement security measures, including restricted access to sensitive nodes and printers.

---

## Network Details
### **Building Specifications**
- **IT Centre**:
  - Total Data Points: 164
  - Includes computer labs, staff offices, meeting rooms, and WiFi coverage zones.
- **Department Building**:
  - Total Data Points: 203
  - Includes lecture halls, computer labs, research labs, and restricted zones.

### **IP Addressing**
- **IP Range**: `10.20.0.0/16`
- Subnets and VLANs are assigned using **CIDR Notation** for optimal IP address utilization.
- Sample VLAN Details:
  - **VLAN 10**:
    - Subnet: `10.20.0.0/25`
    - Usable Range: `10.20.0.1 - 10.20.0.126`
    - Subnet Mask: `255.255.255.128`
  - Full subnet details are included in the report.

### **Access Restrictions**
- Computers in staff rooms and department offices are isolated from the rest of the network.
- Printers are accessible only to the respective authorized staff groups.

---

## Implementation
### **Steps to Configure Network Devices**
1. **Router Configuration**:
   - Assign default gateways for each VLAN.
   - Configure routing between VLANs.
2. **Switch Configuration**:
   - Create and assign VLANs.
   - Configure trunk ports for inter-switch communication.
3. **WiFi Configuration**:
   - Set up SSIDs and secure with WPA2 passwords.
   - Deploy WiFi access points in lobby areas and meeting rooms.

---

## Security Measures
- Firewalls are configured to restrict unauthorized access.
- Printers are limited to specific staff groups.
- Each node is accessible only by the administrator.

---

## Testing
- Verified connectivity between VLANs where allowed.
- Tested restricted access scenarios.
- Validated WiFi and printer functionality.

---

## Files in Repository
- **Network Diagram**: Visual representation of the designed network.
- **Configuration Scripts**: Commands for routers, switches, and WiFi setup.
- **Documentation**: Detailed report with IP distribution and VLAN mapping.

---

##For more details: https://medium.com/@priyadharshaninavarathnam/designing-a-secure-and-efficient-university-network-78d974d7ab40

