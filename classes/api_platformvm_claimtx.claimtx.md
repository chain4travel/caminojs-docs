[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-ClaimTx](../modules/api_platformvm_claimtx.md) › [ClaimTx](api_platformvm_claimtx.claimtx.md)

# Class: ClaimTx

Class representing an unsigned ClaimTx transaction.

## Hierarchy

  ↳ [BaseTx](api_platformvm_basetx.basetx.md)

  ↳ **ClaimTx**

## Index

### Constructors

* [constructor](api_platformvm_claimtx.claimtx.md#constructor)

### Properties

* [_codecID](api_platformvm_claimtx.claimtx.md#protected-_codecid)
* [_outputOwners](api_platformvm_claimtx.claimtx.md#protected-_outputowners)
* [_typeID](api_platformvm_claimtx.claimtx.md#protected-_typeid)
* [_typeName](api_platformvm_claimtx.claimtx.md#protected-_typename)
* [blockchainID](api_platformvm_claimtx.claimtx.md#protected-blockchainid)
* [claimAmounts](api_platformvm_claimtx.claimtx.md#protected-claimamounts)
* [ins](api_platformvm_claimtx.claimtx.md#protected-ins)
* [memo](api_platformvm_claimtx.claimtx.md#protected-memo)
* [networkID](api_platformvm_claimtx.claimtx.md#protected-networkid)
* [numClaimAmounts](api_platformvm_claimtx.claimtx.md#protected-numclaimamounts)
* [numins](api_platformvm_claimtx.claimtx.md#protected-numins)
* [numouts](api_platformvm_claimtx.claimtx.md#protected-numouts)
* [outs](api_platformvm_claimtx.claimtx.md#protected-outs)
* [sigIdxs](api_platformvm_claimtx.claimtx.md#protected-sigidxs)

### Methods

* [addSigIdxs](api_platformvm_claimtx.claimtx.md#addsigidxs)
* [clone](api_platformvm_claimtx.claimtx.md#clone)
* [create](api_platformvm_claimtx.claimtx.md#create)
* [deserialize](api_platformvm_claimtx.claimtx.md#deserialize)
* [fromBuffer](api_platformvm_claimtx.claimtx.md#frombuffer)
* [getBlockchainID](api_platformvm_claimtx.claimtx.md#getblockchainid)
* [getClaimAmounts](api_platformvm_claimtx.claimtx.md#getclaimamounts)
* [getCodecID](api_platformvm_claimtx.claimtx.md#getcodecid)
* [getIns](api_platformvm_claimtx.claimtx.md#getins)
* [getMemo](api_platformvm_claimtx.claimtx.md#getmemo)
* [getNetworkID](api_platformvm_claimtx.claimtx.md#getnetworkid)
* [getOutputOwners](api_platformvm_claimtx.claimtx.md#getoutputowners)
* [getOuts](api_platformvm_claimtx.claimtx.md#getouts)
* [getSigIdxs](api_platformvm_claimtx.claimtx.md#getsigidxs)
* [getTotalOuts](api_platformvm_claimtx.claimtx.md#gettotalouts)
* [getTxType](api_platformvm_claimtx.claimtx.md#gettxtype)
* [getTypeID](api_platformvm_claimtx.claimtx.md#gettypeid)
* [getTypeName](api_platformvm_claimtx.claimtx.md#gettypename)
* [sanitizeObject](api_platformvm_claimtx.claimtx.md#sanitizeobject)
* [select](api_platformvm_claimtx.claimtx.md#select)
* [serialize](api_platformvm_claimtx.claimtx.md#serialize)
* [setOutputOwners](api_platformvm_claimtx.claimtx.md#setoutputowners)
* [sign](api_platformvm_claimtx.claimtx.md#sign)
* [toBuffer](api_platformvm_claimtx.claimtx.md#tobuffer)
* [toString](api_platformvm_claimtx.claimtx.md#tostring)
* [toStringHex](api_platformvm_claimtx.claimtx.md#tostringhex)

## Constructors

###  constructor

\+ **new ClaimTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `ins`: [TransferableInput](api_platformvm_inputs.transferableinput.md)[], `memo`: Buffer, `claimAmounts`: [ClaimAmount](api_platformvm_claimtx.claimamount.md)[]): *[ClaimTx](api_platformvm_claimtx.claimtx.md)*

*Overrides [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md).[constructor](api_platformvm_unlockdeposittx.unlockdeposittx.md#constructor)*

*Defined in [src/apis/platformvm/claimtx.ts:235](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L235)*

Class representing an unsigned Claim transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Optional networkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | Buffer.alloc(32, 16) | Optional blockchainID, default Buffer.alloc(32, 16) |
`outs` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional array of the [TransferableOutput](api_evm_outputs.transferableoutput.md)s |
`ins` | [TransferableInput](api_platformvm_inputs.transferableinput.md)[] | undefined | Optional array of the [TransferableInput](api_evm_inputs.transferableinput.md)s |
`memo` | Buffer | undefined | - |
`claimAmounts` | [ClaimAmount](api_platformvm_claimtx.claimamount.md)[] | undefined | Optional array of ClaimAmount class instances  |

**Returns:** *[ClaimTx](api_platformvm_claimtx.claimtx.md)*

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

• **_typeID**: *number* = PlatformVMConstants.CLAIMTX

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[_typeID](api_platformvm_basetx.basetx.md#protected-_typeid)*

*Defined in [src/apis/platformvm/claimtx.ts:134](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L134)*

___

### `Protected` _typeName

• **_typeName**: *string* = "ClaimTx"

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[_typeName](api_platformvm_basetx.basetx.md#protected-_typename)*

*Defined in [src/apis/platformvm/claimtx.ts:133](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L133)*

___

### `Protected` blockchainID

• **blockchainID**: *Buffer* = Buffer.alloc(32)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[blockchainID](common_transactions.standardbasetx.md#protected-blockchainid)*

*Defined in [src/common/tx.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L86)*

___

### `Protected` claimAmounts

• **claimAmounts**: *[ClaimAmount](api_platformvm_claimtx.claimamount.md)[]* = []

*Defined in [src/apis/platformvm/claimtx.ts:153](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L153)*

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

### `Protected` numClaimAmounts

• **numClaimAmounts**: *Buffer* = Buffer.alloc(4)

*Defined in [src/apis/platformvm/claimtx.ts:152](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L152)*

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

### `Protected` sigIdxs

• **sigIdxs**: *[SigIdx](common_signature.sigidx.md)[][]* = []

*Defined in [src/apis/platformvm/claimtx.ts:155](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L155)*

## Methods

###  addSigIdxs

▸ **addSigIdxs**(`sigIdxs`: [SigIdx](common_signature.sigidx.md)[]): *void*

*Defined in [src/apis/platformvm/claimtx.ts:226](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L226)*

Adds an array of [SigIdx](common_signature.sigidx.md) to the [ClaimTx](api_platformvm_claimtx.claimtx.md).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`sigIdxs` | [SigIdx](common_signature.sigidx.md)[] | The Signature indices to verify one claimAmount  |

**Returns:** *void*

___

###  clone

▸ **clone**(): *this*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[clone](api_platformvm_createsubnettx.createsubnettx.md#clone)*

*Defined in [src/apis/platformvm/claimtx.ts:211](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L211)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[create](api_platformvm_createsubnettx.createsubnettx.md#create)*

*Defined in [src/apis/platformvm/claimtx.ts:217](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L217)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md).[deserialize](api_platformvm_unlockdeposittx.unlockdeposittx.md#deserialize)*

*Defined in [src/apis/platformvm/claimtx.ts:136](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L136)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md).[fromBuffer](api_platformvm_unlockdeposittx.unlockdeposittx.md#frombuffer)*

*Defined in [src/apis/platformvm/claimtx.ts:176](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L176)*

Takes a [Buffer](https://github.com/feross/buffer) containing a [ClaimTx](api_platformvm_claimtx.claimtx.md), parses it, populates the class, and returns the length of the [ClaimTx](api_platformvm_claimtx.claimtx.md) in bytes.

**`remarks`** assume not-checksummed

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`bytes` | Buffer | - | A [Buffer](https://github.com/feross/buffer) containing a raw [ClaimTx](api_platformvm_claimtx.claimtx.md)  |
`offset` | number | 0 | - |

**Returns:** *number*

The length of the raw [ClaimTx](api_platformvm_claimtx.claimtx.md)

___

###  getBlockchainID

▸ **getBlockchainID**(): *Buffer*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getBlockchainID](common_transactions.standardbasetx.md#getblockchainid)*

*Defined in [src/common/tx.ts:108](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L108)*

Returns the Buffer representation of the BlockchainID

**Returns:** *Buffer*

___

###  getClaimAmounts

▸ **getClaimAmounts**(): *[ClaimAmount](api_platformvm_claimtx.claimamount.md)[]*

*Defined in [src/apis/platformvm/claimtx.ts:164](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L164)*

**Returns:** *[ClaimAmount](api_platformvm_claimtx.claimamount.md)[]*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

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

###  getSigIdxs

▸ **getSigIdxs**(): *[SigIdx](common_signature.sigidx.md)[][]*

*Defined in [src/apis/platformvm/claimtx.ts:233](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L233)*

Returns the array of [[SigIdx[]]] for this [[TX]]

**Returns:** *[SigIdx](common_signature.sigidx.md)[][]*

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

*Overrides [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getTxType](api_platformvm_validationtx.validatortx.md#gettxtype)*

*Defined in [src/apis/platformvm/claimtx.ts:160](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L160)*

Returns the id of the [RegisterNodeTx](api_platformvm_registernodetx.registernodetx.md)

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

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[serialize](common_transactions.standardbasetx.md#serialize)*

*Defined in [src/apis/platformvm/claimtx.ts:144](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L144)*

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

▸ **sign**(`msg`: Buffer, `kc`: [KeyChain](api_platformvm_keychain.keychain.md)): *[Credential](common_signature.credential.md)[]*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[sign](api_platformvm_createsubnettx.createsubnettx.md#sign)*

*Defined in [src/apis/platformvm/claimtx.ts:270](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L270)*

Takes the bytes of an [UnsignedTx](api_evm_transactions.unsignedtx.md) and returns an array of [Credential](common_signature.credential.md)s

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | A Buffer for the [UnsignedTx](api_evm_transactions.unsignedtx.md) |
`kc` | [KeyChain](api_platformvm_keychain.keychain.md) | An [KeyChain](api_evm_keychain.keychain.md) used in signing  |

**Returns:** *[Credential](common_signature.credential.md)[]*

An array of [Credential](common_signature.credential.md)s

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[toBuffer](common_transactions.standardbasetx.md#tobuffer)*

*Defined in [src/apis/platformvm/claimtx.ts:194](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L194)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [ClaimTx](api_platformvm_claimtx.claimtx.md).

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
