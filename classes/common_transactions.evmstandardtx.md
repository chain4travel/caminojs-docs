[@c4tplatform/caminojs](../api.md) › [Common-Transactions](../modules/common_transactions.md) › [EVMStandardTx](common_transactions.evmstandardtx.md)

# Class: EVMStandardTx ‹**KPClass, KCClass, SUBTx**›

Class representing a signed transaction.

## Type parameters

▪ **KPClass**: *[SignerKeyPair](common_keychain.signerkeypair.md)*

▪ **KCClass**: *[SignerKeyChain](common_keychain.signerkeychain.md)*

▪ **SUBTx**: *[EVMStandardUnsignedTx](common_transactions.evmstandardunsignedtx.md)‹KPClass, KCClass, [EVMStandardBaseTx](common_transactions.evmstandardbasetx.md)‹KPClass, KCClass››*

## Hierarchy

* [Serializable](utils_serialization.serializable.md)

  ↳ **EVMStandardTx**

  ↳ [Tx](api_evm_transactions.tx.md)

## Index

### Constructors

* [constructor](common_transactions.evmstandardtx.md#constructor)

### Properties

* [_codecID](common_transactions.evmstandardtx.md#protected-_codecid)
* [_typeID](common_transactions.evmstandardtx.md#protected-_typeid)
* [_typeName](common_transactions.evmstandardtx.md#protected-_typename)
* [credentials](common_transactions.evmstandardtx.md#protected-credentials)
* [unsignedTx](common_transactions.evmstandardtx.md#protected-unsignedtx)

### Methods

* [deserialize](common_transactions.evmstandardtx.md#deserialize)
* [fromBuffer](common_transactions.evmstandardtx.md#abstract-frombuffer)
* [fromString](common_transactions.evmstandardtx.md#fromstring)
* [getCodecID](common_transactions.evmstandardtx.md#getcodecid)
* [getTypeID](common_transactions.evmstandardtx.md#gettypeid)
* [getTypeName](common_transactions.evmstandardtx.md#gettypename)
* [getUnsignedTx](common_transactions.evmstandardtx.md#getunsignedtx)
* [sanitizeObject](common_transactions.evmstandardtx.md#sanitizeobject)
* [serialize](common_transactions.evmstandardtx.md#serialize)
* [toBuffer](common_transactions.evmstandardtx.md#tobuffer)
* [toString](common_transactions.evmstandardtx.md#tostring)
* [toStringHex](common_transactions.evmstandardtx.md#tostringhex)

## Constructors

###  constructor

\+ **new EVMStandardTx**(`unsignedTx`: SUBTx, `credentials`: [Credential](common_signature.credential.md)[]): *[EVMStandardTx](common_transactions.evmstandardtx.md)*

*Defined in [src/common/evmtx.ts:387](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L387)*

Class representing a signed transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`unsignedTx` | SUBTx | undefined | Optional [StandardUnsignedTx](common_transactions.standardunsignedtx.md) |
`credentials` | [Credential](common_signature.credential.md)[] | undefined | - |

**Returns:** *[EVMStandardTx](common_transactions.evmstandardtx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Serializable](utils_serialization.serializable.md).[_typeID](utils_serialization.serializable.md#protected-_typeid)*

*Defined in [src/common/evmtx.ts:315](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L315)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardTx"

*Overrides [Serializable](utils_serialization.serializable.md).[_typeName](utils_serialization.serializable.md#protected-_typename)*

*Defined in [src/common/evmtx.ts:314](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L314)*

___

### `Protected` credentials

• **credentials**: *[Credential](common_signature.credential.md)[]* = []

*Defined in [src/common/evmtx.ts:327](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L327)*

___

### `Protected` unsignedTx

• **unsignedTx**: *SUBTx* = undefined

*Defined in [src/common/evmtx.ts:326](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L326)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding?`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/utils/serialization.ts:99](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L99)*

**Parameters:**

Name | Type |
------ | ------ |
`fields` | object |
`encoding?` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) |

**Returns:** *void*

___

### `Abstract` fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset?`: number): *number*

*Defined in [src/common/evmtx.ts:336](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L336)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  fromString

▸ **fromString**(`serialized`: string): *number*

*Defined in [src/common/evmtx.ts:371](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L371)*

Takes a base-58 string containing an [StandardTx](common_transactions.standardtx.md), parses it, populates the class, and returns the length of the Tx in bytes.

**`remarks`** 
unlike most fromStrings, it expects the string to be serialized in cb58 format

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`serialized` | string | A base-58 string containing a raw [StandardTx](common_transactions.standardtx.md)  |

**Returns:** *number*

The length of the raw [StandardTx](common_transactions.standardtx.md)

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

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

###  getUnsignedTx

▸ **getUnsignedTx**(): *SUBTx*

*Defined in [src/common/evmtx.ts:332](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L332)*

Returns the [StandardUnsignedTx](common_transactions.standardunsignedtx.md)

**Returns:** *SUBTx*

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

*Defined in [src/common/evmtx.ts:317](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L317)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/common/evmtx.ts:341](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L341)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [StandardTx](common_transactions.standardtx.md).

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Defined in [src/common/evmtx.ts:381](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L381)*

Returns a cb58 representation of the [StandardTx](common_transactions.standardtx.md).

**`remarks`** 
unlike most toStrings, this returns in cb58 serialization format

**Returns:** *string*

___

###  toStringHex

▸ **toStringHex**(): *string*

*Defined in [src/common/evmtx.ts:385](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/evmtx.ts#L385)*

**Returns:** *string*
