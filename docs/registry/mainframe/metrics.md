
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



## `mainframe.host.channel.utilization` ![Development](https://img.shields.io/badge/-development-blue)

The average percentage of time the channels of the mainframe system were processing I/O.


**Instrument**: `gauge`

**Unit**: `{cpu}`



## `mainframe.host.cpu.active.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of active processors in the mainframe system of a specific type.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`


### Attributes

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.cpu.type` | Enum | Required | Type of mainframe processor. |



## `mainframe.host.cpu.defective.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of defective processors in the mainframe system.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`



## `mainframe.host.cpu.spare.count` ![Development](https://img.shields.io/badge/-development-blue)

The number of spare processors in the mainframe system.


**Instrument**: `updowncounter`

**Unit**: `{cpu}`



## `mainframe.host.cpu.utilization` ![Development](https://img.shields.io/badge/-development-blue)

The utilization percentage for processors of the specified type. Set to -1 when no processors of this type are present.


**Instrument**: `gauge`

**Unit**: `{cpu}`


### Attributes

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.cpu.mode` | Enum | Required | Mode the processor is operating in. The mode can be either 'dedicated' or 'shared'. |
| `mainframe.cpu.type` | Enum | Required | Type of mainframe processor. |
| `cpu.mode` | Enum | Recommended | The mode of the CPU |
| `cpu.logical_number` | `int` | Opt-In | The logical CPU number [0..n-1] |



## `mainframe.host.memory.size` ![Development](https://img.shields.io/badge/-development-blue)

Size of memory in the mainframe system of a specific type.


**Instrument**: `gauge`

**Unit**: `MiBy`


### Attributes

| Attribute | Type | Requirement Level | Description |
|-----------|------|-------------------|-------------|
| `mainframe.memory.type` | Enum | Required | Type of mainframe memory. |



## `mainframe.host.memory.vfm.increment.size` ![Development](https://img.shields.io/badge/-development-blue)

Size of the IBM Virtual Flash Memory (VFM) memory increments of the mainframe system.


**Instrument**: `gauge`

**Unit**: `GiBy`



## `mainframe.host.memory.vfm.size` ![Development](https://img.shields.io/badge/-development-blue)

Total size of the installed IBM Virtual Flash Memory (VFM) memory in the mainframe system.


**Instrument**: `gauge`

**Unit**: `GiBy`


