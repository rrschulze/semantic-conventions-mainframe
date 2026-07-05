
# Metrics: `mainframe`

This document describes the `mainframe` metrics.


## `mainframe.channel.utilization` ![Development](https://img.shields.io/badge/-development-blue)

The percentage of time the channel was processing I/O.


**Instrument**: `gauge`

**Unit**: `1`


### Attributes

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.channel.mode` | Enum | Required | Mode the I/O channel is operating in. The mode can be either 'dedicated' or 'shared'. |



## `mainframe.cpu.active.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of active processors in the mainframe system of a specific type.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`


### Attributes

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.cpu.type` | Enum | Required | Type of mainframe processor. |



## `mainframe.cpu.defective.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of defective processors in the mainframe system.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`



## `mainframe.cpu.spare.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of spare processors in the mainframe system.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`


