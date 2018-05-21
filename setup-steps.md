# Setting up OneConsultation

OneConsultation is a fully managed hosted service, so there's not a lot of time-consuming setup, no machines to configure and no client settings to roll out. 

# To start using OneConsultation (production or trial)

## Step 1 : tell us!
----
Before you can start using OneConsultation (even a trial) you need to tell us, so that we can provision the service for you. Contact your Modality Systems Account Manager, or email [labs@modalitysystems.com](mailto:labs@modalitysystems.com).

We will provide you with details of your portal address and a named point of contact to work with throughout the remaining setup steps. Typically the entire process, from telling us to having customer make test consultations takes between 2-4 working days, provided Step 2 is completed promptly (see below).

## Step 2 : find your Office 365 Tenant ID
----

Your Office 365 tenant ID is a globally unique identifier (GUID) that is different than your tenant name or domain. It's allocated to you by Microsoft and never changes.

We use your tenant ID when you authenticate with OneConsultation to work out which consultations to show you. Your tenant ID acts as a the "key" to showing you only consultations which are meant for your organisations, and hiding those consultations from any other OneConsultation user. We need to know your tenant ID before you can start using OneConsultation.

To find your tenant ID:

**Use the Azure AD portal**

Office 365 uses Azure AD to manage user accounts. You can find your tenant ID in the Azure AD portal. You'll need to be an Azure AD administrator. To find your Office 365 tenant ID in the Azure AD portal:

 1. Log in to Microsoft Azure as an administrator.
 2. In the Microsoft Azure portal, click Azure Active Directory.
 3. Under Manage, click Properties. The tenant ID is shown in the Directory ID box.

**Use Windows PowerShell**

You can use Windows PowerShell to find the tenant ID. You'll need the [Microsoft Azure PowerShell module](https://go.microsoft.com/fwlink/p/?LinkId=717444).

Open a Microsoft Azure PowerShell command window and run the following script, entering your Office 365 credentials when prompted.

```
Login-AzureRmAccount
```

Your tenant ID is listed in the output.

Once you have your tenant ID, provide it to us along with the additional information in Step 3.

## Step 3: Decide on users, room areas and customisations.
----
For trials, all users in your organisation are automatically granted access to use OneConsultation, and a single room area is created. However, there are a number of customisations you can make during the trial process, before you progress from trial to production, or at any time when in production:

### Users
For production, to restrict access to a defined list of users, provide us with a whitelist of users. There is no charge per user, as many users as required can be added. If multiple room areas are required, provide us with details of numbers and display names.

### Appearance
For both production and trial, it is possible to customise the appearance of the user-facing portal. The image, title text, explanatory wording and questions can all be changed. Provide us with details of any required changes. Changes can take up to 3 working days.

### Vanity URL
For both production and trial, it is possible to mask the provided portal URL with a vanity URL (for instance, *video.yourcompany.com*). To do this, you will need to create a CNAME entry for the desired subdomain, pointing to the URL we provided you. You will also need to inform us so we can configure the vanity URL, and provide the matching PFX certificate file and password.

## (Optional Step 4: check network firewall rules)
Once in production it's likely that most users accessing OneConsultation will be doing so from outside of your corporate firewall, so no changes are necessary. Whilst conducting trials, however, you may be using OneConsultation within your corporate network boundary, in which case you should make sure that sufficient access is enabled to reach OneConsultation's video bridging services.

In order to use OneConsultation, ensure web-browser clients have UDP access outbound to:

 - 51.140.26.197
 - 51.140.115.27
 - 13.94.141.192
 - 13.94.146.220
 - 40.71.84.17
 - 13.92.129.46

These are worldwide nodes to ensure that wherever users connect to the service from, they are routed to the most appropriate local node for the best audio & video experience.


