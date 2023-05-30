[@c4tplatform/caminojs](../api.md) › [Common-Transactions](../modules/common_transactions.md) › [StandardUnsignedTx](common_transactions.standardunsignedtx.md)

# Class: StandardUnsignedTx ‹**KPClass, KCClass, SBTx**›

Class representing an unsigned transaction.

## Type parameters

▪ **KPClass**: *[SignerKeyPair](common_keychain.signerkeypair.md)*

▪ **KCClass**: *[SignerKeyChain](common_keychain.signerkeychain.md)*

▪ **SBTx**: *[StandardBaseTx](common_transactions.standardbasetx.md)‹KPClass, KCClass›*

## Hierarchy

* [Serializable](utils_serialization.serializable.md)

  ↳ **StandardUnsignedTx**

  ↳ [UnsignedTx](api_avm_transactions.unsignedtx.md)

  ↳ [UnsignedTx](api_platformvm_transactions.unsignedtx.md)

## Index

### Constructors

* [constructor](common_transactions.standardunsignedtx.md#constructor)

### Properties

* [_codecID](common_transactions.standardunsignedtx.md#protected-_codecid)
* [_typeID](common_transactions.standardunsignedtx.md#protected-_typeid)
* [_typeName](common_transactions.standardunsignedtx.md#protected-_typename)
* [codecID](common_transactions.standardunsignedtx.md#protected-codecid)
* [transaction](common_transactions.standardunsignedtx.md#protected-transaction)

### Methods

* [deserialize](common_transactions.standardunsignedtx.md#deserialize)
* [fromBuffer](common_transactions.standardunsignedtx.md#abstract-frombuffer)
* [getBurn](common_transactions.standardunsignedtx.md#getburn)
* [getCodecID](common_transactions.standardunsignedtx.md#getcodecid)
* [getCodecIDBuffer](common_transactions.standardunsignedtx.md#getcodecidbuffer)
* [getInputTotal](common_transactions.standardunsignedtx.md#getinputtotal)
* [getOutputTotal](common_transactions.standardunsignedtx.md#getoutputtotal)
* [getTransaction](common_transactions.standardunsignedtx.md#abstract-gettransaction)
* [getTypeID](common_transactions.standardunsignedtx.md#gettypeid)
* [getTypeName](common_transactions.standardunsignedtx.md#gettypename)
* [sanitizeObject](common_transactions.standardunsignedtx.md#sanitizeobject)
* [serialize](common_transactions.standardunsignedtx.md#serialize)
* [sign](common_transactions.standardunsignedtx.md#abstract-sign)
* [toBuffer](common_transactions.standardunsignedtx.md#tobuffer)

## Constructors

###  constructor

\+ **new StandardUnsignedTx**(`transaction`: SBTx, `codecID`: number): *[StandardUnsignedTx](common_transactions.standardunsignedtx.md)*

*Defined in [src/common/tx.ts:363](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L363)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`transaction` | SBTx | undefined |
`codecID` | number | 0 |

**Returns:** *[StandardUnsignedTx](common_transactions.standardunsignedtx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Serializable](utils_serialization.serializable.md).[_typeID](utils_serialization.serializable.md#protected-_typeid)*

*Defined in [src/common/tx.ts:235](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L235)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardUnsignedTx"

*Overrides [Serializable](utils_serialization.serializable.md).[_typeName](utils_serialization.serializable.md#protected-_typename)*

*Defined in [src/common/tx.ts:234](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L234)*

___

### `Protected` codecID

• **codecID**: *number* = 0

*Defined in [src/common/tx.ts:262](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L262)*

___

### `Protected` transaction

• **transaction**: *SBTx*

*Defined in [src/common/tx.ts:263](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L263)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/common/tx.ts:252](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L252)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

### `Abstract` fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset?`: number): *number*

*Defined in [src/common/tx.ts:340](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L340)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  getBurn

▸ **getBurn**(`assetID`: Buffer): *BN*

*Defined in [src/common/tx.ts:331](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L331)*

Returns the number of burned tokens as a BN

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |

**Returns:** *BN*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Overrides [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/common/tx.ts:268](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L268)*

Returns the CodecID as a number

**Returns:** *number*

___

###  getCodecIDBuffer

▸ **getCodecIDBuffer**(): *Buffer*

*Defined in [src/common/tx.ts:275](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L275)*

Returns the [Buffer](https://github.com/feross/buffer) representation of the CodecID

**Returns:** *Buffer*

___

###  getInputTotal

▸ **getInputTotal**(`assetID`: Buffer): *BN*

*Defined in [src/common/tx.ts:284](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L284)*

Returns the inputTotal as a BN

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |

**Returns:** *BN*

___

###  getOutputTotal

▸ **getOutputTotal**(`assetID`: Buffer): *BN*

*Defined in [src/common/tx.ts:307](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L307)*

Returns the outputTotal as a BN

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |

**Returns:** *BN*

___

### `Abstract` getTransaction

▸ **getTransaction**(): *SBTx*

*Defined in [src/common/tx.ts:338](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L338)*

Returns the Transaction

**Returns:** *SBTx*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeID](common_signature.sigidx.md#gettypeid)*

*Defined in [src/utils/serialization.ts:63](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L63)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getTypeName

▸ **getTypeName**(): *string*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeName](common_signature.sigidx.md#gettypename)*

*Defined in [src/utils/serialization.ts:56](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L56)*

Used in serialization. TypeName is a string name for the type of object being output.

**Returns:** *string*

___

###  sanitizeObject

▸ **sanitizeObject**(`obj`: object): *object*

*Inherited from [SigIdx](common_signature.sigidx.md).[sanitizeObject](common_signature.sigidx.md#sanitizeobject)*

*Defined in [src/utils/serialization.ts:77](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L77)*

Sanitize to prevent cross scripting attacks.

**Parameters:**

Name | Type |
------ | ------ |
`obj` | object |

**Returns:** *object*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/tx.ts:237](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L237)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

### `Abstract` sign

▸ **sign**(`kc`: KCClass): *[StandardTx](common_transactions.standardtx.md)‹KPClass, KCClass, [StandardUnsignedTx](common_transactions.standardunsignedtx.md)‹KPClass, KCClass, SBTx››*

*Defined in [src/common/tx.ts:361](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L361)*

Signs this [UnsignedTx](api_evm_transactions.unsignedtx.md) and returns signed [StandardTx](common_transactions.standardtx.md)

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`kc` | KCClass | An [KeyChain](api_evm_keychain.keychain.md) used in signing  |

**Returns:** *[StandardTx](common_transactions.standardtx.md)‹KPClass, KCClass, [StandardUnsignedTx](common_transactions.standardunsignedtx.md)‹KPClass, KCClass, SBTx››*

A signed [StandardTx](common_transactions.standardtx.md)

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/common/tx.ts:342](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L342)*

**Returns:** *Buffer*
