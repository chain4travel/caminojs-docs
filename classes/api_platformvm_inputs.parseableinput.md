[@c4tplatform/caminojs](../README.md) › [API-PlatformVM-Inputs](../modules/api_platformvm_inputs.md) › [ParseableInput](api_platformvm_inputs.parseableinput.md)

# Class: ParseableInput

## Hierarchy

  ↳ [StandardParseableInput](common_inputs.standardparseableinput.md)

  ↳ **ParseableInput**

  ↳ [StakeableLockIn](api_platformvm_inputs.stakeablelockin.md)

  ↳ [LockedIn](api_platformvm_inputs.lockedin.md)

## Index

### Constructors

* [constructor](api_platformvm_inputs.parseableinput.md#constructor)

### Properties

* [_codecID](api_platformvm_inputs.parseableinput.md#protected-_codecid)
* [_typeID](api_platformvm_inputs.parseableinput.md#protected-_typeid)
* [_typeName](api_platformvm_inputs.parseableinput.md#protected-_typename)
* [input](api_platformvm_inputs.parseableinput.md#protected-input)

### Methods

* [addSignatureIdx](api_platformvm_inputs.parseableinput.md#addsignatureidx)
* [deserialize](api_platformvm_inputs.parseableinput.md#deserialize)
* [fromBuffer](api_platformvm_inputs.parseableinput.md#frombuffer)
* [getCodecID](api_platformvm_inputs.parseableinput.md#getcodecid)
* [getInput](api_platformvm_inputs.parseableinput.md#getinput)
* [getSigIdxs](api_platformvm_inputs.parseableinput.md#getsigidxs)
* [getTypeID](api_platformvm_inputs.parseableinput.md#gettypeid)
* [getTypeName](api_platformvm_inputs.parseableinput.md#gettypename)
* [sanitizeObject](api_platformvm_inputs.parseableinput.md#sanitizeobject)
* [serialize](api_platformvm_inputs.parseableinput.md#serialize)
* [toBuffer](api_platformvm_inputs.parseableinput.md#tobuffer)
* [comparator](api_platformvm_inputs.parseableinput.md#static-comparator)

## Constructors

###  constructor

\+ **new ParseableInput**(`input`: [BaseInput](../interfaces/common_inputs.baseinput.md)): *[ParseableInput](api_platformvm_inputs.parseableinput.md)*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[constructor](common_inputs.standardparseableinput.md#constructor)*

*Defined in [src/common/input.ts:202](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L202)*

Class representing an [StandardParseableInput](common_inputs.standardparseableinput.md) for a transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`input` | [BaseInput](../interfaces/common_inputs.baseinput.md) | undefined | A number representing the InputID of the [StandardParseableInput](common_inputs.standardparseableinput.md)  |

**Returns:** *[ParseableInput](api_platformvm_inputs.parseableinput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[_typeID](common_inputs.standardparseableinput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/inputs.ts:49](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L49)*

___

### `Protected` _typeName

• **_typeName**: *string* = "ParseableInput"

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[_typeName](common_inputs.standardparseableinput.md#protected-_typename)*

*Defined in [src/apis/platformvm/inputs.ts:48](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L48)*

___

### `Protected` input

• **input**: *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[input](common_inputs.standardparseableinput.md#protected-input)*

*Defined in [src/common/input.ts:167](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L167)*

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

*Defined in [src/apis/platformvm/inputs.ts:52](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L52)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[fromBuffer](common_inputs.standardparseableinput.md#abstract-frombuffer)*

*Defined in [src/apis/platformvm/inputs.ts:58](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L58)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

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

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[getInput](common_inputs.standardparseableinput.md#getinput)*

*Defined in [src/common/input.ts:183](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L183)*

**Returns:** *[BaseInput](../interfaces/common_inputs.baseinput.md)*

___

###  getSigIdxs

▸ **getSigIdxs**(): *[SigIdx](common_signature.sigidx.md)[]*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[getSigIdxs](common_inputs.standardparseableinput.md#getsigidxs)*

*Defined in [src/common/input.ts:189](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L189)*

**Returns:** *[SigIdx](common_signature.sigidx.md)[]*

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

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[serialize](common_inputs.standardparseableinput.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/input.ts:159](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L159)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[toBuffer](common_inputs.standardparseableinput.md#tobuffer)*

*Defined in [src/common/input.ts:196](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L196)*

**Returns:** *Buffer*

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
