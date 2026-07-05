
# Entities: `zos`

This document describes the `zos` entities.


## `zos.software` ![Development](https://img.shields.io/badge/-development-blue)

A software resource running on a z/OS system.


| Property | Value |
|----------|-------|
| Stability | Development |





### Description

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.partition.name` | `string` | Required | Name of the logical partition that hosts a systems with a mainframe operating system. |
| `zos.smf.id` | `string` | Required | The System Management Facility (SMF) Identifier uniquely identified a z/OS system within a SYSPLEX or mainframe environment and is used for system and performance analysis. |
| `zos.sysplex.name` | `string` | Required | The name of the SYSPLEX to which the z/OS system belongs too. |


