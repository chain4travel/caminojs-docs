[@c4tplatform/caminojs](../README.md) › [Utils-Networks](../modules/utils_networks.md) › [Networks](utils_networks.networks.md)

# Class: Networks

A class for storing predefined / fetched networks

## Hierarchy

* **Networks**

## Index

### Constructors

* [constructor](utils_networks.networks.md#constructor)

### Properties

* [registry](utils_networks.networks.md#registry)

### Methods

* [getNetwork](utils_networks.networks.md#getnetwork)
* [registerNetwork](utils_networks.networks.md#registernetwork)

## Constructors

###  constructor

\+ **new Networks**(): *[Networks](utils_networks.networks.md)*

*Defined in [src/utils/networks.ts:178](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L178)*

**Returns:** *[Networks](utils_networks.networks.md)*

## Properties

###  registry

• **registry**: *Map‹string, [Network](../interfaces/utils_networks.network.md)›* = new Map()

*Defined in [src/utils/networks.ts:178](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L178)*

## Methods

###  getNetwork

▸ **getNetwork**(`networkID`: number): *[Network](../interfaces/utils_networks.network.md)*

*Defined in [src/utils/networks.ts:189](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L189)*

**Parameters:**

Name | Type |
------ | ------ |
`networkID` | number |

**Returns:** *[Network](../interfaces/utils_networks.network.md)*

___

###  registerNetwork

▸ **registerNetwork**(`networkID`: number, `network`: [Network](../interfaces/utils_networks.network.md)): *void*

*Defined in [src/utils/networks.ts:185](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L185)*

**Parameters:**

Name | Type |
------ | ------ |
`networkID` | number |
`network` | [Network](../interfaces/utils_networks.network.md) |

**Returns:** *void*
