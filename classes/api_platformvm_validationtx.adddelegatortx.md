[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-ValidationTx](../modules/api_platformvm_validationtx.md) › [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)

# Class: AddDelegatorTx

Class representing an unsigned AddDelegatorTx transaction.

## Hierarchy

  ↳ [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md)

  ↳ **AddDelegatorTx**

  ↳ [AddValidatorTx](api_platformvm_validationtx.addvalidatortx.md)

## Index

### Constructors

* [constructor](api_platformvm_validationtx.adddelegatortx.md#constructor)

### Properties

* [_codecID](api_platformvm_validationtx.adddelegatortx.md#protected-_codecid)
* [_outputOwners](api_platformvm_validationtx.adddelegatortx.md#protected-_outputowners)
* [_typeID](api_platformvm_validationtx.adddelegatortx.md#protected-_typeid)
* [_typeName](api_platformvm_validationtx.adddelegatortx.md#protected-_typename)
* [blockchainID](api_platformvm_validationtx.adddelegatortx.md#protected-blockchainid)
* [endTime](api_platformvm_validationtx.adddelegatortx.md#protected-endtime)
* [ins](api_platformvm_validationtx.adddelegatortx.md#protected-ins)
* [memo](api_platformvm_validationtx.adddelegatortx.md#protected-memo)
* [networkID](api_platformvm_validationtx.adddelegatortx.md#protected-networkid)
* [nodeID](api_platformvm_validationtx.adddelegatortx.md#protected-nodeid)
* [numins](api_platformvm_validationtx.adddelegatortx.md#protected-numins)
* [numouts](api_platformvm_validationtx.adddelegatortx.md#protected-numouts)
* [outs](api_platformvm_validationtx.adddelegatortx.md#protected-outs)
* [rewardOwners](api_platformvm_validationtx.adddelegatortx.md#protected-rewardowners)
* [stakeOuts](api_platformvm_validationtx.adddelegatortx.md#protected-stakeouts)
* [startTime](api_platformvm_validationtx.adddelegatortx.md#protected-starttime)
* [weight](api_platformvm_validationtx.adddelegatortx.md#protected-weight)

### Methods

* [clone](api_platformvm_validationtx.adddelegatortx.md#clone)
* [create](api_platformvm_validationtx.adddelegatortx.md#create)
* [deserialize](api_platformvm_validationtx.adddelegatortx.md#deserialize)
* [fromBuffer](api_platformvm_validationtx.adddelegatortx.md#frombuffer)
* [getBlockchainID](api_platformvm_validationtx.adddelegatortx.md#getblockchainid)
* [getCodecID](api_platformvm_validationtx.adddelegatortx.md#getcodecid)
* [getEndTime](api_platformvm_validationtx.adddelegatortx.md#getendtime)
* [getIns](api_platformvm_validationtx.adddelegatortx.md#getins)
* [getMemo](api_platformvm_validationtx.adddelegatortx.md#getmemo)
* [getNetworkID](api_platformvm_validationtx.adddelegatortx.md#getnetworkid)
* [getNodeID](api_platformvm_validationtx.adddelegatortx.md#getnodeid)
* [getNodeIDString](api_platformvm_validationtx.adddelegatortx.md#getnodeidstring)
* [getOutputOwners](api_platformvm_validationtx.adddelegatortx.md#getoutputowners)
* [getOuts](api_platformvm_validationtx.adddelegatortx.md#getouts)
* [getRewardOwners](api_platformvm_validationtx.adddelegatortx.md#getrewardowners)
* [getStakeAmount](api_platformvm_validationtx.adddelegatortx.md#getstakeamount)
* [getStakeAmountBuffer](api_platformvm_validationtx.adddelegatortx.md#getstakeamountbuffer)
* [getStakeOuts](api_platformvm_validationtx.adddelegatortx.md#getstakeouts)
* [getStakeOutsTotal](api_platformvm_validationtx.adddelegatortx.md#getstakeoutstotal)
* [getStartTime](api_platformvm_validationtx.adddelegatortx.md#getstarttime)
* [getTotalOuts](api_platformvm_validationtx.adddelegatortx.md#gettotalouts)
* [getTxType](api_platformvm_validationtx.adddelegatortx.md#gettxtype)
* [getTypeID](api_platformvm_validationtx.adddelegatortx.md#gettypeid)
* [getTypeName](api_platformvm_validationtx.adddelegatortx.md#gettypename)
* [getWeight](api_platformvm_validationtx.adddelegatortx.md#getweight)
* [getWeightBuffer](api_platformvm_validationtx.adddelegatortx.md#getweightbuffer)
* [sanitizeObject](api_platformvm_validationtx.adddelegatortx.md#sanitizeobject)
* [select](api_platformvm_validationtx.adddelegatortx.md#select)
* [serialize](api_platformvm_validationtx.adddelegatortx.md#serialize)
* [setOutputOwners](api_platformvm_validationtx.adddelegatortx.md#setoutputowners)
* [sign](api_platformvm_validationtx.adddelegatortx.md#sign)
* [toBuffer](api_platformvm_validationtx.adddelegatortx.md#tobuffer)
* [toString](api_platformvm_validationtx.adddelegatortx.md#tostring)
* [toStringHex](api_platformvm_validationtx.adddelegatortx.md#tostringhex)

## Constructors

###  constructor

\+ **new AddDelegatorTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `ins`: [TransferableInput](api_platformvm_inputs.transferableinput.md)[], `memo`: Buffer, `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `stakeOuts`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `rewardOwners`: [ParseableOutput](api_platformvm_outputs.parseableoutput.md)): *[AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[constructor](api_platformvm_validationtx.weightedvalidatortx.md#constructor)*

*Defined in [src/apis/platformvm/validationtx.ts:371](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L371)*

Class representing an unsigned AddDelegatorTx transaction.

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
`stakeAmount` | BN | undefined | Optional. The amount of nAVAX the validator is staking. |
`stakeOuts` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional. The outputs used in paying the stake. |
`rewardOwners` | [ParseableOutput](api_platformvm_outputs.parseableoutput.md) | undefined | Optional. The [ParseableOutput](api_platformvm_outputs.parseableoutput.md) containing a [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md) for the rewards.  |

**Returns:** *[AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)*

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

• **_typeID**: *number* = PlatformVMConstants.ADDDELEGATORTX

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[_typeID](api_platformvm_validationtx.weightedvalidatortx.md#protected-_typeid)*

*Defined in [src/apis/platformvm/validationtx.ts:249](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L249)*

___

### `Protected` _typeName

• **_typeName**: *string* = "AddDelegatorTx"

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[_typeName](api_platformvm_validationtx.weightedvalidatortx.md#protected-_typename)*

*Defined in [src/apis/platformvm/validationtx.ts:248](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L248)*

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

### `Protected` rewardOwners

• **rewardOwners**: *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)* = undefined

*Defined in [src/apis/platformvm/validationtx.ts:271](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L271)*

___

### `Protected` stakeOuts

• **stakeOuts**: *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]* = []

*Defined in [src/apis/platformvm/validationtx.ts:270](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L270)*

___

### `Protected` startTime

• **startTime**: *Buffer* = Buffer.alloc(8)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[startTime](api_platformvm_validationtx.validatortx.md#protected-starttime)*

*Defined in [src/apis/platformvm/validationtx.ts:81](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L81)*

___

### `Protected` weight

• **weight**: *Buffer* = Buffer.alloc(8)

*Inherited from [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[weight](api_platformvm_validationtx.weightedvalidatortx.md#protected-weight)*

*Defined in [src/apis/platformvm/validationtx.ts:182](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L182)*

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[clone](api_platformvm_createsubnettx.createsubnettx.md#clone)*

*Defined in [src/apis/platformvm/validationtx.ts:363](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L363)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[create](api_platformvm_createsubnettx.createsubnettx.md#create)*

*Defined in [src/apis/platformvm/validationtx.ts:369](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L369)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[deserialize](api_platformvm_validationtx.weightedvalidatortx.md#deserialize)*

*Defined in [src/apis/platformvm/validationtx.ts:259](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L259)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[fromBuffer](api_platformvm_validationtx.weightedvalidatortx.md#frombuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:325](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L325)*

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

###  getRewardOwners

▸ **getRewardOwners**(): *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

*Defined in [src/apis/platformvm/validationtx.ts:317](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L317)*

Returns a [Buffer](https://github.com/feross/buffer) for the reward address.

**Returns:** *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

___

###  getStakeAmount

▸ **getStakeAmount**(): *BN*

*Defined in [src/apis/platformvm/validationtx.ts:283](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L283)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN*

___

###  getStakeAmountBuffer

▸ **getStakeAmountBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/validationtx.ts:290](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L290)*

Returns a [Buffer](https://github.com/feross/buffer) for the stake amount.

**Returns:** *Buffer*

___

###  getStakeOuts

▸ **getStakeOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Defined in [src/apis/platformvm/validationtx.ts:297](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L297)*

Returns the array of outputs being staked.

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getStakeOutsTotal

▸ **getStakeOutsTotal**(): *BN*

*Defined in [src/apis/platformvm/validationtx.ts:304](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L304)*

Should match stakeAmount. Used in sanity checking.

**Returns:** *BN*

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

*Overrides [ImportTx](api_platformvm_importtx.importtx.md).[getTotalOuts](api_platformvm_importtx.importtx.md#gettotalouts)*

*Defined in [src/apis/platformvm/validationtx.ts:321](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L321)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getTxType

▸ **getTxType**(): *number*

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getTxType](api_platformvm_validationtx.validatortx.md#gettxtype)*

*Defined in [src/apis/platformvm/validationtx.ts:276](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L276)*

Returns the id of the [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)

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

*Inherited from [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[getWeight](api_platformvm_validationtx.weightedvalidatortx.md#getweight)*

*Defined in [src/apis/platformvm/validationtx.ts:187](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L187)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN*

___

###  getWeightBuffer

▸ **getWeightBuffer**(): *Buffer*

*Inherited from [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[getWeightBuffer](api_platformvm_validationtx.weightedvalidatortx.md#getweightbuffer)*

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

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[serialize](api_platformvm_validationtx.weightedvalidatortx.md#serialize)*

*Defined in [src/apis/platformvm/validationtx.ts:251](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L251)*

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

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[toBuffer](api_platformvm_validationtx.weightedvalidatortx.md#tobuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:344](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/validationtx.ts#L344)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md).

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
