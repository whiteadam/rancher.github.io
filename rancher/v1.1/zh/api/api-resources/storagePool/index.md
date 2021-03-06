---
title: API
layout: rancher-api-default-v1.1
version: v1.1
lang: zh
---

## storagePool

A storage pool is a list of hosts that can participate in shared storage.

### Resource Fields

#### Writeable Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
description | string | Optional | Yes | - | 
name | string | Optional | Yes | - | 


#### Read Only Fields

Field | Type   | Notes
---|---|---
accountId | [account]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/api-resources/account/)  | The unique identifier for the associated account
blockDevicePath | string  | 
created | date  | The date of when the storagePool was created.
driverName | string  | 
externalId | string  | 
id | int  | The unique identifier for the storagePool
kind | string  | 
removed | date  | The date of when the storagePool was removed
state | enum  | The current state of the storagePool. The options are [activating, active, deactivating, inactive, purged, purging, registering, removed, removing, requested, restoring, updating-active, updating-inactive].
transitioning | enum  | Whether or not the storagePool is in a transitioning state
transitioningMessage | string  | The message to show while in a transitioning state
transitioningProgress | int  | The percentage remaining in the transitioning process of the storagePool
uuid | string  | The universally unique identifier for the storagePool. This will always be unique across Rancher installations.
volumeAccessMode | string  | 
volumeCapabilities | array[string]  | 


<br>
