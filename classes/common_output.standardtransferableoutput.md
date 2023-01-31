[@c4tplatform/caminojs](../README.md) › [Common-Output](../modules/common_output.md) › [StandardTransferableOutput](common_output.standardtransferableoutput.md)

# Class: StandardTransferableOutput

## Hierarchy

  ↳ [StandardParseableOutput](common_output.standardparseableoutput.md)

  ↳ **StandardTransferableOutput**

  ↳ [TransferableOutput](api_evm_outputs.transferableoutput.md)

  ↳ [TransferableOutput](api_avm_outputs.transferableoutput.md)

  ↳ [TransferableOutput](api_platformvm_outputs.transferableoutput.md)

## Index

### Constructors

* [constructor](common_output.standardtransferableoutput.md#constructor)

### Properties

* [_codecID](common_output.standardtransferableoutput.md#protected-_codecid)
* [_typeID](common_output.standardtransferableoutput.md#protected-_typeid)
* [_typeName](common_output.standardtransferableoutput.md#protected-_typename)
* [assetID](common_output.standardtransferableoutput.md#protected-assetid)
* [output](common_output.standardtransferableoutput.md#protected-output)

### Methods

* [deserialize](common_output.standardtransferableoutput.md#deserialize)
* [fromBuffer](common_output.standardtransferableoutput.md#abstract-frombuffer)
* [getAddresses](common_output.standardtransferableoutput.md#getaddresses)
* [getAssetID](common_output.standardtransferableoutput.md#getassetid)
* [getCodecID](common_output.standardtransferableoutput.md#getcodecid)
* [getLocktime](common_output.standardtransferableoutput.md#getlocktime)
* [getOutput](common_output.standardtransferableoutput.md#getoutput)
* [getThreshold](common_output.standardtransferableoutput.md#getthreshold)
* [getTypeID](common_output.standardtransferableoutput.md#gettypeid)
* [getTypeName](common_output.standardtransferableoutput.md#gettypename)
* [meetsThreshold](common_output.standardtransferableoutput.md#meetsthreshold)
* [sanitizeObject](common_output.standardtransferableoutput.md#sanitizeobject)
* [serialize](common_output.standardtransferableoutput.md#serialize)
* [toBuffer](common_output.standardtransferableoutput.md#tobuffer)
* [comparator](common_output.standardtransferableoutput.md#static-comparator)

## Constructors

###  constructor

\+ **new StandardTransferableOutput**(`assetID`: Buffer, `output`: [BaseOutput](../interfaces/common_output.baseoutput.md)): *[StandardTransferableOutput](common_output.standardtransferableoutput.md)*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[constructor](common_output.standardparseableoutput.md#constructor)*

*Defined in [src/common/output.ts:514](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L514)*

Class representing an [StandardTransferableOutput](common_output.standardtransferableoutput.md) for a transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`assetID` | Buffer | undefined | A [Buffer](https://github.com/feross/buffer) representing the assetID of the [Output](common_output.output.md) |
`output` | [BaseOutput](../interfaces/common_output.baseoutput.md) | undefined | A number representing the InputID of the [StandardTransferableOutput](common_output.standardtransferableoutput.md)  |

**Returns:** *[StandardTransferableOutput](common_output.standardtransferableoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[_typeID](common_output.standardparseableoutput.md#protected-_typeid)*

*Defined in [src/common/output.ts:483](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L483)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardTransferableOutput"

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[_typeName](common_output.standardparseableoutput.md#protected-_typename)*

*Defined in [src/common/output.ts:482](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L482)*

___

### `Protected` assetID

• **assetID**: *Buffer* = undefined

*Defined in [src/common/output.ts:503](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L503)*

___

### `Protected` output

• **output**: *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[output](common_output.standardparseableoutput.md#protected-output)*

*Defined in [src/common/output.ts:427](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L427)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/common/output.ts:492](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L492)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

### `Abstract` fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset?`: number): *number*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[fromBuffer](common_output.standardparseableoutput.md#abstract-frombuffer)*

*Defined in [src/common/output.ts:508](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L508)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getAddresses](common_output.standardparseableoutput.md#getaddresses)*

*Defined in [src/common/output.ts:460](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L460)*

**Returns:** *Buffer[]*

___

###  getAssetID

▸ **getAssetID**(): *Buffer*

*Defined in [src/common/output.ts:505](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L505)*

**Returns:** *Buffer*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getLocktime

▸ **getLocktime**(): *BN*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getLocktime](common_output.standardparseableoutput.md#getlocktime)*

*Defined in [src/common/output.ts:457](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L457)*

**Returns:** *BN*

___

###  getOutput

▸ **getOutput**(): *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getOutput](common_output.standardparseableoutput.md#getoutput)*

*Defined in [src/common/output.ts:468](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L468)*

**Returns:** *[BaseOutput](../interfaces/common_output.baseoutput.md)*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getThreshold](common_output.standardparseableoutput.md#getthreshold)*

*Defined in [src/common/output.ts:454](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L454)*

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

###  meetsThreshold

▸ **meetsThreshold**(`addrs`: Buffer[], `asOf`: BN): *boolean*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[meetsThreshold](common_output.standardparseableoutput.md#meetsthreshold)*

*Defined in [src/common/output.ts:464](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L464)*

**Parameters:**

Name | Type |
------ | ------ |
`addrs` | Buffer[] |
`asOf` | BN |

**Returns:** *boolean*

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

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[serialize](common_output.standardparseableoutput.md#serialize)*

*Defined in [src/common/output.ts:485](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L485)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[toBuffer](common_output.standardparseableoutput.md#tobuffer)*

*Defined in [src/common/output.ts:510](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L510)*

**Returns:** *Buffer*

___

### `Static` comparator

▸ **comparator**(): *function*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[comparator](common_output.standardparseableoutput.md#static-comparator)*

*Defined in [src/common/output.ts:432](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L432)*

Returns a function used to sort an array of [ParseableOutput](api_platformvm_outputs.parseableoutput.md)s

**Returns:** *function*

▸ (`a`: [StandardParseableOutput](common_output.standardparseableoutput.md), `b`: [StandardParseableOutput](common_output.standardparseableoutput.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [StandardParseableOutput](common_output.standardparseableoutput.md) |
`b` | [StandardParseableOutput](common_output.standardparseableoutput.md) |
