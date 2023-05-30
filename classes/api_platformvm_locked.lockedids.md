[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Locked](../modules/api_platformvm_locked.md) › [LockedIDs](api_platformvm_locked.lockedids.md)

# Class: LockedIDs

## Hierarchy

* **LockedIDs**

## Index

### Constructors

* [constructor](api_platformvm_locked.lockedids.md#constructor)

### Properties

* [bondTxID](api_platformvm_locked.lockedids.md#protected-bondtxid)
* [depositTxID](api_platformvm_locked.lockedids.md#protected-deposittxid)

### Methods

* [deserialize](api_platformvm_locked.lockedids.md#deserialize)
* [fromBuffer](api_platformvm_locked.lockedids.md#frombuffer)
* [getBondTxID](api_platformvm_locked.lockedids.md#getbondtxid)
* [getDepositTxID](api_platformvm_locked.lockedids.md#getdeposittxid)
* [serialize](api_platformvm_locked.lockedids.md#serialize)
* [toBuffer](api_platformvm_locked.lockedids.md#tobuffer)

## Constructors

###  constructor

\+ **new LockedIDs**(`depositTxID?`: Buffer, `bondTxID?`: Buffer): *[LockedIDs](api_platformvm_locked.lockedids.md)*

*Defined in [src/apis/platformvm/locked.ts:73](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L73)*

Class representing an [LockedIDs](api_platformvm_locked.lockedids.md) for LockedIn and LockedOut types.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`depositTxID?` | Buffer | txID where this Output is deposited on |
`bondTxID?` | Buffer | txID where this Output is bonded on  |

**Returns:** *[LockedIDs](api_platformvm_locked.lockedids.md)*

## Properties

### `Protected` bondTxID

• **bondTxID**: *[SerializableTxID](api_platformvm_locked.serializabletxid.md)* = new SerializableTxID()

*Defined in [src/apis/platformvm/locked.ts:53](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L53)*

___

### `Protected` depositTxID

• **depositTxID**: *[SerializableTxID](api_platformvm_locked.serializabletxid.md)* = new SerializableTxID()

*Defined in [src/apis/platformvm/locked.ts:52](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L52)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Defined in [src/apis/platformvm/locked.ts:47](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L47)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Defined in [src/apis/platformvm/locked.ts:62](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L62)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getBondTxID

▸ **getBondTxID**(): *[SerializableTxID](api_platformvm_locked.serializabletxid.md)*

*Defined in [src/apis/platformvm/locked.ts:58](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L58)*

**Returns:** *[SerializableTxID](api_platformvm_locked.serializabletxid.md)*

___

###  getDepositTxID

▸ **getDepositTxID**(): *[SerializableTxID](api_platformvm_locked.serializabletxid.md)*

*Defined in [src/apis/platformvm/locked.ts:55](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L55)*

**Returns:** *[SerializableTxID](api_platformvm_locked.serializabletxid.md)*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Defined in [src/apis/platformvm/locked.ts:39](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L39)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/locked.ts:68](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/locked.ts#L68)*

**Returns:** *Buffer*
