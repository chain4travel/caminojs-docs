[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Outputs](../modules/api_platformvm_outputs.md) › [LockedOut](api_platformvm_outputs.lockedout.md)

# Class: LockedOut

An [Output](../modules/src_common.md#output) class which specifies an output that is controlled by deposit and bond tx.

## Hierarchy

  ↳ [ParseableOutput](api_platformvm_outputs.parseableoutput.md)

  ↳ **LockedOut**

## Index

### Constructors

* [constructor](api_platformvm_outputs.lockedout.md#constructor)

### Properties

* [_codecID](api_platformvm_outputs.lockedout.md#protected-_codecid)
* [_typeID](api_platformvm_outputs.lockedout.md#protected-_typeid)
* [_typeName](api_platformvm_outputs.lockedout.md#protected-_typename)
* [ids](api_platformvm_outputs.lockedout.md#protected-ids)
* [output](api_platformvm_outputs.lockedout.md#protected-output)

### Methods

* [clone](api_platformvm_outputs.lockedout.md#clone)
* [create](api_platformvm_outputs.lockedout.md#create)
* [deserialize](api_platformvm_outputs.lockedout.md#deserialize)
* [fromBuffer](api_platformvm_outputs.lockedout.md#frombuffer)
* [getAddresses](api_platformvm_outputs.lockedout.md#getaddresses)
* [getAmount](api_platformvm_outputs.lockedout.md#getamount)
* [getCodecID](api_platformvm_outputs.lockedout.md#getcodecid)
* [getLockedIDs](api_platformvm_outputs.lockedout.md#getlockedids)
* [getLocktime](api_platformvm_outputs.lockedout.md#getlocktime)
* [getOutput](api_platformvm_outputs.lockedout.md#getoutput)
* [getOutputID](api_platformvm_outputs.lockedout.md#getoutputid)
* [getThreshold](api_platformvm_outputs.lockedout.md#getthreshold)
* [getTypeID](api_platformvm_outputs.lockedout.md#gettypeid)
* [getTypeName](api_platformvm_outputs.lockedout.md#gettypename)
* [makeTransferable](api_platformvm_outputs.lockedout.md#maketransferable)
* [meetsThreshold](api_platformvm_outputs.lockedout.md#meetsthreshold)
* [sanitizeObject](api_platformvm_outputs.lockedout.md#sanitizeobject)
* [serialize](api_platformvm_outputs.lockedout.md#serialize)
* [toBuffer](api_platformvm_outputs.lockedout.md#tobuffer)
* [comparator](api_platformvm_outputs.lockedout.md#static-comparator)

## Constructors

###  constructor

\+ **new LockedOut**(`amount`: BN, `addresses`: Buffer[], `locktime`: BN, `threshold`: number, `ids`: [LockedIDs](api_platformvm_locked.lockedids.md)): *[LockedOut](api_platformvm_outputs.lockedout.md)*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[constructor](common_output.standardparseableoutput.md#constructor)*

*Defined in [src/apis/platformvm/outputs.ts:390](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L390)*

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the output |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the the threshold number of signers required to sign the transaction |
`ids` | [LockedIDs](api_platformvm_locked.lockedids.md) | undefined | LockIDs set of deposit and bond txIDs  |

**Returns:** *[LockedOut](api_platformvm_outputs.lockedout.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.LOCKEDOUTID

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[_typeID](api_platformvm_outputs.parseableoutput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/outputs.ts:320](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L320)*

___

### `Protected` _typeName

• **_typeName**: *string* = "LockedOut"

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[_typeName](api_platformvm_outputs.parseableoutput.md#protected-_typename)*

*Defined in [src/apis/platformvm/outputs.ts:319](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L319)*

___

### `Protected` ids

• **ids**: *[LockedIDs](api_platformvm_locked.lockedids.md)* = new LockedIDs()

*Defined in [src/apis/platformvm/outputs.ts:337](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L337)*

___

### `Protected` output

• **output**: *[BaseOutput](../interfaces/common_output.baseoutput.md)*

*Inherited from [StandardParseableOutput](common_output.standardparseableoutput.md).[output](common_output.standardparseableoutput.md#protected-output)*

*Defined in [src/common/output.ts:457](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L457)*

## Methods

###  clone

▸ **clone**(): *this*

*Defined in [src/apis/platformvm/outputs.ts:354](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L354)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/apis/platformvm/outputs.ts:350](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L350)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [ParseableOutput](api_platformvm_outputs.parseableoutput.md).[deserialize](api_platformvm_outputs.parseableoutput.md#deserialize)*

*Defined in [src/apis/platformvm/outputs.ts:332](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L332)*

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

*Defined in [src/apis/platformvm/outputs.ts:363](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L363)*

Popuates the instance from a [Buffer](https://github.com/feross/buffer) representing the [LockedOut](api_platformvm_outputs.lockedout.md) and returns the size of the output.

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

*Defined in [src/common/output.ts:490](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L490)*

**Returns:** *Buffer[]*

___

###  getAmount

▸ **getAmount**(): *BN*

*Defined in [src/apis/platformvm/outputs.ts:388](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L388)*

Returns the amount from the underlying output

**Returns:** *BN*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getLockedIDs

▸ **getLockedIDs**(): *[LockedIDs](api_platformvm_locked.lockedids.md)*

*Defined in [src/apis/platformvm/outputs.ts:339](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L339)*

**Returns:** *[LockedIDs](api_platformvm_locked.lockedids.md)*

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

###  getOutputID

▸ **getOutputID**(): *number*

*Defined in [src/apis/platformvm/outputs.ts:381](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L381)*

Returns the outputID for this output

**Returns:** *number*

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

###  makeTransferable

▸ **makeTransferable**(`assetID`: Buffer): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

*Defined in [src/apis/platformvm/outputs.ts:346](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L346)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  |

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

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

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[serialize](common_output.standardparseableoutput.md#serialize)*

*Defined in [src/apis/platformvm/outputs.ts:323](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L323)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [StandardParseableOutput](common_output.standardparseableoutput.md).[toBuffer](common_output.standardparseableoutput.md#tobuffer)*

*Defined in [src/apis/platformvm/outputs.ts:372](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L372)*

Returns the buffer representing the [LockedOut](api_platformvm_outputs.lockedout.md) instance.

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
