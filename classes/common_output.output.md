[@c4tplatform/caminojs](../api.md) › [Common-Output](../modules/common_output.md) › [Output](common_output.output.md)

# Class: Output

## Hierarchy

  ↳ [OutputOwners](common_output.outputowners.md)

  ↳ **Output**

  ↳ [StandardAmountOutput](common_output.standardamountoutput.md)

  ↳ [BaseNFTOutput](common_output.basenftoutput.md)

  ↳ [SECPMintOutput](api_avm_outputs.secpmintoutput.md)

  ↳ [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md)

## Index

### Constructors

* [constructor](common_output.output.md#constructor)

### Properties

* [_codecID](common_output.output.md#protected-_codecid)
* [_typeID](common_output.output.md#protected-_typeid)
* [_typeName](common_output.output.md#protected-_typename)
* [addresses](common_output.output.md#protected-addresses)
* [locktime](common_output.output.md#protected-locktime)
* [numaddrs](common_output.output.md#protected-numaddrs)
* [threshold](common_output.output.md#protected-threshold)

### Methods

* [clone](common_output.output.md#abstract-clone)
* [create](common_output.output.md#abstract-create)
* [deserialize](common_output.output.md#deserialize)
* [fromBuffer](common_output.output.md#frombuffer)
* [getAddress](common_output.output.md#getaddress)
* [getAddressIdx](common_output.output.md#getaddressidx)
* [getAddresses](common_output.output.md#getaddresses)
* [getAddressesLength](common_output.output.md#getaddresseslength)
* [getCodecID](common_output.output.md#getcodecid)
* [getLocktime](common_output.output.md#getlocktime)
* [getOutputID](common_output.output.md#abstract-getoutputid)
* [getSpenders](common_output.output.md#getspenders)
* [getThreshold](common_output.output.md#getthreshold)
* [getTypeID](common_output.output.md#gettypeid)
* [getTypeName](common_output.output.md#gettypename)
* [makeTransferable](common_output.output.md#abstract-maketransferable)
* [meetsThreshold](common_output.output.md#meetsthreshold)
* [sanitizeObject](common_output.output.md#sanitizeobject)
* [serialize](common_output.output.md#serialize)
* [toBuffer](common_output.output.md#tobuffer)
* [toString](common_output.output.md#tostring)
* [fromArray](common_output.output.md#static-fromarray)
* [toArray](common_output.output.md#static-toarray)

## Constructors

###  constructor

\+ **new Output**(`addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[Output](common_output.output.md)*

*Inherited from [OutputOwners](common_output.outputowners.md).[constructor](common_output.outputowners.md#constructor)*

*Defined in [src/common/output.ts:362](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L362)*

An [Output](common_output.output.md) class which contains addresses, locktimes, and thresholds.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing output owner's addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the threshold number of signers required to sign the transaction  |

**Returns:** *[Output](common_output.output.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [OutputOwners](common_output.outputowners.md).[_typeID](common_output.outputowners.md#protected-_typeid)*

*Defined in [src/common/output.ts:423](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L423)*

___

### `Protected` _typeName

• **_typeName**: *string* = "Output"

*Overrides [OutputOwners](common_output.outputowners.md).[_typeName](common_output.outputowners.md#protected-_typename)*

*Defined in [src/common/output.ts:422](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L422)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Inherited from [OutputOwners](common_output.outputowners.md).[addresses](common_output.outputowners.md#protected-addresses)*

*Defined in [src/common/output.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L198)*

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

*Defined in [src/common/output.ts:432](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L432)*

**Returns:** *this*

___

### `Abstract` create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/common/output.ts:434](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L434)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Inherited from [OutputOwners](common_output.outputowners.md).[deserialize](common_output.outputowners.md#deserialize)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/common/output.ts:170](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L170)*

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

###  getLocktime

▸ **getLocktime**(): *BN*

*Inherited from [OutputOwners](common_output.outputowners.md).[getLocktime](common_output.outputowners.md#getlocktime)*

*Defined in [src/common/output.ts:208](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L208)*

Returns the a [BN](https://github.com/indutny/bn.js/) repersenting the UNIX Timestamp when the lock is made available.

**Returns:** *BN*

___

### `Abstract` getOutputID

▸ **getOutputID**(): *number*

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

*Inherited from [OutputOwners](common_output.outputowners.md).[serialize](common_output.outputowners.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/output.ts:147](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L147)*

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
