# ![LOGO](logo.png) Google Compute Engine Instance Group Manager **flow**ground Connector

## Description

A generated **flow**ground connector for the Google Compute Engine Instance Group Manager API (version v1beta2).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/replicapool/v1beta2/swagger.json<br/>
Generated at: 2019-05-07T17:41:53+03:00

## API Description

[Deprecated. Please use Instance Group Manager in Compute API] Provides groups of homogenous Compute Engine instances.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Retrieves the list of Instance Group Manager resources contained within the specified zone.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `filter` - _optional_ - Optional. Filter expression for filtering listed resources.
* `maxResults` - _optional_ - Optional. Maximum count of results to be returned. Maximum value is 500 and default value is 500.
* `pageToken` - _optional_ - Optional. Tag returned by a previous list request truncated by maxResults. Used to continue a previous list request.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates an instance group manager, as well as the instance group and the specified number of instances.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `project` - _required_ - The Google Developers Console project name.
* `size` - _required_ - Number of instances that should exist.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the instance group manager and all instances contained within. If you'd like to delete the manager without deleting the instances, you must first abandon the instances to remove them from the group.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - Name of the Instance Group Manager resource to delete.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns the specified Instance Group Manager resource.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - Name of the instance resource to return.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Removes the specified instances from the managed instance group, and from any target pools of which they were members, without deleting the instances.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - The name of the instance group manager.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified instances. The instances are deleted, then removed from the instance group and any target pools of which they were a member. The targetSize of the instance group manager is reduced by the number of instances deleted.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - The name of the instance group manager.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Recreates the specified instances. The instances are deleted, then recreated using the instance group manager's current instance template.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - The name of the instance group manager.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Resizes the managed instance group up or down. If resized up, new instances are created using the current instance template. If resized down, instances are removed in the order outlined in Resizing a managed instance group.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - The name of the instance group manager.
* `project` - _required_ - The Google Developers Console project name.
* `size` - _required_ - Number of instances that should exist in this Instance Group Manager.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sets the instance template to use when creating new instances in this group. Existing instances are not affected.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - The name of the instance group manager.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Modifies the target pools to which all new instances in this group are assigned. Existing instances in the group are not affected.

*Tags:* `instanceGroupManagers`

#### Input Parameters
* `instanceGroupManager` - _required_ - The name of the instance group manager.
* `project` - _required_ - The Google Developers Console project name.
* `zone` - _required_ - The name of the zone in which the instance group manager resides.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the list of operation resources contained within the specified zone.

*Tags:* `zoneOperations`

#### Input Parameters
* `filter` - _optional_ - Optional. Filter expression for filtering listed resources.
* `maxResults` - _optional_ - Optional. Maximum count of results to be returned. Maximum value is 500 and default value is 500.
* `pageToken` - _optional_ - Optional. Tag returned by a previous list request truncated by maxResults. Used to continue a previous list request.
* `project` - _required_ - Name of the project scoping this request.
* `zone` - _required_ - Name of the zone scoping this request.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the specified zone-specific operation resource.

*Tags:* `zoneOperations`

#### Input Parameters
* `operation` - _required_ - Name of the operation resource to return.
* `project` - _required_ - Name of the project scoping this request.
* `zone` - _required_ - Name of the zone scoping this request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-replicapool-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
