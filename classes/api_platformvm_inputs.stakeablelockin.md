[@c4tplatform/caminojs](../README.md) › [API-PlatformVM-Inputs](../modules/api_platformvm_inputs.md) › [StakeableLockIn](api_platformvm_inputs.stakeablelockin.md)

# Class: StakeableLockIn

An [Input](common_inputs.input.md) class which specifies an input that has a locktime which can also
enable staking of the value held, preventing transfers but not validation.

## Hierarchy

  ↳ [ParseableInput](api_platformvm_inputs.parseableinput.md)

  ↳ **StakeableLockIn**

## Index

### Constructors

* [constructor](api_platformvm_inputs.stakeablelockin.md#constructor)

### Properties

* [_codecID](api_platformvm_inputs.stakeablelockin.md#protected-_codecid)
* [_typeID](api_platformvm_inputs.stakeablelockin.md#protected-_typeid)
* [_typeName](api_platformvm_inputs.stakeablelockin.md#protected-_typename)
* [input](api_platformvm_inputs.stakeablelockin.md#protected-input)
* [stakeableLocktime](api_platformvm_inputs.stakeablelockin.md#protected-stakeablelocktime)

### Methods

* [addSignatureIdx](api_platformvm_inputs.stakeablelockin.md#addsignatureidx)
* [clone](api_platformvm_inputs.stakeablelockin.md#clone)
* [create](api_platformvm_inputs.stakeablelockin.md#create)
* [deserialize](api_platformvm_inputs.stakeablelockin.md#deserialize)
* [fromBuffer](api_platformvm_inputs.stakeablelockin.md#frombuffer)
* [getAmount](api_platformvm_inputs.stakeablelockin.md#getamount)
* [getCodecID](api_platformvm_inputs.stakeablelockin.md#getcodecid)
* [getCredentialID](api_platformvm_inputs.stakeablelockin.md#getcredentialid)
* [getInput](api_platformvm_inputs.stakeablelockin.md#getinput)
* [getInputID](api_platformvm_inputs.stakeablelockin.md#getinputid)
* [getSigIdxs](api_platformvm_inputs.stakeablelockin.md#getsigidxs)
* [getStakeableLocktime](api_platformvm_inputs.stakeablelockin.md#getstakeablelocktime)
* [getTransferableInput](api_platformvm_inputs.stakeablelockin.md#gettransferableinput)
* [getTypeID](api_platformvm_inputs.stakeablelockin.md#gettypeid)
* [getTypeName](api_platformvm_inputs.stakeablelockin.md#gettypename)
* [sanitizeObject](api_platformvm_inputs.stakeablelockin.md#sanitizeobject)
* [serialize](api_platformvm_inputs.stakeablelockin.md#serialize)
* [toBuffer](api_platformvm_inputs.stakeablelockin.md#tobuffer)
* [comparator](api_platformvm_inputs.stakeablelockin.md#static-comparator)

## Constructors

###  constructor

\+ **new StakeableLockIn**(`amount`: BN, `stakeableLocktime`: BN, `transferableInput`: [ParseableInput](api_platformvm_inputs.parseableinput.md)): *[StakeableLockIn](api_platformvm_inputs.stakeablelockin.md)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[constructor](common_inputs.standardparseableinput.md#constructor)*

*Defined in [src/apis/platformvm/inputs.ts:248](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L248)*

A [Input](common_inputs.input.md) class which specifies an [Input](common_inputs.input.md) that has a locktime which can also
enable staking of the value held, preventing transfers but not validation.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the input |
`stakeableLocktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the stakeable locktime |
`transferableInput` | [ParseableInput](api_platformvm_inputs.parseableinput.md) | undefined | A [ParseableInput](api_platformvm_inputs.parseableinput.md) which is embedded into this input.  |

**Returns:** *[StakeableLockIn](api_platformvm_inputs.stakeablelockin.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.STAKEABLELOCKOUTID

*Overrides [ParseableInput](api_platformvm_inputs.parseableinput.md).[_typeID](api_platformvm_inputs.parseableinput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/inputs.ts:162](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L162)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StakeableLockIn"

*Overrides [ParseableInput](api_platformvm_inputs.parseableinput.md).[_typeName](api_platformvm_inputs.parseableinput.md#protected-_typename)*

*Defined in [src/apis/platformvm/inputs.ts:161](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L161)*

___

### `Protected` input

• **input**: *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[input](common_inputs.standardparseableinput.md#protected-input)*

*Defined in [src/common/input.ts:167](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L167)*

___

### `Protected` stakeableLocktime

• **stakeableLocktime**: *Buffer*

*Defined in [src/apis/platformvm/inputs.ts:190](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L190)*

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

###  clone

▸ **clone**(): *this*

*Defined in [src/apis/platformvm/inputs.ts:230](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L230)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/apis/platformvm/inputs.ts:226](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L226)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [ParseableInput](api_platformvm_inputs.parseableinput.md).[deserialize](api_platformvm_inputs.parseableinput.md#deserialize)*

*Defined in [src/apis/platformvm/inputs.ts:179](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L179)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`outbuff`: Buffer, `offset`: number): *number*

*Overrides [ParseableInput](api_platformvm_inputs.parseableinput.md).[fromBuffer](api_platformvm_inputs.parseableinput.md#frombuffer)*

*Defined in [src/apis/platformvm/inputs.ts:199](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L199)*

Popuates the instance from a [Buffer](https://github.com/feross/buffer) representing the [StakeableLockOut](api_platformvm_outputs.stakeablelockout.md) and returns the size of the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`outbuff` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAmount

▸ **getAmount**(): *BN*

*Defined in [src/apis/platformvm/inputs.ts:239](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L239)*

Returns the amount from the underlying input

**Returns:** *BN*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getCredentialID

▸ **getCredentialID**(): *number*

*Defined in [src/apis/platformvm/inputs.ts:224](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L224)*

**Returns:** *number*

___

###  getInput

▸ **getInput**(): *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[getInput](common_inputs.standardparseableinput.md#getinput)*

*Defined in [src/common/input.ts:183](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L183)*

**Returns:** *[BaseInput](../interfaces/common_inputs.baseinput.md)*

___

###  getInputID

▸ **getInputID**(): *number*

*Defined in [src/apis/platformvm/inputs.ts:220](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L220)*

Returns the inputID for this input

**Returns:** *number*

___

###  getSigIdxs

▸ **getSigIdxs**(): *[SigIdx](common_signature.sigidx.md)[]*

*Inherited from [StandardParseableInput](common_inputs.standardparseableinput.md).[getSigIdxs](common_inputs.standardparseableinput.md#getsigidxs)*

*Defined in [src/common/input.ts:189](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L189)*

**Returns:** *[SigIdx](common_signature.sigidx.md)[]*

___

###  getStakeableLocktime

▸ **getStakeableLocktime**(): *BN*

*Defined in [src/apis/platformvm/inputs.ts:192](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L192)*

**Returns:** *BN*

___

###  getTransferableInput

▸ **getTransferableInput**(): *[ParseableInput](api_platformvm_inputs.parseableinput.md)*

*Defined in [src/apis/platformvm/inputs.ts:246](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L246)*

Backwards compatibility

**Returns:** *[ParseableInput](api_platformvm_inputs.parseableinput.md)*

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

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[serialize](common_inputs.standardparseableinput.md#serialize)*

*Defined in [src/apis/platformvm/inputs.ts:165](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L165)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[toBuffer](common_inputs.standardparseableinput.md#tobuffer)*

*Defined in [src/apis/platformvm/inputs.ts:209](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/inputs.ts#L209)*

Returns the buffer representing the [StakeableLockOut](api_platformvm_outputs.stakeablelockout.md) instance.

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
