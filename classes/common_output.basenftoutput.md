[@c4tplatform/caminojs](../api.md) › [Common-Output](../modules/common_output.md) › [BaseNFTOutput](common_output.basenftoutput.md)

# Class: BaseNFTOutput

An [Output](common_output.output.md) class which specifies an NFT.

## Hierarchy

  ↳ [Output](common_output.output.md)

  ↳ **BaseNFTOutput**

  ↳ [NFTOutput](api_avm_outputs.nftoutput.md)

## Index

### Constructors

* [constructor](common_output.basenftoutput.md#constructor)

### Properties

* [_codecID](common_output.basenftoutput.md#protected-_codecid)
* [_typeID](common_output.basenftoutput.md#protected-_typeid)
* [_typeName](common_output.basenftoutput.md#protected-_typename)
* [addresses](common_output.basenftoutput.md#protected-addresses)
* [groupID](common_output.basenftoutput.md#protected-groupid)
* [locktime](common_output.basenftoutput.md#protected-locktime)
* [numaddrs](common_output.basenftoutput.md#protected-numaddrs)
* [threshold](common_output.basenftoutput.md#protected-threshold)

### Methods

* [clone](common_output.basenftoutput.md#abstract-clone)
* [create](common_output.basenftoutput.md#abstract-create)
* [deserialize](common_output.basenftoutput.md#deserialize)
* [fromBuffer](common_output.basenftoutput.md#frombuffer)
* [getAddress](common_output.basenftoutput.md#getaddress)
* [getAddressIdx](common_output.basenftoutput.md#getaddressidx)
* [getAddresses](common_output.basenftoutput.md#getaddresses)
* [getAddressesLength](common_output.basenftoutput.md#getaddresseslength)
* [getCodecID](common_output.basenftoutput.md#getcodecid)
* [getGroupID](common_output.basenftoutput.md#getgroupid)
* [getLocktime](common_output.basenftoutput.md#getlocktime)
* [getOutputID](common_output.basenftoutput.md#abstract-getoutputid)
* [getSpenders](common_output.basenftoutput.md#getspenders)
* [getThreshold](common_output.basenftoutput.md#getthreshold)
* [getTypeID](common_output.basenftoutput.md#gettypeid)
* [getTypeName](common_output.basenftoutput.md#gettypename)
* [makeTransferable](common_output.basenftoutput.md#abstract-maketransferable)
* [meetsThreshold](common_output.basenftoutput.md#meetsthreshold)
* [sanitizeObject](common_output.basenftoutput.md#sanitizeobject)
* [serialize](common_output.basenftoutput.md#serialize)
* [toBuffer](common_output.basenftoutput.md#tobuffer)
* [toString](common_output.basenftoutput.md#tostring)
* [fromArray](common_output.basenftoutput.md#static-fromarray)
* [toArray](common_output.basenftoutput.md#static-toarray)

## Constructors

###  constructor

\+ **new BaseNFTOutput**(`addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[BaseNFTOutput](common_output.basenftoutput.md)*

*Inherited from [OutputOwners](common_output.outputowners.md).[constructor](common_output.outputowners.md#constructor)*

*Defined in [src/common/output.ts:362](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L362)*

An [Output](common_output.output.md) class which contains addresses, locktimes, and thresholds.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing output owner's addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the threshold number of signers required to sign the transaction  |

**Returns:** *[BaseNFTOutput](common_output.basenftoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Output](common_output.output.md).[_typeID](common_output.output.md#protected-_typeid)*

*Defined in [src/common/output.ts:650](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L650)*

___

### `Protected` _typeName

• **_typeName**: *string* = "BaseNFTOutput"

*Overrides [Output](common_output.output.md).[_typeName](common_output.output.md#protected-_typename)*

*Defined in [src/common/output.ts:649](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L649)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Inherited from [OutputOwners](common_output.outputowners.md).[addresses](common_output.outputowners.md#protected-addresses)*

*Defined in [src/common/output.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L198)*

___

### `Protected` groupID

• **groupID**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/output.ts:676](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L676)*

___

### `Protected` locktime

• **locktime**: *Buffer* = Buffer.alloc(8)

*Inherited from [OutputOwners](common_output.outputowners.md).[locktime](common_output.outputowners.md#protected-locktime)*

*Defined in [src/common/output.ts:195](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L195)*

___

### `Protected` numaddrs

• **numaddrs**: *Buffer* = Buffer.alloc(4)

*Inherited from [OutputOwners](common_output.outputowners.md).[numaddrs](common_output.outputowners.md#protected-numaddrs)*

*Defined in [src/common/output.ts:197](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L197)*

___

### `Protected` threshold

• **threshold**: *Buffer* = Buffer.alloc(4)

*Inherited from [OutputOwners](common_output.outputowners.md).[threshold](common_output.outputowners.md#protected-threshold)*

*Defined in [src/common/output.ts:196](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L196)*

## Methods

### `Abstract` clone

▸ **clone**(): *this*

*Inherited from [Output](common_output.output.md).[clone](common_output.output.md#abstract-clone)*

*Defined in [src/common/output.ts:432](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L432)*

**Returns:** *this*

___

### `Abstract` create

▸ **create**(...`args`: any[]): *this*

*Inherited from [Output](common_output.output.md).[create](common_output.output.md#abstract-create)*

*Defined in [src/common/output.ts:434](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L434)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [OutputOwners](common_output.outputowners.md).[deserialize](common_output.outputowners.md#deserialize)*

*Defined in [src/common/output.ts:665](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L665)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Inherited from [OutputOwners](common_output.outputowners.md).[fromBuffer](common_output.outputowners.md#frombuffer)*

*Defined in [src/common/output.ts:322](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L322)*

Returns a base-58 string representing the [Output](common_output.output.md).

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAddress

▸ **getAddress**(`idx`: number): *Buffer*

*Inherited from [OutputOwners](common_output.outputowners.md).[getAddress](common_output.outputowners.md#getaddress)*

*Defined in [src/common/output.ts:253](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L253)*

Returns the address from the index provided.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`idx` | number | The index of the address.  |

**Returns:** *Buffer*

Returns the string representing the address.

___

###  getAddressIdx

▸ **getAddressIdx**(`address`: Buffer): *number*

*Inherited from [OutputOwners](common_output.outputowners.md).[getAddressIdx](common_output.outputowners.md#getaddressidx)*

*Defined in [src/common/output.ts:233](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L233)*

Returns the index of the address.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | Buffer | A [Buffer](https://github.com/feross/buffer) of the address to look up to return its index.  |

**Returns:** *number*

The index of the address.

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Inherited from [OutputOwners](common_output.outputowners.md).[getAddresses](common_output.outputowners.md#getaddresses)*

*Defined in [src/common/output.ts:213](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L213)*

Returns an array of [Buffer](https://github.com/feross/buffer)s for the addresses.

**Returns:** *Buffer[]*

___

###  getAddressesLength

▸ **getAddressesLength**(): *number*

*Inherited from [OutputOwners](common_output.outputowners.md).[getAddressesLength](common_output.outputowners.md#getaddresseslength)*

*Defined in [src/common/output.ts:224](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L224)*

Returns an the length of the Addresses array.

**Returns:** *number*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getGroupID

▸ **getGroupID**(): *number*

*Defined in [src/common/output.ts:681](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L681)*

Returns the groupID as a number.

**Returns:** *number*

___

###  getLocktime

▸ **getLocktime**(): *BN*

*Inherited from [OutputOwners](common_output.outputowners.md).[getLocktime](common_output.outputowners.md#getlocktime)*

*Defined in [src/common/output.ts:208](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L208)*

Returns the a [BN](https://github.com/indutny/bn.js/) repersenting the UNIX Timestamp when the lock is made available.

**Returns:** *BN*

___

### `Abstract` getOutputID

▸ **getOutputID**(): *number*

*Inherited from [Output](common_output.output.md).[getOutputID](common_output.output.md#abstract-getoutputid)*

*Defined in [src/common/output.ts:430](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L430)*

Returns the outputID for the output which tells parsers what type it is

**Returns:** *number*

___

###  getSpenders

▸ **getSpenders**(`addresses`: Buffer[], `asOf`: BN): *Buffer[]*

*Inherited from [OutputOwners](common_output.outputowners.md).[getSpenders](common_output.outputowners.md#getspenders)*

*Defined in [src/common/output.ts:282](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L282)*

Given an array of addresses and an optional timestamp, select an array of address [Buffer](https://github.com/feross/buffer)s of qualified spenders for the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`addresses` | Buffer[] | - |
`asOf` | BN | undefined |

**Returns:** *Buffer[]*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Inherited from [OutputOwners](common_output.outputowners.md).[getThreshold](common_output.outputowners.md#getthreshold)*

*Defined in [src/common/output.ts:203](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L203)*

Returns the threshold of signers required to spend this output.

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

### `Abstract` makeTransferable

▸ **makeTransferable**(`assetID`: Buffer): *[StandardTransferableOutput](common_output.standardtransferableoutput.md)*

*Inherited from [Output](common_output.output.md).[makeTransferable](common_output.output.md#abstract-maketransferable)*

*Defined in [src/common/output.ts:442](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L442)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  Must be implemented to use the appropriate TransferableOutput for the VM.  |

**Returns:** *[StandardTransferableOutput](common_output.standardtransferableoutput.md)*

___

###  meetsThreshold

▸ **meetsThreshold**(`addresses`: Buffer[], `asOf`: BN): *boolean*

*Inherited from [OutputOwners](common_output.outputowners.md).[meetsThreshold](common_output.outputowners.md#meetsthreshold)*

*Defined in [src/common/output.ts:263](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L263)*

Given an array of address [Buffer](https://github.com/feross/buffer)s and an optional timestamp, returns true if the addresses meet the threshold required to spend the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`addresses` | Buffer[] | - |
`asOf` | BN | undefined |

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

*Overrides [OutputOwners](common_output.outputowners.md).[serialize](common_output.outputowners.md#serialize)*

*Defined in [src/common/output.ts:652](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L652)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [OutputOwners](common_output.outputowners.md).[toBuffer](common_output.outputowners.md#tobuffer)*

*Defined in [src/common/output.ts:343](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L343)*

Returns the buffer representing the [Output](common_output.output.md) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [OutputOwners](common_output.outputowners.md).[toString](common_output.outputowners.md#tostring)*

*Defined in [src/common/output.ts:360](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L360)*

Returns a base-58 string representing the [Output](common_output.output.md).

**Returns:** *string*

___

### `Static` fromArray

▸ **fromArray**(`b`: Buffer): *[OutputOwners](common_output.outputowners.md)[]*

*Inherited from [OutputOwners](common_output.outputowners.md).[fromArray](common_output.outputowners.md#static-fromarray)*

*Defined in [src/common/output.ts:395](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L395)*

**Parameters:**

Name | Type |
------ | ------ |
`b` | Buffer |

**Returns:** *[OutputOwners](common_output.outputowners.md)[]*

___

### `Static` toArray

▸ **toArray**(`o`: [OutputOwners](common_output.outputowners.md)[]): *Buffer*

*Inherited from [OutputOwners](common_output.outputowners.md).[toArray](common_output.outputowners.md#static-toarray)*

*Defined in [src/common/output.ts:407](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L407)*

**Parameters:**

Name | Type |
------ | ------ |
`o` | [OutputOwners](common_output.outputowners.md)[] |

**Returns:** *Buffer*
