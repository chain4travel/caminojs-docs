[@c4tplatform/caminojs](../api.md) › [Common-Inputs](../modules/common_inputs.md) › [StandardTransferableInput](common_inputs.standardtransferableinput.md)

# Class: StandardTransferableInput

## Hierarchy

  ↳ [StandardParseableInput](common_inputs.standardparseableinput.md)

  ↳ **StandardTransferableInput**

  ↳ [TransferableInput](api_evm_inputs.transferableinput.md)

  ↳ [TransferableInput](api_avm_inputs.transferableinput.md)

  ↳ [TransferableInput](api_platformvm_inputs.transferableinput.md)

## Index

### Constructors

* [constructor](common_inputs.standardtransferableinput.md#constructor)

### Properties

* [_codecID](common_inputs.standardtransferableinput.md#protected-_codecid)
* [_typeID](common_inputs.standardtransferableinput.md#protected-_typeid)
* [_typeName](common_inputs.standardtransferableinput.md#protected-_typename)
* [assetID](common_inputs.standardtransferableinput.md#protected-assetid)
* [input](common_inputs.standardtransferableinput.md#protected-input)
* [outputidx](common_inputs.standardtransferableinput.md#protected-outputidx)
* [txid](common_inputs.standardtransferableinput.md#protected-txid)

### Methods

* [addSignatureIdx](common_inputs.standardtransferableinput.md#addsignatureidx)
* [deserialize](common_inputs.standardtransferableinput.md#deserialize)
* [fromBuffer](common_inputs.standardtransferableinput.md#abstract-frombuffer)
* [getAssetID](common_inputs.standardtransferableinput.md#getassetid)
* [getCodecID](common_inputs.standardtransferableinput.md#getcodecid)
* [getInput](common_inputs.standardtransferableinput.md#getinput)
* [getOutputIdx](common_inputs.standardtransferableinput.md#getoutputidx)
* [getSigIdxs](common_inputs.standardtransferableinput.md#getsigidxs)
* [getTxID](common_inputs.standardtransferableinput.md#gettxid)
* [getTypeID](common_inputs.standardtransferableinput.md#gettypeid)
* [getTypeName](common_inputs.standardtransferableinput.md#gettypename)
* [getUTXOID](common_inputs.standardtransferableinput.md#getutxoid)
* [sanitizeObject](common_inputs.standardtransferableinput.md#sanitizeobject)
* [serialize](common_inputs.standardtransferableinput.md#serialize)
* [toBuffer](common_inputs.standardtransferableinput.md#tobuffer)
* [toString](common_inputs.standardtransferableinput.md#tostring)
* [comparator](common_inputs.standardtransferableinput.md#static-comparator)

## Constructors

###  constructor

\+ **new StandardTransferableInput**(`txid`: Buffer, `outputidx`: Buffer, `assetID`: Buffer, `input`: [BaseInput](../interfaces/common_inputs.baseinput.md)): *[StandardTransferableInput](common_inputs.standardtransferableinput.md)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[constructor](common_inputs.standardparseableinput.md#constructor)*

*Defined in [src/common/input.ts:317](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L317)*

Class representing an [StandardTransferableInput](common_inputs.standardtransferableinput.md) for a transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`txid` | Buffer | undefined | A [Buffer](https://github.com/feross/buffer) containing the transaction ID of the referenced UTXO |
`outputidx` | Buffer | undefined | A [Buffer](https://github.com/feross/buffer) containing the index of the output in the transaction consumed in the [StandardTransferableInput](common_inputs.standardtransferableinput.md) |
`assetID` | Buffer | undefined | A [Buffer](https://github.com/feross/buffer) representing the assetID of the [Input](common_inputs.input.md) |
`input` | [BaseInput](../interfaces/common_inputs.baseinput.md) | undefined | An [Input](common_inputs.input.md) to be made transferable  |

**Returns:** *[StandardTransferableInput](common_inputs.standardtransferableinput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[_typeID](common_inputs.standardparseableinput.md#protected-_typeid)*

*Defined in [src/common/input.ts:217](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L217)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardTransferableInput"

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[_typeName](common_inputs.standardparseableinput.md#protected-_typename)*

*Defined in [src/common/input.ts:216](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L216)*

___

### `Protected` assetID

• **assetID**: *Buffer* = Buffer.alloc(32)

*Defined in [src/common/input.ts:261](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L261)*

___

### `Protected` input

• **input**: *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[input](common_inputs.standardparseableinput.md#protected-input)*

*Defined in [src/common/input.ts:167](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L167)*

___

### `Protected` outputidx

• **outputidx**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/input.ts:260](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L260)*

___

### `Protected` txid

• **txid**: *Buffer* = Buffer.alloc(32)

*Defined in [src/common/input.ts:259](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L259)*

## Methods

###  addSignatureIdx

▸ **addSignatureIdx**(`addressIdx`: number, `address`: Buffer): *void*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[addSignatureIdx](common_inputs.standardparseableinput.md#addsignatureidx)*

*Defined in [src/common/input.ts:185](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L185)*

**Parameters:**

Name | Type |
------ | ------ |
`addressIdx` | number |
`address` | Buffer |

**Returns:** *void*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/common/input.ts:233](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L233)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

### `Abstract` fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset?`: number): *number*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[fromBuffer](common_inputs.standardparseableinput.md#abstract-frombuffer)*

*Defined in [src/common/input.ts:289](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L289)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  getAssetID

▸ **getAssetID**(): *Buffer*

*Defined in [src/common/input.ts:287](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L287)*

Returns the assetID of the input.

**Returns:** *Buffer*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getInput

▸ **getInput**(): *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[getInput](common_inputs.standardparseableinput.md#getinput)*

*Defined in [src/common/input.ts:282](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L282)*

Returns the input.

**Returns:** *[BaseInput](../interfaces/common_inputs.baseinput.md)*

___

###  getOutputIdx

▸ **getOutputIdx**(): *Buffer*

*Defined in [src/common/input.ts:271](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L271)*

Returns a [Buffer](https://github.com/feross/buffer)  of the OutputIdx.

**Returns:** *Buffer*

___

###  getSigIdxs

▸ **getSigIdxs**(): *[SigIdx](common_signature.sigidx.md)[]*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[getSigIdxs](common_inputs.standardparseableinput.md#getsigidxs)*

*Defined in [src/common/input.ts:189](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L189)*

**Returns:** *[SigIdx](common_signature.sigidx.md)[]*

___

###  getTxID

▸ **getTxID**(): *Buffer*

*Defined in [src/common/input.ts:266](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L266)*

Returns a [Buffer](https://github.com/feross/buffer) of the TxID.

**Returns:** *Buffer*

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

###  getUTXOID

▸ **getUTXOID**(): *string*

*Defined in [src/common/input.ts:276](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L276)*

Returns a base-58 string representation of the UTXOID this [StandardTransferableInput](common_inputs.standardtransferableinput.md) references.

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

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[serialize](common_inputs.standardparseableinput.md#serialize)*

*Defined in [src/common/input.ts:219](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L219)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[toBuffer](common_inputs.standardparseableinput.md#tobuffer)*

*Defined in [src/common/input.ts:294](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L294)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [StandardTransferableInput](common_inputs.standardtransferableinput.md).

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Defined in [src/common/input.ts:314](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L314)*

Returns a base-58 representation of the [StandardTransferableInput](common_inputs.standardtransferableinput.md).

**Returns:** *string*

___

### `Static` comparator

▸ **comparator**(): *function*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[comparator](common_inputs.standardparseableinput.md#static-comparator)*

*Defined in [src/common/input.ts:172](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L172)*

Returns a function used to sort an array of [StandardParseableInput](common_inputs.standardparseableinput.md)s

**Returns:** *function*

▸ (`a`: [StandardParseableInput](common_inputs.standardparseableinput.md), `b`: [StandardParseableInput](common_inputs.standardparseableinput.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [StandardParseableInput](common_inputs.standardparseableinput.md) |
`b` | [StandardParseableInput](common_inputs.standardparseableinput.md) |
