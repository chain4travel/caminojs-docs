[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-ValidationTx](../modules/api_platformvm_validationtx.md) › [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md)

# Class: WeightedValidatorTx

## Hierarchy

  ↳ [ValidatorTx](api_platformvm_validationtx.validatortx.md)

  ↳ **WeightedValidatorTx**

  ↳ [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)

## Index

### Constructors

* [constructor](api_platformvm_validationtx.weightedvalidatortx.md#constructor)

### Properties

* [_codecID](api_platformvm_validationtx.weightedvalidatortx.md#protected-_codecid)
* [_outputOwners](api_platformvm_validationtx.weightedvalidatortx.md#protected-_outputowners)
* [_typeID](api_platformvm_validationtx.weightedvalidatortx.md#protected-_typeid)
* [_typeName](api_platformvm_validationtx.weightedvalidatortx.md#protected-_typename)
* [blockchainID](api_platformvm_validationtx.weightedvalidatortx.md#protected-blockchainid)
* [endTime](api_platformvm_validationtx.weightedvalidatortx.md#protected-endtime)
* [ins](api_platformvm_validationtx.weightedvalidatortx.md#protected-ins)
* [memo](api_platformvm_validationtx.weightedvalidatortx.md#protected-memo)
* [networkID](api_platformvm_validationtx.weightedvalidatortx.md#protected-networkid)
* [nodeID](api_platformvm_validationtx.weightedvalidatortx.md#protected-nodeid)
* [numins](api_platformvm_validationtx.weightedvalidatortx.md#protected-numins)
* [numouts](api_platformvm_validationtx.weightedvalidatortx.md#protected-numouts)
* [outs](api_platformvm_validationtx.weightedvalidatortx.md#protected-outs)
* [startTime](api_platformvm_validationtx.weightedvalidatortx.md#protected-starttime)
* [weight](api_platformvm_validationtx.weightedvalidatortx.md#protected-weight)

### Methods

* [clone](api_platformvm_validationtx.weightedvalidatortx.md#clone)
* [create](api_platformvm_validationtx.weightedvalidatortx.md#create)
* [deserialize](api_platformvm_validationtx.weightedvalidatortx.md#deserialize)
* [fromBuffer](api_platformvm_validationtx.weightedvalidatortx.md#frombuffer)
* [getBlockchainID](api_platformvm_validationtx.weightedvalidatortx.md#getblockchainid)
* [getCodecID](api_platformvm_validationtx.weightedvalidatortx.md#getcodecid)
* [getEndTime](api_platformvm_validationtx.weightedvalidatortx.md#getendtime)
* [getIns](api_platformvm_validationtx.weightedvalidatortx.md#getins)
* [getMemo](api_platformvm_validationtx.weightedvalidatortx.md#getmemo)
* [getNetworkID](api_platformvm_validationtx.weightedvalidatortx.md#getnetworkid)
* [getNodeID](api_platformvm_validationtx.weightedvalidatortx.md#getnodeid)
* [getNodeIDString](api_platformvm_validationtx.weightedvalidatortx.md#getnodeidstring)
* [getOutputOwners](api_platformvm_validationtx.weightedvalidatortx.md#getoutputowners)
* [getOuts](api_platformvm_validationtx.weightedvalidatortx.md#getouts)
* [getStartTime](api_platformvm_validationtx.weightedvalidatortx.md#getstarttime)
* [getTotalOuts](api_platformvm_validationtx.weightedvalidatortx.md#gettotalouts)
* [getTxType](api_platformvm_validationtx.weightedvalidatortx.md#gettxtype)
* [getTypeID](api_platformvm_validationtx.weightedvalidatortx.md#gettypeid)
* [getTypeName](api_platformvm_validationtx.weightedvalidatortx.md#gettypename)
* [getWeight](api_platformvm_validationtx.weightedvalidatortx.md#getweight)
* [getWeightBuffer](api_platformvm_validationtx.weightedvalidatortx.md#getweightbuffer)
* [sanitizeObject](api_platformvm_validationtx.weightedvalidatortx.md#sanitizeobject)
* [select](api_platformvm_validationtx.weightedvalidatortx.md#select)
* [serialize](api_platformvm_validationtx.weightedvalidatortx.md#serialize)
* [setOutputOwners](api_platformvm_validationtx.weightedvalidatortx.md#setoutputowners)
* [sign](api_platformvm_validationtx.weightedvalidatortx.md#sign)
* [toBuffer](api_platformvm_validationtx.weightedvalidatortx.md#tobuffer)
* [toString](api_platformvm_validationtx.weightedvalidatortx.md#tostring)
* [toStringHex](api_platformvm_validationtx.weightedvalidatortx.md#tostringhex)

## Constructors

###  constructor

\+ **new WeightedValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `ins`: [TransferableInput](api_platformvm_inputs.transferableinput.md)[], `memo`: Buffer, `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `weight`: BN): *[WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md)*

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[constructor](api_platformvm_validationtx.validatortx.md#constructor)*

*Defined in [src/apis/platformvm/validationtx.ts:211](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L211)*

Class representing an unsigned AddSubnetValidatorTx transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Optional. Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | Buffer.alloc(32, 16) | Optional. Blockchainid, default Buffer.alloc(32, 16) |
`outs` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional. Array of the [TransferableOutput](api_evm_outputs.transferableoutput.md)s |
`ins` | [TransferableInput](api_platformvm_inputs.transferableinput.md)[] | undefined | Optional. Array of the [TransferableInput](api_evm_inputs.transferableinput.md)s |
`memo` | Buffer | undefined | Optional. [Buffer](https://github.com/feross/buffer) for the memo field |
`nodeID` | Buffer | undefined | Optional. The node ID of the validator being added. |
`startTime` | BN | undefined | Optional. The Unix time when the validator starts validating the Primary Network. |
`endTime` | BN | undefined | Optional. The Unix time when the validator stops validating the Primary Network (and staked AVAX is returned). |
`weight` | BN | undefined | Optional. The amount of nAVAX the validator is staking.  |

**Returns:** *[WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _outputOwners

• **_outputOwners**: *[OutputOwners](common_output.outputowners.md)[]* = undefined

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[_outputOwners](api_platformvm_importtx.importtx.md#protected-_outputowners)*

*Defined in [src/apis/platformvm/basetx.ts:36](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L36)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[_typeID](api_platformvm_validationtx.validatortx.md#protected-_typeid)*

*Defined in [src/apis/platformvm/validationtx.ts:157](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L157)*

___

### `Protected` _typeName

• **_typeName**: *string* = "WeightedValidatorTx"

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[_typeName](api_platformvm_validationtx.validatortx.md#protected-_typename)*

*Defined in [src/apis/platformvm/validationtx.ts:156](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L156)*

___

### `Protected` blockchainID

• **blockchainID**: *Buffer* = Buffer.alloc(32)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[blockchainID](common_transactions.standardbasetx.md#protected-blockchainid)*

*Defined in [src/common/tx.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L86)*

___

### `Protected` endTime

• **endTime**: *Buffer* = Buffer.alloc(8)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[endTime](api_platformvm_validationtx.validatortx.md#protected-endtime)*

*Defined in [src/apis/platformvm/validationtx.ts:82](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L82)*

___

### `Protected` ins

• **ins**: *[StandardTransferableInput](common_inputs.standardtransferableinput.md)[]*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[ins](common_transactions.standardbasetx.md#protected-ins)*

*Defined in [src/common/tx.ts:90](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L90)*

___

### `Protected` memo

• **memo**: *Buffer* = Buffer.alloc(0)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[memo](common_transactions.standardbasetx.md#protected-memo)*

*Defined in [src/common/tx.ts:91](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L91)*

___

### `Protected` networkID

• **networkID**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[networkID](common_transactions.standardbasetx.md#protected-networkid)*

*Defined in [src/common/tx.ts:85](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L85)*

___

### `Protected` nodeID

• **nodeID**: *Buffer* = Buffer.alloc(20)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[nodeID](api_platformvm_validationtx.validatortx.md#protected-nodeid)*

*Defined in [src/apis/platformvm/validationtx.ts:80](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L80)*

___

### `Protected` numins

• **numins**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[numins](common_transactions.standardbasetx.md#protected-numins)*

*Defined in [src/common/tx.ts:89](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L89)*

___

### `Protected` numouts

• **numouts**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[numouts](common_transactions.standardbasetx.md#protected-numouts)*

*Defined in [src/common/tx.ts:87](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L87)*

___

### `Protected` outs

• **outs**: *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[outs](common_transactions.standardbasetx.md#protected-outs)*

*Defined in [src/common/tx.ts:88](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L88)*

___

### `Protected` startTime

• **startTime**: *Buffer* = Buffer.alloc(8)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[startTime](api_platformvm_validationtx.validatortx.md#protected-starttime)*

*Defined in [src/apis/platformvm/validationtx.ts:81](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L81)*

___

### `Protected` weight

• **weight**: *Buffer* = Buffer.alloc(8)

*Defined in [src/apis/platformvm/validationtx.ts:182](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L182)*

## Methods

###  clone

▸ **clone**(): *this*

*Inherited from [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[clone](api_platformvm_createsubnettx.createsubnettx.md#clone)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[clone](common_transactions.standardbasetx.md#abstract-clone)*

*Defined in [src/apis/platformvm/basetx.ts:161](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L161)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Inherited from [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[create](api_platformvm_createsubnettx.createsubnettx.md#create)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[create](common_transactions.standardbasetx.md#abstract-create)*

*Defined in [src/apis/platformvm/basetx.ts:167](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L167)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[deserialize](api_platformvm_validationtx.validatortx.md#deserialize)*

*Defined in [src/apis/platformvm/validationtx.ts:171](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L171)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[fromBuffer](api_platformvm_validationtx.validatortx.md#frombuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L198)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getBlockchainID

▸ **getBlockchainID**(): *Buffer*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getBlockchainID](common_transactions.standardbasetx.md#getblockchainid)*

*Defined in [src/common/tx.ts:108](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L108)*

Returns the Buffer representation of the BlockchainID

**Returns:** *Buffer*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getEndTime

▸ **getEndTime**(): *BN‹›*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getEndTime](api_platformvm_validationtx.validatortx.md#getendtime)*

*Defined in [src/apis/platformvm/validationtx.ts:107](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L107)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN‹›*

___

###  getIns

▸ **getIns**(): *[TransferableInput](api_platformvm_inputs.transferableinput.md)[]*

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[getIns](api_platformvm_importtx.importtx.md#getins)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getIns](common_transactions.standardbasetx.md#abstract-getins)*

*Defined in [src/apis/platformvm/basetx.ts:60](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L60)*

**Returns:** *[TransferableInput](api_platformvm_inputs.transferableinput.md)[]*

___

###  getMemo

▸ **getMemo**(): *Buffer*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getMemo](common_transactions.standardbasetx.md#getmemo)*

*Defined in [src/common/tx.ts:130](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L130)*

Returns the [Buffer](https://github.com/feross/buffer) representation of the memo

**Returns:** *Buffer*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getNetworkID](common_transactions.standardbasetx.md#getnetworkid)*

*Defined in [src/common/tx.ts:101](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L101)*

Returns the NetworkID as a number

**Returns:** *number*

___

###  getNodeID

▸ **getNodeID**(): *Buffer*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getNodeID](api_platformvm_validationtx.validatortx.md#getnodeid)*

*Defined in [src/apis/platformvm/validationtx.ts:87](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L87)*

Returns a [Buffer](https://github.com/feross/buffer) for the stake amount.

**Returns:** *Buffer*

___

###  getNodeIDString

▸ **getNodeIDString**(): *string*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getNodeIDString](api_platformvm_validationtx.validatortx.md#getnodeidstring)*

*Defined in [src/apis/platformvm/validationtx.ts:94](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L94)*

Returns a string for the nodeID amount.

**Returns:** *string*

___

###  getOutputOwners

▸ **getOutputOwners**(): *[OutputOwners](common_output.outputowners.md)[]*

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[getOutputOwners](api_platformvm_importtx.importtx.md#getoutputowners)*

*Defined in [src/apis/platformvm/basetx.ts:78](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L78)*

**Returns:** *[OutputOwners](common_output.outputowners.md)[]*

The outputOwners of inputs, one per input

___

###  getOuts

▸ **getOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[getOuts](api_platformvm_importtx.importtx.md#getouts)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getOuts](common_transactions.standardbasetx.md#abstract-getouts)*

*Defined in [src/apis/platformvm/basetx.ts:56](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L56)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getStartTime

▸ **getStartTime**(): *BN‹›*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getStartTime](api_platformvm_validationtx.validatortx.md#getstarttime)*

*Defined in [src/apis/platformvm/validationtx.ts:100](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L100)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN‹›*

___

###  getTotalOuts

▸ **getTotalOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[getTotalOuts](api_platformvm_importtx.importtx.md#gettotalouts)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getTotalOuts](common_transactions.standardbasetx.md#abstract-gettotalouts)*

*Defined in [src/apis/platformvm/basetx.ts:64](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L64)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getTxType

▸ **getTxType**(): *number*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getTxType](api_platformvm_validationtx.validatortx.md#gettxtype)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getTxType](common_transactions.standardbasetx.md#abstract-gettxtype)*

*Defined in [src/apis/platformvm/basetx.ts:71](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L71)*

Returns the id of the [BaseTx](api_avm_basetx.basetx.md)

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

###  getWeight

▸ **getWeight**(): *BN*

*Defined in [src/apis/platformvm/validationtx.ts:187](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L187)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN*

___

###  getWeightBuffer

▸ **getWeightBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/validationtx.ts:194](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L194)*

Returns a [Buffer](https://github.com/feross/buffer) for the stake amount.

**Returns:** *Buffer*

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

###  select

▸ **select**(`id`: number, ...`args`: any[]): *this*

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[select](api_platformvm_importtx.importtx.md#select)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[select](common_transactions.standardbasetx.md#abstract-select)*

*Defined in [src/apis/platformvm/basetx.ts:171](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L171)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *this*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[serialize](api_platformvm_validationtx.validatortx.md#serialize)*

*Defined in [src/apis/platformvm/validationtx.ts:159](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L159)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  setOutputOwners

▸ **setOutputOwners**(`owners`: [OutputOwners](common_output.outputowners.md)[]): *void*

*Inherited from [ImportTx](api_platformvm_importtx.importtx.md).[setOutputOwners](api_platformvm_importtx.importtx.md#setoutputowners)*

*Defined in [src/apis/platformvm/basetx.ts:88](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L88)*

**`params`** The outputOwners of inputs, one per input

**Parameters:**

Name | Type |
------ | ------ |
`owners` | [OutputOwners](common_output.outputowners.md)[] |

**Returns:** *void*

___

###  sign

▸ **sign**(`msg`: Buffer, `kc`: [SignerKeyChain](common_keychain.signerkeychain.md)): *[Credential](common_signature.credential.md)[]*

*Inherited from [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[sign](api_platformvm_createsubnettx.createsubnettx.md#sign)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[sign](common_transactions.standardbasetx.md#abstract-sign)*

*Defined in [src/apis/platformvm/basetx.ts:142](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L142)*

Takes the bytes of an [UnsignedTx](api_evm_transactions.unsignedtx.md) and returns an array of [Credential](common_signature.credential.md)s

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | A Buffer for the [UnsignedTx](api_evm_transactions.unsignedtx.md) |
`kc` | [SignerKeyChain](common_keychain.signerkeychain.md) | An [KeyChain](api_evm_keychain.keychain.md) used in signing  |

**Returns:** *[Credential](common_signature.credential.md)[]*

An array of [Credential](common_signature.credential.md)s

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[toBuffer](api_platformvm_validationtx.validatortx.md#tobuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:208](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L208)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [AddSubnetValidatorTx](api_platformvm_addsubnetvalidatortx.addsubnetvalidatortx.md).

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[toString](common_transactions.standardbasetx.md#tostring)*

*Defined in [src/common/tx.ts:170](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L170)*

Returns a base-58 representation of the [StandardBaseTx](common_transactions.standardbasetx.md).

**Returns:** *string*

___

###  toStringHex

▸ **toStringHex**(): *string*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[toStringHex](common_transactions.standardbasetx.md#tostringhex)*

*Defined in [src/common/tx.ts:174](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L174)*

**Returns:** *string*
