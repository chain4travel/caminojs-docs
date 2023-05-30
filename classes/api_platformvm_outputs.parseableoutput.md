[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Outputs](../modules/api_platformvm_outputs.md) › [ParseableOutput](api_platformvm_outputs.parseableoutput.md)

# Class: ParseableOutput

## Hierarchy

  ↳ [StandardParseableOutput](common_output.standardparseableoutput.md)

  ↳ **ParseableOutput**

  ↳ [StakeableLockOut](api_platformvm_outputs.stakeablelockout.md)

  ↳ [LockedOut](api_platformvm_outputs.lockedout.md)

## Index

### Constructors

* [constructor](api_platformvm_outputs.parseableoutput.md#constructor)

### Properties

* [_codecID](api_platformvm_outputs.parseableoutput.md#protected-_codecid)
* [_typeID](api_platformvm_outputs.parseableoutput.md#protected-_typeid)
* [_typeName](api_platformvm_outputs.parseableoutput.md#protected-_typename)
* [output](api_platformvm_outputs.parseableoutput.md#protected-output)

### Methods

* [deserialize](api_platformvm_outputs.parseableoutput.md#deserialize)
* [fromBuffer](api_platformvm_outputs.parseableoutput.md#frombuffer)
* [getAddresses](api_platformvm_outputs.parseableoutput.md#getaddresses)
* [getCodecID](api_platformvm_outputs.parseableoutput.md#getcodecid)
* [getLocktime](api_platformvm_outputs.parseableoutput.md#getlocktime)
* [getOutput](api_platformvm_outputs.parseableoutput.md#getoutput)
* [getThreshold](api_platformvm_outputs.parseableoutput.md#getthreshold)
* [getTypeID](api_platformvm_outputs.parseableoutput.md#gettypeid)
* [getTypeName](api_platformvm_outputs.parseableoutput.md#gettypename)
* [meetsThreshold](api_platformvm_outputs.parseableoutput.md#meetsthreshold)
* [sanitizeObject](api_platformvm_outputs.parseableoutput.md#sanitizeobject)
* [serialize](api_platformvm_outputs.parseableoutput.md#serialize)
* [toBuffer](api_platformvm_outputs.parseableoutput.md#tobuffer)
* [comparator](api_platformvm_outputs.parseableoutput.md#static-comparator)

## Constructors

###  constructor

\+ **new ParseableOutput**(`output`: [BaseOutput](../interfaces/common_output.baseoutput.md)): *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[constructor](common_output.standardparseableoutput.md#constructor)*

*Defined in [src/common/output.ts:498](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L498)*

Class representing an [ParseableOutput](api_platformvm_outputs.parseableoutput.md) for a transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`output` | [BaseOutput](../interfaces/common_output.baseoutput.md) | undefined | A number representing the InputID of the [ParseableOutput](api_platformvm_outputs.parseableoutput.md)  |

**Returns:** *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[_typeID](common_output.standardparseableoutput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/outputs.ts:90](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L90)*

___

### `Protected` _typeName

• **_typeName**: *string* = "ParseableOutput"

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[_typeName](common_output.standardparseableoutput.md#protected-_typename)*

*Defined in [src/apis/platformvm/outputs.ts:89](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L89)*

___

### `Protected` output

• **output**: *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[output](common_output.standardparseableoutput.md#protected-output)*

*Defined in [src/common/output.ts:457](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L457)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/apis/platformvm/outputs.ts:94](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L94)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[fromBuffer](common_output.standardparseableoutput.md#abstract-frombuffer)*

*Defined in [src/apis/platformvm/outputs.ts:100](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L100)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getAddresses](common_output.standardparseableoutput.md#getaddresses)*

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

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getLocktime](common_output.standardparseableoutput.md#getlocktime)*

*Defined in [src/common/output.ts:487](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L487)*

**Returns:** *BN*

___

###  getOutput

▸ **getOutput**(): *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getOutput](common_output.standardparseableoutput.md#getoutput)*

*Defined in [src/common/output.ts:498](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L498)*

**Returns:** *[BaseOutput](../interfaces/common_output.baseoutput.md)*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getThreshold](common_output.standardparseableoutput.md#getthreshold)*

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

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[meetsThreshold](common_output.standardparseableoutput.md#meetsthreshold)*

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

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[serialize](common_output.standardparseableoutput.md#serialize)*

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

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[toBuffer](common_output.standardparseableoutput.md#tobuffer)*

*Defined in [src/common/output.ts:476](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L476)*

**Returns:** *Buffer*

___

### `Static` comparator

▸ **comparator**(): *function*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[comparator](common_output.standardparseableoutput.md#static-comparator)*

*Defined in [src/common/output.ts:462](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L462)*

Returns a function used to sort an array of [ParseableOutput](api_platformvm_outputs.parseableoutput.md)s

**Returns:** *function*

▸ (`a`: [StandardParseableOutput](common_output.standardparseableoutput.md), `b`: [StandardParseableOutput](common_output.standardparseableoutput.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [StandardParseableOutput](common_output.standardparseableoutput.md) |
`b` | [StandardParseableOutput](common_output.standardparseableoutput.md) |
