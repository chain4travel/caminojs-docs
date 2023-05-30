[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Outputs](../modules/api_platformvm_outputs.md) › [AmountOutput](api_platformvm_outputs.amountoutput.md)

# Class: AmountOutput

## Hierarchy

  ↳ [StandardAmountOutput](common_output.standardamountoutput.md)

  ↳ **AmountOutput**

  ↳ [SECPTransferOutput](api_platformvm_outputs.secptransferoutput.md)

## Index

### Constructors

* [constructor](api_platformvm_outputs.amountoutput.md#constructor)

### Properties

* [_codecID](api_platformvm_outputs.amountoutput.md#protected-_codecid)
* [_typeID](api_platformvm_outputs.amountoutput.md#protected-_typeid)
* [_typeName](api_platformvm_outputs.amountoutput.md#protected-_typename)
* [addresses](api_platformvm_outputs.amountoutput.md#protected-addresses)
* [amount](api_platformvm_outputs.amountoutput.md#protected-amount)
* [amountValue](api_platformvm_outputs.amountoutput.md#protected-amountvalue)
* [locktime](api_platformvm_outputs.amountoutput.md#protected-locktime)
* [numaddrs](api_platformvm_outputs.amountoutput.md#protected-numaddrs)
* [threshold](api_platformvm_outputs.amountoutput.md#protected-threshold)

### Methods

* [clone](api_platformvm_outputs.amountoutput.md#abstract-clone)
* [create](api_platformvm_outputs.amountoutput.md#abstract-create)
* [deserialize](api_platformvm_outputs.amountoutput.md#deserialize)
* [fromBuffer](api_platformvm_outputs.amountoutput.md#frombuffer)
* [getAddress](api_platformvm_outputs.amountoutput.md#getaddress)
* [getAddressIdx](api_platformvm_outputs.amountoutput.md#getaddressidx)
* [getAddresses](api_platformvm_outputs.amountoutput.md#getaddresses)
* [getAddressesLength](api_platformvm_outputs.amountoutput.md#getaddresseslength)
* [getAmount](api_platformvm_outputs.amountoutput.md#getamount)
* [getCodecID](api_platformvm_outputs.amountoutput.md#getcodecid)
* [getLocktime](api_platformvm_outputs.amountoutput.md#getlocktime)
* [getOutputID](api_platformvm_outputs.amountoutput.md#abstract-getoutputid)
* [getSpenders](api_platformvm_outputs.amountoutput.md#getspenders)
* [getThreshold](api_platformvm_outputs.amountoutput.md#getthreshold)
* [getTypeID](api_platformvm_outputs.amountoutput.md#gettypeid)
* [getTypeName](api_platformvm_outputs.amountoutput.md#gettypename)
* [makeTransferable](api_platformvm_outputs.amountoutput.md#maketransferable)
* [meetsThreshold](api_platformvm_outputs.amountoutput.md#meetsthreshold)
* [sanitizeObject](api_platformvm_outputs.amountoutput.md#sanitizeobject)
* [serialize](api_platformvm_outputs.amountoutput.md#serialize)
* [toBuffer](api_platformvm_outputs.amountoutput.md#tobuffer)
* [toString](api_platformvm_outputs.amountoutput.md#tostring)
* [fromArray](api_platformvm_outputs.amountoutput.md#static-fromarray)
* [toArray](api_platformvm_outputs.amountoutput.md#static-toarray)

## Constructors

###  constructor

\+ **new AmountOutput**(`amount`: BN, `addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[AmountOutput](api_platformvm_outputs.amountoutput.md)*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[constructor](common_output.standardamountoutput.md#constructor)*

*Overrides [OutputOwners](common_output.outputowners.md).[constructor](common_output.outputowners.md#constructor)*

*Defined in [src/common/output.ts:621](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L621)*

A [StandardAmountOutput](../modules/src_common.md#standardamountoutput) class which issues a payment on an assetID.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the output |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the the threshold number of signers required to sign the transaction  |

**Returns:** *[AmountOutput](api_platformvm_outputs.amountoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardAmountOutput](common_output.standardamountoutput.md).[_typeID](common_output.standardamountoutput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/outputs.ts:112](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L112)*

___

### `Protected` _typeName

• **_typeName**: *string* = "AmountOutput"

*Overrides [StandardAmountOutput](common_output.standardamountoutput.md).[_typeName](common_output.standardamountoutput.md#protected-_typename)*

*Defined in [src/apis/platformvm/outputs.ts:111](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L111)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Inherited from [OutputOwners](common_output.outputowners.md).[addresses](common_output.outputowners.md#protected-addresses)*

*Defined in [src/common/output.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L198)*

___

### `Protected` amount

• **amount**: *Buffer* = Buffer.alloc(8)

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[amount](common_output.standardamountoutput.md#protected-amount)*

*Defined in [src/common/output.ts:592](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L592)*

___

### `Protected` amountValue

• **amountValue**: *BN* = new BN(0)

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[amountValue](common_output.standardamountoutput.md#protected-amountvalue)*

*Defined in [src/common/output.ts:593](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L593)*

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

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[deserialize](common_output.standardamountoutput.md#deserialize)*

*Overrides [OutputOwners](common_output.outputowners.md).[deserialize](common_output.outputowners.md#deserialize)*

*Defined in [src/common/output.ts:580](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L580)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`outbuff`: Buffer, `offset`: number): *number*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[fromBuffer](common_output.standardamountoutput.md#frombuffer)*

*Overrides [OutputOwners](common_output.outputowners.md).[fromBuffer](common_output.outputowners.md#frombuffer)*

*Defined in [src/common/output.ts:605](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L605)*

Popuates the instance from a [Buffer](https://github.com/feross/buffer) representing the [StandardAmountOutput](../modules/src_common.md#standardamountoutput) and returns the size of the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`outbuff` | Buffer | - |
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

###  getAmount

▸ **getAmount**(): *BN*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[getAmount](common_output.standardamountoutput.md#getamount)*

*Defined in [src/common/output.ts:598](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L598)*

Returns the amount as a [BN](https://github.com/indutny/bn.js/).

**Returns:** *BN*

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

###  makeTransferable

▸ **makeTransferable**(`assetID`: Buffer): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

*Overrides [Output](common_output.output.md).[makeTransferable](common_output.output.md#abstract-maketransferable)*

*Defined in [src/apis/platformvm/outputs.ts:119](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/outputs.ts#L119)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  |

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

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

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[serialize](common_output.standardamountoutput.md#serialize)*

*Overrides [OutputOwners](common_output.outputowners.md).[serialize](common_output.outputowners.md#serialize)*

*Defined in [src/common/output.ts:567](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L567)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[toBuffer](common_output.standardamountoutput.md#tobuffer)*

*Overrides [OutputOwners](common_output.outputowners.md).[toBuffer](common_output.outputowners.md#tobuffer)*

*Defined in [src/common/output.ts:615](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L615)*

Returns the buffer representing the [StandardAmountOutput](../modules/src_common.md#standardamountoutput) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [OutputOwners](common_output.outputowners.md).[toString](common_output.outputowners.md#tostring)*

*Defined in [src/common/output.ts:360](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/output.ts#L360)*

Returns a base-58 string representing the [Output](../modules/src_common.md#output).

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
