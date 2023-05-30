[@c4tplatform/caminojs](../api.md) › [Common-Output](../modules/common_output.md) › [OutputOwners](common_output.outputowners.md)

# Class: OutputOwners

Defines the most basic values for output ownership. Mostly inherited from, but can be used in population of NFT Owner data.

## Hierarchy

* [Serializable](utils_serialization.serializable.md)

  ↳ **OutputOwners**

  ↳ [Output](common_output.output.md)

## Index

### Constructors

* [constructor](common_output.outputowners.md#constructor)

### Properties

* [_codecID](common_output.outputowners.md#protected-_codecid)
* [_typeID](common_output.outputowners.md#protected-_typeid)
* [_typeName](common_output.outputowners.md#protected-_typename)
* [addresses](common_output.outputowners.md#protected-addresses)
* [locktime](common_output.outputowners.md#protected-locktime)
* [numaddrs](common_output.outputowners.md#protected-numaddrs)
* [threshold](common_output.outputowners.md#protected-threshold)

### Methods

* [deserialize](common_output.outputowners.md#deserialize)
* [fromBuffer](common_output.outputowners.md#frombuffer)
* [getAddress](common_output.outputowners.md#getaddress)
* [getAddressIdx](common_output.outputowners.md#getaddressidx)
* [getAddresses](common_output.outputowners.md#getaddresses)
* [getAddressesLength](common_output.outputowners.md#getaddresseslength)
* [getCodecID](common_output.outputowners.md#getcodecid)
* [getLocktime](common_output.outputowners.md#getlocktime)
* [getSpenders](common_output.outputowners.md#getspenders)
* [getThreshold](common_output.outputowners.md#getthreshold)
* [getTypeID](common_output.outputowners.md#gettypeid)
* [getTypeName](common_output.outputowners.md#gettypename)
* [meetsThreshold](common_output.outputowners.md#meetsthreshold)
* [sanitizeObject](common_output.outputowners.md#sanitizeobject)
* [serialize](common_output.outputowners.md#serialize)
* [toBuffer](common_output.outputowners.md#tobuffer)
* [toString](common_output.outputowners.md#tostring)
* [fromArray](common_output.outputowners.md#static-fromarray)
* [toArray](common_output.outputowners.md#static-toarray)

## Constructors

###  constructor

\+ **new OutputOwners**(`addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[OutputOwners](common_output.outputowners.md)*

*Defined in [src/common/output.ts:362](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L362)*

An [Output](common_output.output.md) class which contains addresses, locktimes, and thresholds.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing output owner's addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the threshold number of signers required to sign the transaction  |

**Returns:** *[OutputOwners](common_output.outputowners.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Serializable](utils_serialization.serializable.md).[_typeID](utils_serialization.serializable.md#protected-_typeid)*

*Defined in [src/common/output.ts:145](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L145)*

___

### `Protected` _typeName

• **_typeName**: *string* = "OutputOwners"

*Overrides [Serializable](utils_serialization.serializable.md).[_typeName](utils_serialization.serializable.md#protected-_typename)*

*Defined in [src/common/output.ts:144](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L144)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Defined in [src/common/output.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L198)*

___

### `Protected` locktime

• **locktime**: *Buffer* = Buffer.alloc(8)

*Defined in [src/common/output.ts:195](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L195)*

___

### `Protected` numaddrs

• **numaddrs**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/output.ts:197](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L197)*

___

### `Protected` threshold

• **threshold**: *Buffer* = Buffer.alloc(4)

*Defined in [src/common/output.ts:196](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L196)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

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

*Defined in [src/common/output.ts:213](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L213)*

Returns an array of [Buffer](https://github.com/feross/buffer)s for the addresses.

**Returns:** *Buffer[]*

___

###  getAddressesLength

▸ **getAddressesLength**(): *number*

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

*Defined in [src/common/output.ts:208](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L208)*

Returns the a [BN](https://github.com/indutny/bn.js/) repersenting the UNIX Timestamp when the lock is made available.

**Returns:** *BN*

___

###  getSpenders

▸ **getSpenders**(`addresses`: Buffer[], `asOf`: BN): *Buffer[]*

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

###  meetsThreshold

▸ **meetsThreshold**(`addresses`: Buffer[], `asOf`: BN): *boolean*

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

*Defined in [src/common/output.ts:343](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L343)*

Returns the buffer representing the [Output](common_output.output.md) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Defined in [src/common/output.ts:360](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L360)*

Returns a base-58 string representing the [Output](common_output.output.md).

**Returns:** *string*

___

### `Static` fromArray

▸ **fromArray**(`b`: Buffer): *[OutputOwners](common_output.outputowners.md)[]*

*Defined in [src/common/output.ts:395](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L395)*

**Parameters:**

Name | Type |
------ | ------ |
`b` | Buffer |

**Returns:** *[OutputOwners](common_output.outputowners.md)[]*

___

### `Static` toArray

▸ **toArray**(`o`: [OutputOwners](common_output.outputowners.md)[]): *Buffer*

*Defined in [src/common/output.ts:407](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L407)*

**Parameters:**

Name | Type |
------ | ------ |
`o` | [OutputOwners](common_output.outputowners.md)[] |

**Returns:** *Buffer*
