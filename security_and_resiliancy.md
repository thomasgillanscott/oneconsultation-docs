# Security and Service Resiliancy

## Security

OneConsultation is hosted in Microsoft Azure and therefore adheres to Microsoft security practices for access to any part of the service. 

Access to the Admin Portal to view waiting consultations is restricted by Azure Active Directory and only visible to users who authenticate using credentials from your tenant. Modality Systems do not have access to access this process or view any waiting consultations.

Modality Systems is ISO27001 accredited and conforms to the practices around access and account control in accessing the service. Modality does have access to the configuration and management of the underlying video bridging service for the purposes of managing and maintaining the service, but this contains no user information.

For more information about how security is managed within Microsoft Azure, visit the [Azure Trust Centre](https://www.microsoft.com/en-us/trustcenter/security/azure-security).

For information about the different compliance offerings which Microsoft Azure can support worldwide, see the [current list of compliance offerings](https://www.microsoft.com/en-us/trustcenter/compliance/complianceofferings).

## Data Security

The system does not store any user data at rest. Public user information gathered via the pre-consultation questions is only stored in memory for the purposes of displaying in the Admin Portal, and is never persisted to an at rest service.

## Resiliancy

OneConsultation is hosted entirely in Microsoft Azure and makes use of multiple Azure offerings to ensure a consistent user experience.

The underlying video bridging service which OneConsultation uses is also hosted on the Microsoft Azure platform, providing local connectivity ingress points to the service in multiple geographical regions.

The service has multiple conference nodes in each region; in the event of node failure the system will move onto the next available node in that region. If all nodes are not available in a region then the service can failover to the next region. This provides multiple points of failure in the service. Uptime of regions and nodes in monitored by Modality Systems Support Team which operate a 24/7 "follow the sun" support and response service.
