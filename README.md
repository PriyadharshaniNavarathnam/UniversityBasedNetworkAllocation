

## Project Overview

This project is a self-learning assignment focused on designing a computer network for the IT Centre and Department building of a university. The network is designed to provide optimal use of IP addresses, including subnets and VLANs, router and switch configuration, and WiFi access points setup.

## Project Details

### Building Specifications

- **Buildings**: IT Centre and Department building
- **Dimensions**: 
  - Length: 70 meters
  - Width: 30 meters
  - Height: 4 meters per floor
  - Number of Floors: 2

### Network Requirements

- **IP Address Range**: 10.20.0.0/16
- **Subnets and VLANs**: 
  - Each building area and function (e.g., labs, staff rooms, offices) are assigned specific subnets and VLANs.
- **Access Restrictions**:
  - Staff room computers are isolated from other areas.
  - Department office computers are isolated from other areas.
  - Printers are restricted to department staff or IT Centre staff respectively.
  - Only administrators can access network nodes.

### Components and Configurations

- **Network Diagram**: Includes subnets and VLAN assignments.
- **Router and Switch Configuration**: Steps to configure routers and switches.
- **WiFi Access Points**: Configuration details for wireless networks.
- **Security Measures**: VLAN assignments and access restrictions to ensure security.

### VLAN and IP Address Distribution

| VLAN Name | VLAN No | VLAN ID          | Required Size | Allocated Size | IP Address Range     | Subnet Mask         | CIDR  | Broadcast Address |
|-----------|---------|------------------|---------------|----------------|----------------------|---------------------|-------|-------------------|
| Block10   | 10      | 10.20.0.0/25     | 120           | 128            | 10.20.0.1-10.20.0.126| 255.255.255.128     | /25   | 10.20.0.127       |
| Block20   | 20      | 10.20.0.128/25   | 100           | 128            | 10.20.0.129-10.20.0.254| 255.255.255.128  | /25   | 10.20.0.255       |
| Block30   | 30      | 10.20.1.0/26     | 50            | 64             | 10.20.1.1-10.20.1.62 | 255.255.255.192     | /26   | 10.20.1.63        |
| Block40   | 40      | 10.20.1.64/26    | 34            | 64             | 10.20.1.65-10.20.1.126| 255.255.255.192    | /26   | 10.20.1.127       |
| Block50   | 50      | 10.20.1.128/27   | 30            | 32             | 10.20.1.129-10.20.1.158| 255.255.255.224   | /27   | 10.20.1.159       |
| Block60   | 60      | 10.20.1.160/28   | 14            | 16             | 10.20.1.161-10.20.1.174| 255.255.255.240   | /28   | 10.20.1.175       |
| Block70   | 70      | 10.20.1.176/28   | 7             | 16             | 10.20.1.177-10.20.1.190| 255.255.255.240   | /28   | 10.20.1.191       |
| Block80   | 80      | 10.20.1.192/29   | 5             | 8              | 10.20.1.193-10.20.1.198| 255.255.255.248   | /29   | 10.20.1.199       |
| Block90   | 90      | 10.20.1.200/29   | 5             | 8              | 10.20.1.201-10.20.1.206| 255.255.255.248   | /29   | 10.20.1.207       |
| Block100  | 100     | 10.20.1.208/29   | 3             | 8              | 10.20.1.209-10.20.1.214| 255.255.255.248   | /29   | 10.20.1.215       |
| Block110  | 110     | 10.20.1.216/29   | 3             | 8              | 10.20.1.217-10.20.1.222| 255.255.255.248   | /29   | 10.20.1.223       |

### Steps for Configuration

1. **Router Configuration**: Set up the router with default gateways for each VLAN.
2. **Switch Configuration**: Assign VLANs to switch ports and set up trunk ports.
3. **WiFi Configuration**: Set up WiFi routers with appropriate SSID and passwords.
4. **Access Control**: Configure firewall rules to restrict access as per requirements.

## Project Author

- **Name**: Priyadharshani N.
- **Student ID**: 2020 / E / 120


## Additional Information

For detailed network diagrams and configuration steps, refer to the included figures and tables in the project documentation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
