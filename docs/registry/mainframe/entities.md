
# Entities: `mainframe`

This document describes the `mainframe` entities.


## `mainframe.host` ![Development](https://img.shields.io/badge/-development-blue)

A mainframe host, representing the pyhsical machine, also known as the Central Processor Complex (CPC).


| Property | Value |
|----------|-------|
| Stability | Development |




### Identity

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `host.name` | `string` | Required | Name of the host. On Unix systems, it may contain what the hostname command returns, or the fully qualified hostname, or another name specified by the user. |



### Description

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `host.arch` | Enum | Recommended | The CPU architecture the host system is running on. |
| `host.id` | `string` | Recommended | Unique host ID. For Cloud, this must be the instance_id assigned by the cloud provider. For non-containerized systems, this should be the `machine-id`. See the table below for the sources to use to determine the `machine-id` based on operating system. |
| `host.type` | `string` | Recommended | Type of host. For Cloud, this must be the machine type. |
| `mainframe.host.machine_model` | `string` | Recommended | IBM machine model of the Central Processor Complex (CPC). |
| `mainframe.host.machine_type` | `string` | Recommended | Four-digit IBM machine type of the Central Processor Complex (CPC). |
| `mainframe.host.serial_number` | `string` | Recommended | Serial number of the central processing complex (CPC). |


