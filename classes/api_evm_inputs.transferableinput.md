[@c4tplatform/caminojs](../api.md) › [API-EVM-Inputs](../modules/api_evm_inputs.md) › [TransferableInput](api_evm_inputs.transferableinput.md)

# Class: TransferableInput

## Hierarchy

  ↳ [StandardTransferableInput](common_inputs.standardtransferableinput.md)

  ↳ **TransferableInput**

## Index

### Constructors

* [constructor](api_evm_inputs.transferableinput.md#constructor)

### Properties

* [_codecID](api_evm_inputs.transferableinput.md#protected-_codecid)
* [_typeID](api_evm_inputs.transferableinput.md#protected-_typeid)
* [_typeName](api_evm_inputs.transferableinput.md#protected-_typename)
* [assetID](api_evm_inputs.transferableinput.md#protected-assetid)
* [input](api_evm_inputs.transferableinput.md#protected-input)
* [outputidx](api_evm_inputs.transferableinput.md#protected-outputidx)
* [txid](api_evm_inputs.transferableinput.md#protected-txid)

### Methods

* [addSignatureIdx](api_evm_inputs.transferableinput.md#addsignatureidx)
* [deserialize](api_evm_inputs.transferableinput.md#deserialize)
* [fromBuffer](api_evm_inputs.transferableinput.md#frombuffer)
* [getAssetID](api_evm_inputs.transferableinput.md#getassetid)
* [getCodecID](api_evm_inputs.transferableinput.md#getcodecid)
* [getCost](api_evm_inputs.transferableinput.md#getcost)
* [getInput](api_evm_inputs.transferableinput.md#getinput)
* [getOutputIdx](api_evm_inputs.transferableinput.md#getoutputidx)
* [getSigIdxs](api_evm_inputs.transferableinput.md#getsigidxs)
* [getTxID](api_evm_inputs.transferableinput.md#gettxid)
* [getTypeID](api_evm_inputs.transferableinput.md#gettypeid)
* [getTypeName](api_evm_inputs.transferableinput.md#gettypename)
* [getUTXOID](api_evm_inputs.transferableinput.md#getutxoid)
* [sanitizeObject](api_evm_inputs.transferableinput.md#sanitizeobject)
* [serialize](api_evm_inputs.transferableinput.md#serialize)
* [toBuffer](api_evm_inputs.transferableinput.md#tobuffer)
* [toString](api_evm_inputs.transferableinput.md#tostring)
* [comparator](api_evm_inputs.transferableinput.md#static-comparator)

## Constructors

###  constructor

\+ **new TransferableInput**(`txid`: Buffer, `outputidx`: Buffer, `assetID`: Buffer, `input`: [BaseInput](../interfaces/common_inputs.baseinput.md)): *[TransferableInput](api_evm_inputs.transferableinput.md)*

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[constructor](common_inputs.standardtransferableinput.md#constructor)*

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

**Returns:** *[TransferableInput](api_evm_inputs.transferableinput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardTransferableInput](common_inputs.standardtransferableinput.md).[_typeID](common_inputs.standardtransferableinput.md#protected-_typeid)*

*Defined in [src/apis/evm/inputs.ts:42](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/inputs.ts#L42)*

___

### `Protected` _typeName

• **_typeName**: *string* = "TransferableInput"

*Overrides [StandardTransferableInput](common_inputs.standardtransferableinput.md).[_typeName](common_inputs.standardtransferableinput.md#protected-_typename)*

*Defined in [src/apis/evm/inputs.ts:41](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/inputs.ts#L41)*

___

### `Protected` assetID

• **assetID**: *Buffer* = Buffer.alloc(32)

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[assetID](common_inputs.standardtransferableinput.md#protected-assetid)*

*Defined in [src/common/input.ts:261](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L261)*

___

### `Protected` input

• **input**: *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[input](common_inputs.standardparseableinput.md#protected-input)*

*Defined in [src/common/input.ts:167](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L167)*

___

### `Protected` outputidx

• **outputidx**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[outputidx](common_inputs.standardtransferableinput.md#protected-outputidx)*

*Defined in [src/common/input.ts:260](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L260)*

___

### `Protected` txid

• **txid**: *Buffer* = Buffer.alloc(32)

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[txid](common_inputs.standardtransferableinput.md#protected-txid)*

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

*Overrides [StandardTransferableInput](common_inputs.standardtransferableinput.md).[deserialize](common_inputs.standardtransferableinput.md#deserialize)*

*Defined in [src/apis/evm/inputs.ts:46](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/inputs.ts#L46)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [StandardTransferableInput](common_inputs.standardtransferableinput.md).[fromBuffer](common_inputs.standardtransferableinput.md#abstract-frombuffer)*

*Defined in [src/apis/evm/inputs.ts:69](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/inputs.ts#L69)*

Takes a [Buffer](https://github.com/feross/buffer) containing a [TransferableInput](api_evm_inputs.transferableinput.md), parses it, populates the class, and returns the length of the [TransferableInput](api_evm_inputs.transferableinput.md) in bytes.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`bytes` | Buffer | - | A [Buffer](https://github.com/feross/buffer) containing a raw [TransferableInput](api_evm_inputs.transferableinput.md)  |
`offset` | number | 0 | - |

**Returns:** *number*

The length of the raw [TransferableInput](api_evm_inputs.transferableinput.md)

___

###  getAssetID

▸ **getAssetID**(): *Buffer*

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[getAssetID](common_inputs.standardtransferableinput.md#getassetid)*

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

###  getCost

▸ **getCost**(`c`: [C](../interfaces/utils_networks.c.md)): *number*

*Defined in [src/apis/evm/inputs.ts:57](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/inputs.ts#L57)*

Assesses the amount to be paid based on the number of signatures required

**Parameters:**

Name | Type |
------ | ------ |
`c` | [C](../interfaces/utils_networks.c.md) |

**Returns:** *number*

the amount to be paid

___

###  getInput

▸ **getInput**(): *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[getInput](common_inputs.standardtransferableinput.md#getinput)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[getInput](common_inputs.standardparseableinput.md#getinput)*

*Defined in [src/common/input.ts:282](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L282)*

Returns the input.

**Returns:** *[BaseInput](../interfaces/common_inputs.baseinput.md)*

___

###  getOutputIdx

▸ **getOutputIdx**(): *Buffer*

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[getOutputIdx](common_inputs.standardtransferableinput.md#getoutputidx)*

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

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[getTxID](common_inputs.standardtransferableinput.md#gettxid)*

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

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[getUTXOID](common_inputs.standardtransferableinput.md#getutxoid)*

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

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[serialize](common_inputs.standardtransferableinput.md#serialize)*

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

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[toBuffer](common_inputs.standardtransferableinput.md#tobuffer)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[toBuffer](common_inputs.standardparseableinput.md#tobuffer)*

*Defined in [src/common/input.ts:294](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L294)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [StandardTransferableInput](common_inputs.standardtransferableinput.md).

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [StandardTransferableInput](common_inputs.standardtransferableinput.md).[toString](common_inputs.standardtransferableinput.md#tostring)*

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
