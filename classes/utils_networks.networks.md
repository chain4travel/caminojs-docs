[@c4tplatform/caminojs](../api.md) › [Utils-Networks](../modules/utils_networks.md) › [Networks](utils_networks.networks.md)

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
* [isPredefined](utils_networks.networks.md#ispredefined)
* [registerNetwork](utils_networks.networks.md#registernetwork)

## Constructors

###  constructor

\+ **new Networks**(): *[Networks](utils_networks.networks.md)*

*Defined in [src/utils/networks.ts:187](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/networks.ts#L187)*

**Returns:** *[Networks](utils_networks.networks.md)*

## Properties

###  registry

• **registry**: *Map‹string, [Network](../interfaces/utils_networks.network.md)›* = new Map()

*Defined in [src/utils/networks.ts:187](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/networks.ts#L187)*

## Methods

###  getNetwork

▸ **getNetwork**(`networkID`: number): *[Network](../interfaces/utils_networks.network.md)*

*Defined in [src/utils/networks.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/networks.ts#L198)*

**Parameters:**

Name | Type |
------ | ------ |
`networkID` | number |

**Returns:** *[Network](../interfaces/utils_networks.network.md)*

___

###  isPredefined

▸ **isPredefined**(`networkID`: number): *boolean*

*Defined in [src/utils/networks.ts:202](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/networks.ts#L202)*

**Parameters:**

Name | Type |
------ | ------ |
`networkID` | number |

**Returns:** *boolean*

___

###  registerNetwork

▸ **registerNetwork**(`networkID`: number, `network`: [Network](../interfaces/utils_networks.network.md)): *void*

*Defined in [src/utils/networks.ts:194](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/networks.ts#L194)*

**Parameters:**

Name | Type |
------ | ------ |
`networkID` | number |
`network` | [Network](../interfaces/utils_networks.network.md) |

**Returns:** *void*
