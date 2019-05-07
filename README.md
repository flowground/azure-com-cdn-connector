# ![LOGO](logo.png) CdnManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the CdnManagementClient API (version 2017-10-12).

Generated from: https://api.apis.guru/v2/specs/azure.com/cdn/2017-10-12/swagger.json<br/>
Generated at: 2019-05-07T17:37:42+03:00

## API Description

Use these APIs to manage Azure CDN resources through the Azure Resource Manager. You must make sure that requests made to these resources are secure.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Check the availability of a resource name. This is needed for resources where name is globally unique, such as a CDN endpoint.

*Tags:* `CheckNameAvailability`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Edgenodes are the global Point of Presence (POP) locations used to deliver CDN content to end users.

*Tags:* `Edgenodes`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Lists all of the available CDN REST API operations.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Check the availability of a resource name. This is needed for resources where name is globally unique, such as a CDN endpoint.

*Tags:* `CheckNameAvailabilityWithSubscription`

#### Input Parameters
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Check the quota and actual usage of the CDN profiles under the given subscription.

*Tags:* `CheckResourceUsage`

#### Input Parameters
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Lists all of the CDN profiles within an Azure subscription.

*Tags:* `Profiles`

#### Input Parameters
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Check if the probe path is a valid path and the file can be accessed. Probe path is the path to a file hosted on the origin server to help accelerate the delivery of dynamic content via the CDN endpoint. This path is relative to the origin path specified in the endpoint configuration.

*Tags:* `ValidateProbe`

#### Input Parameters
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Lists all of the CDN profiles within a resource group.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Deletes an existing CDN profile with the specified parameters. Deleting a profile will result in the deletion of all of the sub-resources including endpoints, origins and custom domains.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Gets a CDN profile with the specified profile name under the specified subscription and resource group.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Updates an existing CDN profile with the specified profile name under the specified subscription and resource group.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Creates a new CDN profile with a profile name under the specified subscription and resource group.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Checks the quota and actual usage of endpoints under the given CDN profile.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Lists existing CDN endpoints.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Deletes an existing CDN endpoint with the specified endpoint name under the specified subscription, resource group and profile.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Gets an existing CDN endpoint with the specified endpoint name under the specified subscription, resource group and profile.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Updates an existing CDN endpoint with the specified endpoint name under the specified subscription, resource group and profile. Only tags and Origin HostHeader can be updated after creating an endpoint. To update origins, use the Update Origin operation. To update custom domains, use the Update Custom Domain operation.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Creates a new CDN endpoint with the specified endpoint name under the specified subscription, resource group and profile.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Checks the quota and usage of geo filters and custom domains under the given endpoint.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Lists all of the existing custom domains within an endpoint.

*Tags:* `CustomDomains`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Deletes an existing custom domain within an endpoint.

*Tags:* `CustomDomains`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `customDomainName` - _required_ - Name of the custom domain within an endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Gets an existing custom domain within an endpoint.

*Tags:* `CustomDomains`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `customDomainName` - _required_ - Name of the custom domain within an endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Creates a new custom domain within an endpoint.

*Tags:* `CustomDomains`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `customDomainName` - _required_ - Name of the custom domain within an endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Disable https delivery of the custom domain.

*Tags:* `CustomDomains`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `customDomainName` - _required_ - Name of the custom domain within an endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Enable https delivery of the custom domain.

*Tags:* `CustomDomains`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `customDomainName` - _required_ - Name of the custom domain within an endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Pre-loads a content to CDN. Available for Verizon Profiles.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Lists all of the existing origins within an endpoint.

*Tags:* `Origins`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Gets an existing origin within an endpoint.

*Tags:* `Origins`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `originName` - _required_ - Name of the origin which is unique within the endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Updates an existing origin within an endpoint.

*Tags:* `Origins`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `originName` - _required_ - Name of the origin which is unique within the endpoint.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Removes a content from CDN.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Starts an existing CDN endpoint that is on a stopped state.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Stops an existing running CDN endpoint.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Validates the custom domain mapping to ensure it maps to the correct CDN endpoint in DNS.

*Tags:* `Endpoints`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `endpointName` - _required_ - Name of the endpoint under the profile which is unique globally.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Generates a dynamic SSO URI used to sign in to the CDN supplemental portal. Supplemental portal is used to configure advanced feature capabilities that are not yet available in the Azure portal, such as core reports in a standard profile; rules engine, advanced HTTP reports, and real-time stats and alerts in a premium profile. The SSO URI changes approximately every 10 minutes.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

### Gets the supported optimization types for the current profile. A user can create an endpoint with an optimization type from the listed values.

*Tags:* `Profiles`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the Resource group within the Azure subscription.
* `profileName` - _required_ - Name of the CDN profile which is unique within the resource group.
* `subscriptionId` - _required_ - Azure Subscription ID.
* `api-version` - _required_ - Version of the API to be used with the client request. Current version is 2017-04-02.

## License

**flow**ground :- Telekom iPaaS / azure-com-cdn-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
