# Security and Service Resiliancy

## Security

OneConsultation is hosted in Microsoft Azure and therefore adheres to Microsoft security practices for access to any part of the service. 

Access to the Admin Portal to view waiting consultations is restricted by Azure Active Directory and only visible to users who authenticate using credentials from the customer's tenant. Modality Systems do not have access to access this process or view any customer's waiting consultations.

Modality Systems is ISO27001 accredited and conform to the practices around access and account control in accessing the service. Modality does have acccess to the configuration and management of the underlying video bridging service for the purposes of managing and maintaining the service, but this contains no user information.

## Data

The system does not store any user data at rest. User information gathered via the questions users are asked is only stored in memory for the purposes of diplaying in the Admin Portal, and is never persisted to an at rest service.