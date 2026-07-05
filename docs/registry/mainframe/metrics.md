
# Metrics: `mainframe`

This document describes the `mainframe` metrics.


## `mainframe.cpu.physical.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of physical CPUs in the mainframe system of a specific type.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`


### Attributes

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.cpu.mode` | Enum | Required | Mode the processor is operating in. The mode can be either 'dedicated' or 'shared'. |
| `mainframe.cpu.type` | Enum | Required | Type of mainframe processor. |


