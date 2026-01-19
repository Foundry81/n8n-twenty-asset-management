# Twenty CRM `IT Assets` Object
IT assets including hardware systems, software, SaaS information, and configurations. No sensitive information is kept in this system. Authentication details are stored elsewhere; detailed system information lives in the docs.

## Relations
Defines the relationship between IT Asset objects and other objects in the CRM:

| Name            | App    | Type         | Value                         |
| --------------- | ------ | ------------ | ----------------------------- |
| Primary Owner   | Custom |  One-to-many | Workspace/Organization/Person |
| Secondary Owner | Custom |  One-to-many | Workspace/Organization/Person |

## Fields
Standard (App) and custom fields, values are for select/multi-select (or boolean) field:

| Name                      | App    | Data type     | Values                                                                          |
| ------------------------- | ------ | ------------- | ------------------------------------------------------------------------------- |
| Access Method             | Custom | Multi-select  | Console/SSH/Web/API                                                             |
| Asset Category            | Custom | Select        | Physical/Virtual/Cloud/Logical                                                  |
| Asset Type                | Custom | Select        | Server/Virtual Machine/Container/Network Device/SaaS/Service/SBC/Laptop/Cluster |
| Backup Location           | Custom | Multi-select  | Local/Remote                                                                    |
| Backup Status             | Custom | Select        | None/Config Only/Full/Containers/Proxmox Backup Server                          |
| Business Function/Role    | Custom | Text          |                                                                                 |
| Clock Speed               | Custom | Number        |                                                                                 |
| CPU Architecture          | Custom | Text          |                                                                                 |
| CPU Cores                 | Custom | Number        |                                                                                 |
| CPU Model                 | Custom | Text          |                                                                                 |
| Created by                | App    | Actor         |                                                                                 |
| Creation date             | App    | Date and Time |                                                                                 |
| Current Purpose           | Custom | Text          |                                                                                 |
| Date Commissionsed        | Custom | Date          |                                                                                 |
| Deleted at                | App    | Date and Time |                                                                                 |
| Downtime Operational Risk | Custom | Select        | High/Medium/Low/NBD                                                             |
| Environment               | Custom | Select        | Production/Lab/Development/Testing/Deprecated                                   |
| Intended Purpose          | Custom | Text          |                                                                                 |
| Internal Documentation    | Custom | Links         |                                                                                 |
| IP Addresses              | Custom | Array         |                                                                                 |
| Last Reviewed             | Custom | Date          |                                                                                 |
| Last update               | App    | Date and Time |                                                                                 |
| Lifecycle Stage           | Custom | Select        | Planned/In Service/End of Life                                                  |
| Logical Location          | Custom | Text          |                                                                                 |
| Management IP             | Custom | Text          |                                                                                 |
| Management URL            | Custom | Links         |                                                                                 |
| Memory                    | Custom | Text          |                                                                                 |
| n8n Credential            | Custom | Text          |                                                                                 |
| n8n Workflow              | Custom | Select        | Linux/Synology/TrueNAS                                                          |
| Name                      | App    | Text          |                                                                                 |
| Operational Status        | Custom | Select        | Active/Maintenance/Degraded/Retired                                             |
| OS                        | Custom | Text          |                                                                                 |
| OS Version                | Custom | Text          |                                                                                 |
| Physical Location         | Custom | Text          |                                                                                 |
| Public Documentation      | Custom | Links         |                                                                                 |
| Purpose Drift             | Custom | True/False    | True/False                                                                      |
| Restore Point Objective   | Custom | Number        |                                                                                 |
| Restore Time Objective    | Custom | Number        |                                                                                 |
| Storage                   | Custom | Text          |                                                                                 |
| Updated by                | Custom | Actor         |                                                                                 |
