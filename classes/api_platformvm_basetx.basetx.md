[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-BaseTx](../modules/api_platformvm_basetx.md) › [BaseTx](api_platformvm_basetx.basetx.md)

# Class: BaseTx

Class representing a base for all transactions.

## Hierarchy

  ↳ [StandardBaseTx](common_transactions.standardbasetx.md)‹[SignerKeyPair](common_keychain.signerkeypair.md), [SignerKeyChain](common_keychain.signerkeychain.md)›

  ↳ **BaseTx**

  ↳ [ImportTx](api_platformvm_importtx.importtx.md)

  ↳ [AddSubnetValidatorTx](api_platformvm_addsubnetvalidatortx.addsubnetvalidatortx.md)

  ↳ [ClaimTx](api_platformvm_claimtx.claimtx.md)

  ↳ [CreateChainTx](api_platformvm_createchaintx.createchaintx.md)

  ↳ [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md)

  ↳ [DepositTx](api_platformvm_deposittx.deposittx.md)

  ↳ [RegisterNodeTx](api_platformvm_registernodetx.registernodetx.md)

  ↳ [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md)

  ↳ [ValidatorTx](api_platformvm_validationtx.validatortx.md)

  ↳ [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md)

  ↳ [ExportTx](api_platformvm_exporttx.exporttx.md)

  ↳ [AddressStateTx](api_platformvm_addressstatetx.addressstatetx.md)

## Index

### Constructors

* [constructor](api_platformvm_basetx.basetx.md#constructor)

### Properties

* [_codecID](api_platformvm_basetx.basetx.md#protected-_codecid)
* [_outputOwners](api_platformvm_basetx.basetx.md#protected-_outputowners)
* [_typeID](api_platformvm_basetx.basetx.md#protected-_typeid)
* [_typeName](api_platformvm_basetx.basetx.md#protected-_typename)
* [blockchainID](api_platformvm_basetx.basetx.md#protected-blockchainid)
* [ins](api_platformvm_basetx.basetx.md#protected-ins)
* [memo](api_platformvm_basetx.basetx.md#protected-memo)
* [networkID](api_platformvm_basetx.basetx.md#protected-networkid)
* [numins](api_platformvm_basetx.basetx.md#protected-numins)
* [numouts](api_platformvm_basetx.basetx.md#protected-numouts)
* [outs](api_platformvm_basetx.basetx.md#protected-outs)

### Methods

* [clone](api_platformvm_basetx.basetx.md#clone)
* [create](api_platformvm_basetx.basetx.md#create)
* [deserialize](api_platformvm_basetx.basetx.md#deserialize)
* [fromBuffer](api_platformvm_basetx.basetx.md#frombuffer)
* [getBlockchainID](api_platformvm_basetx.basetx.md#getblockchainid)
* [getCodecID](api_platformvm_basetx.basetx.md#getcodecid)
* [getIns](api_platformvm_basetx.basetx.md#getins)
* [getMemo](api_platformvm_basetx.basetx.md#getmemo)
* [getNetworkID](api_platformvm_basetx.basetx.md#getnetworkid)
* [getOutputOwners](api_platformvm_basetx.basetx.md#getoutputowners)
* [getOuts](api_platformvm_basetx.basetx.md#getouts)
* [getTotalOuts](api_platformvm_basetx.basetx.md#gettotalouts)
* [getTxType](api_platformvm_basetx.basetx.md#gettxtype)
* [getTypeID](api_platformvm_basetx.basetx.md#gettypeid)
* [getTypeName](api_platformvm_basetx.basetx.md#gettypename)
* [sanitizeObject](api_platformvm_basetx.basetx.md#sanitizeobject)
* [select](api_platformvm_basetx.basetx.md#select)
* [serialize](api_platformvm_basetx.basetx.md#serialize)
* [setOutputOwners](api_platformvm_basetx.basetx.md#setoutputowners)
* [sign](api_platformvm_basetx.basetx.md#sign)
* [toBuffer](api_platformvm_basetx.basetx.md#tobuffer)
* [toString](api_platformvm_basetx.basetx.md#tostring)
* [toStringHex](api_platformvm_basetx.basetx.md#tostringhex)

## Constructors

###  constructor

\+ **new BaseTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `ins`: [TransferableInput](api_platformvm_inputs.transferableinput.md)[], `memo`: Buffer): *[BaseTx](api_platformvm_basetx.basetx.md)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[constructor](common_transactions.standardbasetx.md#constructor)*

*Defined in [src/apis/platformvm/basetx.ts:174](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L174)*

Class representing a BaseTx which is the foundation for all transactions.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Optional networkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | Buffer.alloc(32, 16) | Optional blockchainID, default Buffer.alloc(32, 16) |
`outs` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional array of the [TransferableOutput](api_evm_outputs.transferableoutput.md)s |
`ins` | [TransferableInput](api_platformvm_inputs.transferableinput.md)[] | undefined | Optional array of the [TransferableInput](api_evm_inputs.transferableinput.md)s |
`memo` | Buffer | undefined | Optional [Buffer](https://github.com/feross/buffer) for the memo field  |

**Returns:** *[BaseTx](api_platformvm_basetx.basetx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _outputOwners

• **_outputOwners**: *[OutputOwners](common_output.outputowners.md)[]* = undefined

*Defined in [src/apis/platformvm/basetx.ts:36](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L36)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.BASETX

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[_typeID](common_transactions.standardbasetx.md#protected-_typeid)*

*Defined in [src/apis/platformvm/basetx.ts:35](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L35)*

___

### `Protected` _typeName

• **_typeName**: *string* = "BaseTx"

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[_typeName](common_transactions.standardbasetx.md#protected-_typename)*

*Defined in [src/apis/platformvm/basetx.ts:34](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L34)*

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

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[clone](common_transactions.standardbasetx.md#abstract-clone)*

*Defined in [src/apis/platformvm/basetx.ts:161](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L161)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

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

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[deserialize](common_transactions.standardbasetx.md#deserialize)*

*Defined in [src/apis/platformvm/basetx.ts:38](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L38)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Defined in [src/apis/platformvm/basetx.ts:101](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L101)*

Takes a [Buffer](https://github.com/feross/buffer) containing an [BaseTx](api_platformvm_basetx.basetx.md), parses it, populates the class, and returns the length of the BaseTx in bytes.

**`remarks`** assume not-checksummed

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`bytes` | Buffer | - | A [Buffer](https://github.com/feross/buffer) containing a raw [BaseTx](api_platformvm_basetx.basetx.md)  |
`offset` | number | 0 | - |

**Returns:** *number*

The length of the raw [BaseTx](api_platformvm_basetx.basetx.md)

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

###  getIns

▸ **getIns**(): *[TransferableInput](api_platformvm_inputs.transferableinput.md)[]*

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

*Defined in [src/apis/platformvm/basetx.ts:78](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L78)*

**Returns:** *[OutputOwners](common_output.outputowners.md)[]*

The outputOwners of inputs, one per input

___

###  getOuts

▸ **getOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getOuts](common_transactions.standardbasetx.md#abstract-getouts)*

*Defined in [src/apis/platformvm/basetx.ts:56](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L56)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getTotalOuts

▸ **getTotalOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getTotalOuts](common_transactions.standardbasetx.md#abstract-gettotalouts)*

*Defined in [src/apis/platformvm/basetx.ts:64](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L64)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getTxType

▸ **getTxType**(): *number*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getTxType](common_transactions.standardbasetx.md#abstract-gettxtype)*

*Defined in [src/apis/platformvm/basetx.ts:71](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/basetx.ts#L71)*

Returns the id of the [BaseTx](api_platformvm_basetx.basetx.md)

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

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[serialize](common_transactions.standardbasetx.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/tx.ts:44](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L44)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  setOutputOwners

▸ **setOutputOwners**(`owners`: [OutputOwners](common_output.outputowners.md)[]): *void*

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

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[toBuffer](common_transactions.standardbasetx.md#tobuffer)*

*Defined in [src/common/tx.ts:137](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/tx.ts#L137)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [StandardBaseTx](common_transactions.standardbasetx.md).

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
