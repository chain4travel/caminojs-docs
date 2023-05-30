[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-MultisigAliasTx](../modules/api_platformvm_multisigaliastx.md) › [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md)

# Class: MultisigAliasTx

Class representing an unsigned MultisigAlias transaction.

## Hierarchy

  ↳ [BaseTx](api_platformvm_basetx.basetx.md)

  ↳ **MultisigAliasTx**

## Index

### Constructors

* [constructor](api_platformvm_multisigaliastx.multisigaliastx.md#constructor)

### Properties

* [_codecID](api_platformvm_multisigaliastx.multisigaliastx.md#protected-_codecid)
* [_outputOwners](api_platformvm_multisigaliastx.multisigaliastx.md#protected-_outputowners)
* [_typeID](api_platformvm_multisigaliastx.multisigaliastx.md#protected-_typeid)
* [_typeName](api_platformvm_multisigaliastx.multisigaliastx.md#protected-_typename)
* [auth](api_platformvm_multisigaliastx.multisigaliastx.md#protected-auth)
* [blockchainID](api_platformvm_multisigaliastx.multisigaliastx.md#protected-blockchainid)
* [ins](api_platformvm_multisigaliastx.multisigaliastx.md#protected-ins)
* [memo](api_platformvm_multisigaliastx.multisigaliastx.md#protected-memo)
* [multisigAlias](api_platformvm_multisigaliastx.multisigaliastx.md#protected-multisigalias)
* [networkID](api_platformvm_multisigaliastx.multisigaliastx.md#protected-networkid)
* [numins](api_platformvm_multisigaliastx.multisigaliastx.md#protected-numins)
* [numouts](api_platformvm_multisigaliastx.multisigaliastx.md#protected-numouts)
* [outs](api_platformvm_multisigaliastx.multisigaliastx.md#protected-outs)
* [sigCount](api_platformvm_multisigaliastx.multisigaliastx.md#protected-sigcount)
* [sigIdxs](api_platformvm_multisigaliastx.multisigaliastx.md#protected-sigidxs)

### Methods

* [addSignatureIdx](api_platformvm_multisigaliastx.multisigaliastx.md#addsignatureidx)
* [clone](api_platformvm_multisigaliastx.multisigaliastx.md#clone)
* [create](api_platformvm_multisigaliastx.multisigaliastx.md#create)
* [deserialize](api_platformvm_multisigaliastx.multisigaliastx.md#deserialize)
* [fromBuffer](api_platformvm_multisigaliastx.multisigaliastx.md#frombuffer)
* [getAuth](api_platformvm_multisigaliastx.multisigaliastx.md#getauth)
* [getBlockchainID](api_platformvm_multisigaliastx.multisigaliastx.md#getblockchainid)
* [getCodecID](api_platformvm_multisigaliastx.multisigaliastx.md#getcodecid)
* [getCredentialID](api_platformvm_multisigaliastx.multisigaliastx.md#getcredentialid)
* [getIns](api_platformvm_multisigaliastx.multisigaliastx.md#getins)
* [getMemo](api_platformvm_multisigaliastx.multisigaliastx.md#getmemo)
* [getMultisigAlias](api_platformvm_multisigaliastx.multisigaliastx.md#getmultisigalias)
* [getNetworkID](api_platformvm_multisigaliastx.multisigaliastx.md#getnetworkid)
* [getOutputOwners](api_platformvm_multisigaliastx.multisigaliastx.md#getoutputowners)
* [getOuts](api_platformvm_multisigaliastx.multisigaliastx.md#getouts)
* [getSigIdxs](api_platformvm_multisigaliastx.multisigaliastx.md#getsigidxs)
* [getTotalOuts](api_platformvm_multisigaliastx.multisigaliastx.md#gettotalouts)
* [getTxType](api_platformvm_multisigaliastx.multisigaliastx.md#gettxtype)
* [getTypeID](api_platformvm_multisigaliastx.multisigaliastx.md#gettypeid)
* [getTypeName](api_platformvm_multisigaliastx.multisigaliastx.md#gettypename)
* [sanitizeObject](api_platformvm_multisigaliastx.multisigaliastx.md#sanitizeobject)
* [select](api_platformvm_multisigaliastx.multisigaliastx.md#select)
* [serialize](api_platformvm_multisigaliastx.multisigaliastx.md#serialize)
* [setOutputOwners](api_platformvm_multisigaliastx.multisigaliastx.md#setoutputowners)
* [sign](api_platformvm_multisigaliastx.multisigaliastx.md#sign)
* [toBuffer](api_platformvm_multisigaliastx.multisigaliastx.md#tobuffer)
* [toString](api_platformvm_multisigaliastx.multisigaliastx.md#tostring)
* [toStringHex](api_platformvm_multisigaliastx.multisigaliastx.md#tostringhex)

## Constructors

###  constructor

\+ **new MultisigAliasTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `ins`: [TransferableInput](api_platformvm_inputs.transferableinput.md)[], `memo`: Buffer, `multisigAlias`: [MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md), `auth`: [SubnetAuth](api_platformvm_subnetauth.subnetauth.md)): *[MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md)*

*Overrides [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md).[constructor](api_platformvm_unlockdeposittx.unlockdeposittx.md#constructor)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:261](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L261)*

Class representing a MultisigAlias transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Optional networkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | Buffer.alloc(32, 16) | Optional blockchainID, default Buffer.alloc(32, 16) |
`outs` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional array of the [TransferableOutput](api_evm_outputs.transferableoutput.md)s |
`ins` | [TransferableInput](api_platformvm_inputs.transferableinput.md)[] | undefined | Optional array of the [TransferableInput](api_evm_inputs.transferableinput.md)s |
`memo` | Buffer | undefined | Optional [Buffer](https://github.com/feross/buffer) for the memo field |
`multisigAlias` | [MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md) | undefined | Multisig alias definition. MultisigAlias.ID must be empty if it's the new alias. |
`auth` | [SubnetAuth](api_platformvm_subnetauth.subnetauth.md) | undefined | Auth that allows existing owners to change an alias.  |

**Returns:** *[MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md)*

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

• **_typeID**: *number* = PlatformVMConstants.MULTISIGALIASTX

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[_typeID](api_platformvm_basetx.basetx.md#protected-_typeid)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:106](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L106)*

___

### `Protected` _typeName

• **_typeName**: *string* = "MultisigAliasTx"

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[_typeName](api_platformvm_basetx.basetx.md#protected-_typename)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:105](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L105)*

___

### `Protected` auth

• **auth**: *[SubnetAuth](api_platformvm_subnetauth.subnetauth.md)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:111](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L111)*

___

### `Protected` blockchainID

• **blockchainID**: *Buffer* = Buffer.alloc(32)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[blockchainID](common_transactions.standardbasetx.md#protected-blockchainid)*

*Defined in [src/common/tx.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L86)*

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

### `Protected` multisigAlias

• **multisigAlias**: *[MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:109](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L109)*

___

### `Protected` networkID

• **networkID**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[networkID](common_transactions.standardbasetx.md#protected-networkid)*

*Defined in [src/common/tx.ts:85](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L85)*

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

### `Protected` sigCount

• **sigCount**: *Buffer* = Buffer.alloc(4)

*Defined in [src/apis/platformvm/multisigaliastx.ts:113](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L113)*

___

### `Protected` sigIdxs

• **sigIdxs**: *[SigIdx](common_signature.sigidx.md)[]* = []

*Defined in [src/apis/platformvm/multisigaliastx.ts:114](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L114)*

## Methods

###  addSignatureIdx

▸ **addSignatureIdx**(`addressIdx`: number, `address`: Buffer): *void*

*Defined in [src/apis/platformvm/multisigaliastx.ts:212](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L212)*

Creates and adds a [SigIdx](common_signature.sigidx.md) to the [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`addressIdx` | number | The index of the address to reference in the signatures |
`address` | Buffer | The address of the source of the signature  |

**Returns:** *void*

___

###  clone

▸ **clone**(): *this*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[clone](api_platformvm_createsubnettx.createsubnettx.md#clone)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:196](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L196)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md).[create](api_platformvm_createsubnettx.createsubnettx.md#create)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:202](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L202)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md).[deserialize](api_platformvm_unlockdeposittx.unlockdeposittx.md#deserialize)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:116](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L116)*

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

*Defined in [src/apis/platformvm/multisigaliastx.ts:163](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L163)*

Takes a [Buffer](https://github.com/feross/buffer) containing a raw [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md), parses it, populates the class, and returns the length of the [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md) in bytes.

**`remarks`** assume not-checksummed

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`bytes` | Buffer | - | A [Buffer](https://github.com/feross/buffer) containing a raw [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md) |
`offset` | number | 0 | The offset to start reading the bytes from. Default: 0  |

**Returns:** *number*

The length of the raw [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md)

___

###  getAuth

▸ **getAuth**(): *[SubnetAuth](api_platformvm_subnetauth.subnetauth.md)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:149](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L149)*

Returns the Auth that allows existing owners to change an alias.

**Returns:** *[SubnetAuth](api_platformvm_subnetauth.subnetauth.md)*

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

###  getCredentialID

▸ **getCredentialID**(): *number*

*Defined in [src/apis/platformvm/multisigaliastx.ts:233](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L233)*

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

###  getMultisigAlias

▸ **getMultisigAlias**(): *[MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md)*

*Defined in [src/apis/platformvm/multisigaliastx.ts:142](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L142)*

Returns the MultisigAlias definition.

**Returns:** *[MultisigAlias](api_platformvm_multisigaliastx.multisigalias.md)*

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

▸ **getSigIdxs**(): *[SigIdx](common_signature.sigidx.md)[]*

*Defined in [src/apis/platformvm/multisigaliastx.ts:229](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L229)*

Returns the array of [SigIdx](common_signature.sigidx.md) for this [[TX]]

**Returns:** *[SigIdx](common_signature.sigidx.md)[]*

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

*Defined in [src/apis/platformvm/multisigaliastx.ts:135](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L135)*

Returns the id of the [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md)

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

*Defined in [src/apis/platformvm/multisigaliastx.ts:124](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L124)*

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

*Defined in [src/apis/platformvm/multisigaliastx.ts:245](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L245)*

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

*Defined in [src/apis/platformvm/multisigaliastx.ts:180](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/multisigaliastx.ts#L180)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md).

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
