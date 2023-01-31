[@c4tplatform/caminojs](../README.md) › [API-PlatformVM-Locked](../modules/api_platformvm_locked.md) › [SerializableTxID](api_platformvm_locked.serializabletxid.md)

# Class: SerializableTxID

## Hierarchy

* **SerializableTxID**

## Index

### Properties

* [txid](api_platformvm_locked.serializabletxid.md#protected-txid)

### Methods

* [decode](api_platformvm_locked.serializabletxid.md#decode)
* [encode](api_platformvm_locked.serializabletxid.md#encode)
* [fromBuffer](api_platformvm_locked.serializabletxid.md#frombuffer)
* [toBuffer](api_platformvm_locked.serializabletxid.md#tobuffer)

## Properties

### `Protected` txid

• **txid**: *Buffer* = Buffer.alloc(32)

*Defined in [src/apis/platformvm/locked.ts:22](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L22)*

## Methods

###  decode

▸ **decode**(`value`: string, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Defined in [src/apis/platformvm/locked.ts:18](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L18)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`value` | string | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  encode

▸ **encode**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *string*

*Defined in [src/apis/platformvm/locked.ts:14](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L14)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *string*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset?`: number): *number*

*Defined in [src/apis/platformvm/locked.ts:24](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L24)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/locked.ts:29](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L29)*

**Returns:** *Buffer*
