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
* [serialize](api_platformvm_locked.lockedids.md#serialize)
* [toBuffer](api_platformvm_locked.lockedids.md#tobuffer)

## Constructors

###  constructor

\+ **new LockedIDs**(`depositTxID?`: Buffer, `bondTxID?`: Buffer): *[LockedIDs](api_platformvm_locked.lockedids.md)*

*Defined in [src/apis/platformvm/locked.ts:62](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L62)*

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

*Defined in [src/apis/platformvm/locked.ts:49](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L49)*

___

### `Protected` depositTxID

• **depositTxID**: *[SerializableTxID](api_platformvm_locked.serializabletxid.md)* = new SerializableTxID()

*Defined in [src/apis/platformvm/locked.ts:48](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L48)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Defined in [src/apis/platformvm/locked.ts:43](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L43)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset?`: number): *number*

*Defined in [src/apis/platformvm/locked.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L51)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Defined in [src/apis/platformvm/locked.ts:35](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L35)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/locked.ts:57](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/locked.ts#L57)*

**Returns:** *Buffer*
