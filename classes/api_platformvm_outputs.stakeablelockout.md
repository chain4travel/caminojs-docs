[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Outputs](../modules/api_platformvm_outputs.md) › [StakeableLockOut](api_platformvm_outputs.stakeablelockout.md)

# Class: StakeableLockOut

An [Output](../modules/src_common.md#output) class which specifies an output that has a locktime which can also enable
staking of the value held, preventing transfers but not validation.

## Hierarchy

  ↳ [ParseableOutput](api_platformvm_outputs.parseableoutput.md)

  ↳ **StakeableLockOut**

## Index

### Constructors

* [constructor](api_platformvm_outputs.stakeablelockout.md#constructor)

### Properties

* [_codecID](api_platformvm_outputs.stakeablelockout.md#protected-_codecid)
* [_typeID](api_platformvm_outputs.stakeablelockout.md#protected-_typeid)
* [_typeName](api_platformvm_outputs.stakeablelockout.md#protected-_typename)
* [output](api_platformvm_outputs.stakeablelockout.md#protected-output)
* [stakeableLocktime](api_platformvm_outputs.stakeablelockout.md#protected-stakeablelocktime)

### Methods

* [clone](api_platformvm_outputs.stakeablelockout.md#clone)
* [create](api_platformvm_outputs.stakeablelockout.md#create)
* [deserialize](api_platformvm_outputs.stakeablelockout.md#deserialize)
* [fromBuffer](api_platformvm_outputs.stakeablelockout.md#frombuffer)
* [getAddresses](api_platformvm_outputs.stakeablelockout.md#getaddresses)
* [getAmount](api_platformvm_outputs.stakeablelockout.md#getamount)
* [getCodecID](api_platformvm_outputs.stakeablelockout.md#getcodecid)
* [getLocktime](api_platformvm_outputs.stakeablelockout.md#getlocktime)
* [getOutput](api_platformvm_outputs.stakeablelockout.md#getoutput)
* [getOutputID](api_platformvm_outputs.stakeablelockout.md#getoutputid)
* [getStakeableLocktime](api_platformvm_outputs.stakeablelockout.md#getstakeablelocktime)
* [getThreshold](api_platformvm_outputs.stakeablelockout.md#getthreshold)
* [getTransferableOutput](api_platformvm_outputs.stakeablelockout.md#gettransferableoutput)
* [getTypeID](api_platformvm_outputs.stakeablelockout.md#gettypeid)
* [getTypeName](api_platformvm_outputs.stakeablelockout.md#gettypename)
* [makeTransferable](api_platformvm_outputs.stakeablelockout.md#maketransferable)
* [meetsThreshold](api_platformvm_outputs.stakeablelockout.md#meetsthreshold)
* [sanitizeObject](api_platformvm_outputs.stakeablelockout.md#sanitizeobject)
* [serialize](api_platformvm_outputs.stakeablelockout.md#serialize)
* [toBuffer](api_platformvm_outputs.stakeablelockout.md#tobuffer)
* [comparator](api_platformvm_outputs.stakeablelockout.md#static-comparator)

## Constructors

###  constructor

\+ **new StakeableLockOut**(`amount`: BN, `addresses`: Buffer[], `locktime`: BN, `threshold`: number, `stakeableLocktime`: BN, `output`: [ParseableOutput](api_platformvm_outputs.parseableoutput.md)): *[StakeableLockOut](api_platformvm_outputs.stakeablelockout.md)*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[constructor](common_output.standardparseableoutput.md#constructor)*

*Defined in [src/apis/platformvm/outputs.ts:248](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L248)*

A [Output](../modules/src_common.md#output) class which specifies a [ParseableOutput](api_platformvm_outputs.parseableoutput.md) that has a locktime which can also
enable staking of the value held, preventing transfers but not validation.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the output |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the the threshold number of signers required to sign the transaction |
`stakeableLocktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the stakeable locktime |
`output` | [ParseableOutput](api_platformvm_outputs.parseableoutput.md) | undefined | A [BaseOutput](../modules/src_common.md#baseoutput) which is embedded into this output.  |

**Returns:** *[StakeableLockOut](api_platformvm_outputs.stakeablelockout.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.STAKEABLELOCKOUTID

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[_typeID](api_platformvm_outputs.parseableoutput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/outputs.ts:157](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L157)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StakeableLockOut"

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[_typeName](api_platformvm_outputs.parseableoutput.md#protected-_typename)*

*Defined in [src/apis/platformvm/outputs.ts:156](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L156)*

___

### `Protected` output

• **output**: *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[output](common_output.standardparseableoutput.md#protected-output)*

*Defined in [src/common/output.ts:427](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L427)*

___

### `Protected` stakeableLocktime

• **stakeableLocktime**: *Buffer*

*Defined in [src/apis/platformvm/outputs.ts:185](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L185)*

## Methods

###  clone

▸ **clone**(): *this*

*Defined in [src/apis/platformvm/outputs.ts:230](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L230)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/apis/platformvm/outputs.ts:226](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L226)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[deserialize](api_platformvm_outputs.parseableoutput.md#deserialize)*

*Defined in [src/apis/platformvm/outputs.ts:174](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L174)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`outbuff`: Buffer, `offset`: number): *number*

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[fromBuffer](api_platformvm_outputs.parseableoutput.md#frombuffer)*

*Defined in [src/apis/platformvm/outputs.ts:201](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L201)*

Popuates the instance from a [Buffer](https://github.com/feross/buffer) representing the [StakeableLockOut](api_platformvm_outputs.stakeablelockout.md) and returns the size of the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`outbuff` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getAddresses](common_output.standardparseableoutput.md#getaddresses)*

*Defined in [src/common/output.ts:460](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L460)*

**Returns:** *Buffer[]*

___

###  getAmount

▸ **getAmount**(): *BN*

*Defined in [src/apis/platformvm/outputs.ts:239](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L239)*

Returns the amount from the underlying output

**Returns:** *BN*

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

###  getOutputID

▸ **getOutputID**(): *number*

*Defined in [src/apis/platformvm/outputs.ts:222](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L222)*

Returns the outputID for this output

**Returns:** *number*

___

###  getStakeableLocktime

▸ **getStakeableLocktime**(): *BN*

*Defined in [src/apis/platformvm/outputs.ts:187](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L187)*

**Returns:** *BN*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[getThreshold](common_output.standardparseableoutput.md#getthreshold)*

*Defined in [src/common/output.ts:454](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L454)*

**Returns:** *number*

___

###  getTransferableOutput

▸ **getTransferableOutput**(): *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

*Defined in [src/apis/platformvm/outputs.ts:246](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L246)*

Backwards compatibility

**Returns:** *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

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

###  makeTransferable

▸ **makeTransferable**(`assetID`: Buffer): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

*Defined in [src/apis/platformvm/outputs.ts:194](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L194)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  |

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

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

*Defined in [src/apis/platformvm/outputs.ts:160](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L160)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[toBuffer](common_output.standardparseableoutput.md#tobuffer)*

*Defined in [src/apis/platformvm/outputs.ts:211](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L211)*

Returns the buffer representing the [StakeableLockOut](api_platformvm_outputs.stakeablelockout.md) instance.

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
