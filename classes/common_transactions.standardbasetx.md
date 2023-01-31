[@c4tplatform/caminojs](../api.md) › [Common-Transactions](../modules/common_transactions.md) › [StandardBaseTx](common_transactions.standardbasetx.md)

# Class: StandardBaseTx ‹**KPClass, KCClass**›

Class representing a base for all transactions.

## Type parameters

▪ **KPClass**: *[StandardKeyPair](common_keychain.standardkeypair.md)*

▪ **KCClass**: *[StandardKeyChain](common_keychain.standardkeychain.md)‹KPClass›*

## Hierarchy

* [Serializable](utils_serialization.serializable.md)

  ↳ **StandardBaseTx**

  ↳ [BaseTx](api_avm_basetx.basetx.md)

  ↳ [BaseTx](api_platformvm_basetx.basetx.md)

## Index

### Constructors

* [constructor](common_transactions.standardbasetx.md#constructor)

### Properties

* [_codecID](common_transactions.standardbasetx.md#protected-_codecid)
* [_typeID](common_transactions.standardbasetx.md#protected-_typeid)
* [_typeName](common_transactions.standardbasetx.md#protected-_typename)
* [blockchainID](common_transactions.standardbasetx.md#protected-blockchainid)
* [ins](common_transactions.standardbasetx.md#protected-ins)
* [memo](common_transactions.standardbasetx.md#protected-memo)
* [networkID](common_transactions.standardbasetx.md#protected-networkid)
* [numins](common_transactions.standardbasetx.md#protected-numins)
* [numouts](common_transactions.standardbasetx.md#protected-numouts)
* [outs](common_transactions.standardbasetx.md#protected-outs)

### Methods

* [clone](common_transactions.standardbasetx.md#abstract-clone)
* [create](common_transactions.standardbasetx.md#abstract-create)
* [deserialize](common_transactions.standardbasetx.md#deserialize)
* [getBlockchainID](common_transactions.standardbasetx.md#getblockchainid)
* [getCodecID](common_transactions.standardbasetx.md#getcodecid)
* [getIns](common_transactions.standardbasetx.md#abstract-getins)
* [getMemo](common_transactions.standardbasetx.md#getmemo)
* [getNetworkID](common_transactions.standardbasetx.md#getnetworkid)
* [getOuts](common_transactions.standardbasetx.md#abstract-getouts)
* [getTotalOuts](common_transactions.standardbasetx.md#abstract-gettotalouts)
* [getTxType](common_transactions.standardbasetx.md#abstract-gettxtype)
* [getTypeID](common_transactions.standardbasetx.md#gettypeid)
* [getTypeName](common_transactions.standardbasetx.md#gettypename)
* [sanitizeObject](common_transactions.standardbasetx.md#sanitizeobject)
* [select](common_transactions.standardbasetx.md#abstract-select)
* [serialize](common_transactions.standardbasetx.md#serialize)
* [sign](common_transactions.standardbasetx.md#abstract-sign)
* [toBuffer](common_transactions.standardbasetx.md#tobuffer)
* [toString](common_transactions.standardbasetx.md#tostring)
* [toStringHex](common_transactions.standardbasetx.md#tostringhex)

## Constructors

###  constructor

\+ **new StandardBaseTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [StandardTransferableOutput](common_output.standardtransferableoutput.md)[], `ins`: [StandardTransferableInput](common_inputs.standardtransferableinput.md)[], `memo`: Buffer): *[StandardBaseTx](common_transactions.standardbasetx.md)*

*Defined in [src/common/tx.ts:192](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L192)*

Class representing a StandardBaseTx which is the foundation for all transactions.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Optional networkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | Buffer.alloc(32, 16) | Optional blockchainID, default Buffer.alloc(32, 16) |
`outs` | [StandardTransferableOutput](common_output.standardtransferableoutput.md)[] | undefined | Optional array of the [TransferableOutput](api_evm_outputs.transferableoutput.md)s |
`ins` | [StandardTransferableInput](common_inputs.standardtransferableinput.md)[] | undefined | Optional array of the [TransferableInput](api_evm_inputs.transferableinput.md)s |
`memo` | Buffer | undefined | Optional [Buffer](https://github.com/feross/buffer) for the memo field  |

**Returns:** *[StandardBaseTx](common_transactions.standardbasetx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Serializable](utils_serialization.serializable.md).[_typeID](utils_serialization.serializable.md#protected-_typeid)*

*Defined in [src/common/tx.ts:42](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L42)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardBaseTx"

*Overrides [Serializable](utils_serialization.serializable.md).[_typeName](utils_serialization.serializable.md#protected-_typename)*

*Defined in [src/common/tx.ts:41](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L41)*

___

### `Protected` blockchainID

• **blockchainID**: *Buffer* = Buffer.alloc(32)

*Defined in [src/common/tx.ts:86](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L86)*

___

### `Protected` ins

• **ins**: *[StandardTransferableInput](common_inputs.standardtransferableinput.md)[]*

*Defined in [src/common/tx.ts:90](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L90)*

___

### `Protected` memo

• **memo**: *Buffer* = Buffer.alloc(0)

*Defined in [src/common/tx.ts:91](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L91)*

___

### `Protected` networkID

• **networkID**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/tx.ts:85](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L85)*

___

### `Protected` numins

• **numins**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/tx.ts:89](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L89)*

___

### `Protected` numouts

• **numouts**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/tx.ts:87](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L87)*

___

### `Protected` outs

• **outs**: *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

*Defined in [src/common/tx.ts:88](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L88)*

## Methods

### `Abstract` clone

▸ **clone**(): *this*

*Defined in [src/common/tx.ts:188](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L188)*

**Returns:** *this*

___

### `Abstract` create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/common/tx.ts:190](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L190)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/common/tx.ts:66](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L66)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  getBlockchainID

▸ **getBlockchainID**(): *Buffer*

*Defined in [src/common/tx.ts:108](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L108)*

Returns the Buffer representation of the BlockchainID

**Returns:** *Buffer*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

### `Abstract` getIns

▸ **getIns**(): *[StandardTransferableInput](common_inputs.standardtransferableinput.md)[]*

*Defined in [src/common/tx.ts:115](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L115)*

Returns the array of [StandardTransferableInput](common_inputs.standardtransferableinput.md)s

**Returns:** *[StandardTransferableInput](common_inputs.standardtransferableinput.md)[]*

___

###  getMemo

▸ **getMemo**(): *Buffer*

*Defined in [src/common/tx.ts:130](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L130)*

Returns the [Buffer](https://github.com/feross/buffer) representation of the memo

**Returns:** *Buffer*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Defined in [src/common/tx.ts:101](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L101)*

Returns the NetworkID as a number

**Returns:** *number*

___

### `Abstract` getOuts

▸ **getOuts**(): *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

*Defined in [src/common/tx.ts:120](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L120)*

Returns the array of [StandardTransferableOutput](../modules/src_common.md#standardtransferableoutput)s

**Returns:** *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

___

### `Abstract` getTotalOuts

▸ **getTotalOuts**(): *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

*Defined in [src/common/tx.ts:125](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L125)*

Returns the array of combined total [StandardTransferableOutput](../modules/src_common.md#standardtransferableoutput)s

**Returns:** *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

___

### `Abstract` getTxType

▸ **getTxType**(): *number*

*Defined in [src/common/tx.ts:96](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L96)*

Returns the id of the [StandardBaseTx](common_transactions.standardbasetx.md)

**Returns:** *number*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeID](common_signature.sigidx.md#gettypeid)*

*Defined in [src/utils/serialization.ts:63](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L63)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getTypeName

▸ **getTypeName**(): *string*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeName](common_signature.sigidx.md#gettypename)*

*Defined in [src/utils/serialization.ts:56](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L56)*

Used in serialization. TypeName is a string name for the type of object being output.

**Returns:** *string*

___

###  sanitizeObject

▸ **sanitizeObject**(`obj`: object): *object*

*Inherited from [SigIdx](common_signature.sigidx.md).[sanitizeObject](common_signature.sigidx.md#sanitizeobject)*

*Defined in [src/utils/serialization.ts:77](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L77)*

Sanitize to prevent cross scripting attacks.

**Parameters:**

Name | Type |
------ | ------ |
`obj` | object |

**Returns:** *object*

___

### `Abstract` select

▸ **select**(`id`: number, ...`args`: any[]): *this*

*Defined in [src/common/tx.ts:192](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L192)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *this*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/tx.ts:44](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L44)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

### `Abstract` sign

▸ **sign**(`msg`: Buffer, `kc`: [StandardKeyChain](common_keychain.standardkeychain.md)‹KPClass›): *[Credential](common_signature.credential.md)[]*

*Defined in [src/common/tx.ts:186](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L186)*

Takes the bytes of an [UnsignedTx](api_evm_transactions.unsignedtx.md) and returns an array of [Credential](common_signature.credential.md)s

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | A Buffer for the [UnsignedTx](api_evm_transactions.unsignedtx.md) |
`kc` | [StandardKeyChain](common_keychain.standardkeychain.md)‹KPClass› | An [KeyChain](api_evm_keychain.keychain.md) used in signing  |

**Returns:** *[Credential](common_signature.credential.md)[]*

An array of [Credential](common_signature.credential.md)s

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/common/tx.ts:137](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L137)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [StandardBaseTx](common_transactions.standardbasetx.md).

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Defined in [src/common/tx.ts:170](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L170)*

Returns a base-58 representation of the [StandardBaseTx](common_transactions.standardbasetx.md).

**Returns:** *string*

___

###  toStringHex

▸ **toStringHex**(): *string*

*Defined in [src/common/tx.ts:174](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/tx.ts#L174)*

**Returns:** *string*
