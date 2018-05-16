# Security and Service Resiliancy

## Security

OneConsultation is hosted in Microsoft Azure and therefore adheres to Microsoft security practices for access to any part of the service. 

Access to the Admin Portal to view waiting consultations is restricted by Azure Active Directory and only visible to users who authenticate using credentials from the customer's tenant. Modality Systems do not have access to access this process or view any customer's waiting consultations.

Modality Systems is ISO27001 accredited and conform to the practices around access and account control in accessing the service. Modality does have acccess to the configuration and management of the underlying video bridging service for the purposes of managing and maintaining the service, but this contains no user information.

For more information about how security is managed within Microsoft Azure, visit the [Azure Trust Centre](https://www.microsoft.com/en-us/trustcenter/security/azure-security).

For information about the different compliance offerings which Microsoft Azure can support worldwide, see the [current list of compliance offerings](https://www.microsoft.com/en-us/trustcenter/compliance/complianceofferings).

## Data Security

The system does not store any user data at rest. User information gathered via the questions users are asked is only stored in memory for the purposes of diplaying in the Admin Portal, and is never persisted to an at rest service.

## Resiliancy

OneConsultation is hosted entirely in Microsoft Azure and makes use of multiple Azure offerings to ensure a consistant user experience.

The underlying video bridging service which OneConsultation uses is also hosted on the Microosft Azure platform, providing local connectivity ingress points to the service in multiple geographical regions.

The service has multiple conference nodes in each region; in the event of node failure the system will move onto the next available node in that region. If all nodes are not available in a region then the service can failover to the next region. This provides multiple points of failure in the service. Uptime of regions and nodes in monitored by Modality Systems Support Team which operate a 24/7 "follow the sun" support and response service.
