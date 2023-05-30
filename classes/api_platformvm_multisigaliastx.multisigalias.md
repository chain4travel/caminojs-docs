[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-MultisigAliasTx](../modules/api_platformvm_multisigaliastx.md) › [MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md)

# Class: MultisigAlias

Class representing a Multisig Alias object.

## Hierarchy

* **MultisigAlias**

## Index

### Constructors

* [constructor](api_platformvm_multisigaliastx.multisigalias.md#constructor)

### Properties

* [id](api_platformvm_multisigaliastx.multisigalias.md#protected-id)
* [memo](api_platformvm_multisigaliastx.multisigalias.md#protected-memo)
* [owners](api_platformvm_multisigaliastx.multisigalias.md#protected-owners)

### Methods

* [deserialize](api_platformvm_multisigaliastx.multisigalias.md#deserialize)
* [fromBuffer](api_platformvm_multisigaliastx.multisigalias.md#frombuffer)
* [getMemo](api_platformvm_multisigaliastx.multisigalias.md#getmemo)
* [serialize](api_platformvm_multisigaliastx.multisigalias.md#serialize)
* [toBuffer](api_platformvm_multisigaliastx.multisigalias.md#tobuffer)

## Constructors

###  constructor

\+ **new MultisigAlias**(`id`: Buffer, `memo`: Buffer, `owners`: [ParseableOutput](api_platformvm_outputs.parseableoutput.md)): *[MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:29](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L29)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`id` | Buffer | undefined |
`memo` | Buffer | undefined |
`owners` | [ParseableOutput](api_platformvm_outputs.parseableoutput.md) | undefined |

**Returns:** *[MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md)*

## Properties

### `Protected` id

• **id**: *Buffer‹›* = Buffer.alloc(20)

*Defined in [src/apis/platformvm/multisigaliastx.ts:27](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L27)*

___

### `Protected` memo

• **memo**: *Buffer‹›* = Buffer.alloc(256)

*Defined in [src/apis/platformvm/multisigaliastx.ts:28](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L28)*

___

### `Protected` owners

• **owners**: *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)* = undefined

*Defined in [src/apis/platformvm/multisigaliastx.ts:29](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L29)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *this*

*Defined in [src/apis/platformvm/multisigaliastx.ts:47](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L47)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *this*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Defined in [src/apis/platformvm/multisigaliastx.ts:68](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L68)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getMemo

▸ **getMemo**(): *Buffer*

*Defined in [src/apis/platformvm/multisigaliastx.ts:43](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L43)*

**Returns:** *Buffer*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Defined in [src/apis/platformvm/multisigaliastx.ts:60](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L60)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/multisigaliastx.ts:83](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L83)*

**Returns:** *Buffer*
