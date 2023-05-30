[@c4tplatform/caminojs](../api.md) › [Common-Output](../modules/common_output.md) › [StandardParseableOutput](common_output.standardparseableoutput.md)

# Class: StandardParseableOutput

## Hierarchy

* [Serializable](utils_serialization.serializable.md)

  ↳ **StandardParseableOutput**

  ↳ [StandardTransferableOutput](common_output.standardtransferableoutput.md)

  ↳ [ParseableOutput](api_platformvm_outputs.parseableoutput.md)

## Index

### Constructors

* [constructor](common_output.standardparseableoutput.md#constructor)

### Properties

* [_codecID](common_output.standardparseableoutput.md#protected-_codecid)
* [_typeID](common_output.standardparseableoutput.md#protected-_typeid)
* [_typeName](common_output.standardparseableoutput.md#protected-_typename)
* [output](common_output.standardparseableoutput.md#protected-output)

### Methods

* [deserialize](common_output.standardparseableoutput.md#deserialize)
* [fromBuffer](common_output.standardparseableoutput.md#abstract-frombuffer)
* [getAddresses](common_output.standardparseableoutput.md#getaddresses)
* [getCodecID](common_output.standardparseableoutput.md#getcodecid)
* [getLocktime](common_output.standardparseableoutput.md#getlocktime)
* [getOutput](common_output.standardparseableoutput.md#getoutput)
* [getThreshold](common_output.standardparseableoutput.md#getthreshold)
* [getTypeID](common_output.standardparseableoutput.md#gettypeid)
* [getTypeName](common_output.standardparseableoutput.md#gettypename)
* [meetsThreshold](common_output.standardparseableoutput.md#meetsthreshold)
* [sanitizeObject](common_output.standardparseableoutput.md#sanitizeobject)
* [serialize](common_output.standardparseableoutput.md#serialize)
* [toBuffer](common_output.standardparseableoutput.md#tobuffer)
* [comparator](common_output.standardparseableoutput.md#static-comparator)

## Constructors

###  constructor

\+ **new StandardParseableOutput**(`output`: [BaseOutput](../interfaces/common_output.baseoutput.md)): *[StandardParseableOutput](common_output.standardparseableoutput.md)*

*Defined in [src/common/output.ts:498](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L498)*

Class representing an [ParseableOutput](api_platformvm_outputs.parseableoutput.md) for a transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`output` | [BaseOutput](../interfaces/common_output.baseoutput.md) | undefined | A number representing the InputID of the [ParseableOutput](api_platformvm_outputs.parseableoutput.md)  |

**Returns:** *[StandardParseableOutput](common_output.standardparseableoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Serializable](utils_serialization.serializable.md).[_typeID](utils_serialization.serializable.md#protected-_typeid)*

*Defined in [src/common/output.ts:447](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L447)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardParseableOutput"

*Overrides [Serializable](utils_serialization.serializable.md).[_typeName](utils_serialization.serializable.md#protected-_typename)*

*Defined in [src/common/output.ts:446](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L446)*

___

### `Protected` output

• **output**: *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Defined in [src/common/output.ts:457](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L457)*

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

*Defined in [src/common/output.ts:474](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L474)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset?` | number |

**Returns:** *number*

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Defined in [src/common/output.ts:490](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L490)*

**Returns:** *Buffer[]*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getLocktime

▸ **getLocktime**(): *BN*

*Defined in [src/common/output.ts:487](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L487)*

**Returns:** *BN*

___

###  getOutput

▸ **getOutput**(): *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Defined in [src/common/output.ts:498](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L498)*

**Returns:** *[BaseOutput](../interfaces/common_output.baseoutput.md)*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Defined in [src/common/output.ts:484](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L484)*

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

###  meetsThreshold

▸ **meetsThreshold**(`addrs`: Buffer[], `asOf`: BN): *boolean*

*Defined in [src/common/output.ts:494](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L494)*

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

*Defined in [src/common/output.ts:449](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L449)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/common/output.ts:476](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L476)*

**Returns:** *Buffer*

___

### `Static` comparator

▸ **comparator**(): *function*

*Defined in [src/common/output.ts:462](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L462)*

Returns a function used to sort an array of [ParseableOutput](api_platformvm_outputs.parseableoutput.md)s

**Returns:** *function*

▸ (`a`: [StandardParseableOutput](common_output.standardparseableoutput.md), `b`: [StandardParseableOutput](common_output.standardparseableoutput.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [StandardParseableOutput](common_output.standardparseableoutput.md) |
`b` | [StandardParseableOutput](common_output.standardparseableoutput.md) |
