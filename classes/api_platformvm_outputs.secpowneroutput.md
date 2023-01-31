[@c4tplatform/caminojs](../README.md) › [API-PlatformVM-Outputs](../modules/api_platformvm_outputs.md) › [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md)

# Class: SECPOwnerOutput

An [Output](../modules/src_common.md#output) class which only specifies an Output ownership and uses secp256k1 signature scheme.

## Hierarchy

  ↳ [Output](common_output.output.md)

  ↳ **SECPOwnerOutput**

## Index

### Constructors

* [constructor](api_platformvm_outputs.secpowneroutput.md#constructor)

### Properties

* [_codecID](api_platformvm_outputs.secpowneroutput.md#protected-_codecid)
* [_typeID](api_platformvm_outputs.secpowneroutput.md#protected-_typeid)
* [_typeName](api_platformvm_outputs.secpowneroutput.md#protected-_typename)
* [addresses](api_platformvm_outputs.secpowneroutput.md#protected-addresses)
* [locktime](api_platformvm_outputs.secpowneroutput.md#protected-locktime)
* [numaddrs](api_platformvm_outputs.secpowneroutput.md#protected-numaddrs)
* [threshold](api_platformvm_outputs.secpowneroutput.md#protected-threshold)

### Methods

* [clone](api_platformvm_outputs.secpowneroutput.md#clone)
* [create](api_platformvm_outputs.secpowneroutput.md#create)
* [deserialize](api_platformvm_outputs.secpowneroutput.md#deserialize)
* [fromBuffer](api_platformvm_outputs.secpowneroutput.md#frombuffer)
* [getAddress](api_platformvm_outputs.secpowneroutput.md#getaddress)
* [getAddressIdx](api_platformvm_outputs.secpowneroutput.md#getaddressidx)
* [getAddresses](api_platformvm_outputs.secpowneroutput.md#getaddresses)
* [getCodecID](api_platformvm_outputs.secpowneroutput.md#getcodecid)
* [getLocktime](api_platformvm_outputs.secpowneroutput.md#getlocktime)
* [getOutputID](api_platformvm_outputs.secpowneroutput.md#getoutputid)
* [getSpenders](api_platformvm_outputs.secpowneroutput.md#getspenders)
* [getThreshold](api_platformvm_outputs.secpowneroutput.md#getthreshold)
* [getTypeID](api_platformvm_outputs.secpowneroutput.md#gettypeid)
* [getTypeName](api_platformvm_outputs.secpowneroutput.md#gettypename)
* [makeTransferable](api_platformvm_outputs.secpowneroutput.md#maketransferable)
* [meetsThreshold](api_platformvm_outputs.secpowneroutput.md#meetsthreshold)
* [sanitizeObject](api_platformvm_outputs.secpowneroutput.md#sanitizeobject)
* [serialize](api_platformvm_outputs.secpowneroutput.md#serialize)
* [toBuffer](api_platformvm_outputs.secpowneroutput.md#tobuffer)
* [toString](api_platformvm_outputs.secpowneroutput.md#tostring)

## Constructors

###  constructor

\+ **new SECPOwnerOutput**(`addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md)*

*Inherited from [OutputOwners](common_output.outputowners.md).[constructor](common_output.outputowners.md#constructor)*

*Defined in [src/common/output.ts:357](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L357)*

An [Output](../modules/src_common.md#output) class which contains addresses, locktimes, and thresholds.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing output owner's addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the the threshold number of signers required to sign the transaction  |

**Returns:** *[SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.SECPOWNEROUTPUTID

*Overrides [Output](common_output.output.md).[_typeID](common_output.output.md#protected-_typeid)*

*Defined in [src/apis/platformvm/outputs.ts:285](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L285)*

___

### `Protected` _typeName

• **_typeName**: *string* = "SECPOwnerOutput"

*Overrides [Output](common_output.output.md).[_typeName](common_output.output.md#protected-_typename)*

*Defined in [src/apis/platformvm/outputs.ts:284](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L284)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Inherited from [OutputOwners](common_output.outputowners.md).[addresses](common_output.outputowners.md#protected-addresses)*

*Defined in [src/common/output.ts:198](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L198)*

___

### `Protected` locktime

• **locktime**: *Buffer* = Buffer.alloc(8)

*Inherited from [OutputOwners](common_output.outputowners.md).[locktime](common_output.outputowners.md#protected-locktime)*

*Defined in [src/common/output.ts:195](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L195)*

___

### `Protected` numaddrs

• **numaddrs**: *Buffer* = Buffer.alloc(4)

*Inherited from [OutputOwners](common_output.outputowners.md).[numaddrs](common_output.outputowners.md#protected-numaddrs)*

*Defined in [src/common/output.ts:197](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L197)*

___

### `Protected` threshold

• **threshold**: *Buffer* = Buffer.alloc(4)

*Inherited from [OutputOwners](common_output.outputowners.md).[threshold](common_output.outputowners.md#protected-threshold)*

*Defined in [src/common/output.ts:196](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L196)*

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [Output](common_output.output.md).[clone](common_output.output.md#abstract-clone)*

*Defined in [src/apis/platformvm/outputs.ts:308](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L308)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [Output](common_output.output.md).[create](common_output.output.md#abstract-create)*

*Defined in [src/apis/platformvm/outputs.ts:304](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L304)*

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

*Defined in [src/common/output.ts:170](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L170)*

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

*Defined in [src/common/output.ts:317](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L317)*

Returns a base-58 string representing the [Output](../modules/src_common.md#output).

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

*Defined in [src/common/output.ts:248](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L248)*

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

*Defined in [src/common/output.ts:228](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L228)*

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

*Defined in [src/common/output.ts:213](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L213)*

Returns an array of [Buffer](https://github.com/feross/buffer)s for the addresses.

**Returns:** *Buffer[]*

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

*Inherited from [OutputOwners](common_output.outputowners.md).[getLocktime](common_output.outputowners.md#getlocktime)*

*Defined in [src/common/output.ts:208](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L208)*

Returns the a [BN](https://github.com/indutny/bn.js/) repersenting the UNIX Timestamp when the lock is made available.

**Returns:** *BN*

___

###  getOutputID

▸ **getOutputID**(): *number*

*Overrides [Output](common_output.output.md).[getOutputID](common_output.output.md#abstract-getoutputid)*

*Defined in [src/apis/platformvm/outputs.ts:292](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L292)*

Returns the outputID for this output

**Returns:** *number*

___

###  getSpenders

▸ **getSpenders**(`addresses`: Buffer[], `asOf`: BN): *Buffer[]*

*Inherited from [OutputOwners](common_output.outputowners.md).[getSpenders](common_output.outputowners.md#getspenders)*

*Defined in [src/common/output.ts:277](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L277)*

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

*Defined in [src/common/output.ts:203](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L203)*

Returns the threshold of signers required to spend this output.

**Returns:** *number*

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

*Overrides [Output](common_output.output.md).[makeTransferable](common_output.output.md#abstract-maketransferable)*

*Defined in [src/apis/platformvm/outputs.ts:300](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/outputs.ts#L300)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  |

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

___

###  meetsThreshold

▸ **meetsThreshold**(`addresses`: Buffer[], `asOf`: BN): *boolean*

*Inherited from [OutputOwners](common_output.outputowners.md).[meetsThreshold](common_output.outputowners.md#meetsthreshold)*

*Defined in [src/common/output.ts:258](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L258)*

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

*Inherited from [OutputOwners](common_output.outputowners.md).[serialize](common_output.outputowners.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/output.ts:147](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L147)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [OutputOwners](common_output.outputowners.md).[toBuffer](common_output.outputowners.md#tobuffer)*

*Defined in [src/common/output.ts:338](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L338)*

Returns the buffer representing the [Output](../modules/src_common.md#output) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [OutputOwners](common_output.outputowners.md).[toString](common_output.outputowners.md#tostring)*

*Defined in [src/common/output.ts:355](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L355)*

Returns a base-58 string representing the [Output](../modules/src_common.md#output).

**Returns:** *string*
