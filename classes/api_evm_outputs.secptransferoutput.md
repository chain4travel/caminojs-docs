[@c4tplatform/caminojs](../README.md) › [API-EVM-Outputs](../modules/api_evm_outputs.md) › [SECPTransferOutput](api_evm_outputs.secptransferoutput.md)

# Class: SECPTransferOutput

An [Output](../modules/src_common.md#output) class which specifies an Output that carries an ammount for an assetID and uses secp256k1 signature scheme.

## Hierarchy

  ↳ [AmountOutput](api_evm_outputs.amountoutput.md)

  ↳ **SECPTransferOutput**

## Index

### Constructors

* [constructor](api_evm_outputs.secptransferoutput.md#constructor)

### Properties

* [_codecID](api_evm_outputs.secptransferoutput.md#protected-_codecid)
* [_typeID](api_evm_outputs.secptransferoutput.md#protected-_typeid)
* [_typeName](api_evm_outputs.secptransferoutput.md#protected-_typename)
* [addresses](api_evm_outputs.secptransferoutput.md#protected-addresses)
* [amount](api_evm_outputs.secptransferoutput.md#protected-amount)
* [amountValue](api_evm_outputs.secptransferoutput.md#protected-amountvalue)
* [locktime](api_evm_outputs.secptransferoutput.md#protected-locktime)
* [numaddrs](api_evm_outputs.secptransferoutput.md#protected-numaddrs)
* [threshold](api_evm_outputs.secptransferoutput.md#protected-threshold)

### Methods

* [clone](api_evm_outputs.secptransferoutput.md#clone)
* [create](api_evm_outputs.secptransferoutput.md#create)
* [deserialize](api_evm_outputs.secptransferoutput.md#deserialize)
* [fromBuffer](api_evm_outputs.secptransferoutput.md#frombuffer)
* [getAddress](api_evm_outputs.secptransferoutput.md#getaddress)
* [getAddressIdx](api_evm_outputs.secptransferoutput.md#getaddressidx)
* [getAddresses](api_evm_outputs.secptransferoutput.md#getaddresses)
* [getAmount](api_evm_outputs.secptransferoutput.md#getamount)
* [getCodecID](api_evm_outputs.secptransferoutput.md#getcodecid)
* [getLocktime](api_evm_outputs.secptransferoutput.md#getlocktime)
* [getOutputID](api_evm_outputs.secptransferoutput.md#getoutputid)
* [getSpenders](api_evm_outputs.secptransferoutput.md#getspenders)
* [getThreshold](api_evm_outputs.secptransferoutput.md#getthreshold)
* [getTypeID](api_evm_outputs.secptransferoutput.md#gettypeid)
* [getTypeName](api_evm_outputs.secptransferoutput.md#gettypename)
* [makeTransferable](api_evm_outputs.secptransferoutput.md#maketransferable)
* [meetsThreshold](api_evm_outputs.secptransferoutput.md#meetsthreshold)
* [sanitizeObject](api_evm_outputs.secptransferoutput.md#sanitizeobject)
* [select](api_evm_outputs.secptransferoutput.md#select)
* [serialize](api_evm_outputs.secptransferoutput.md#serialize)
* [toBuffer](api_evm_outputs.secptransferoutput.md#tobuffer)
* [toString](api_evm_outputs.secptransferoutput.md#tostring)

## Constructors

###  constructor

\+ **new SECPTransferOutput**(`amount`: BN, `addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[SECPTransferOutput](api_evm_outputs.secptransferoutput.md)*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[constructor](common_output.standardamountoutput.md#constructor)*

*Overrides [OutputOwners](common_output.outputowners.md).[constructor](common_output.outputowners.md#constructor)*

*Defined in [src/common/output.ts:591](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L591)*

A [StandardAmountOutput](../modules/src_common.md#standardamountoutput) class which issues a payment on an assetID.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the output |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the the threshold number of signers required to sign the transaction  |

**Returns:** *[SECPTransferOutput](api_evm_outputs.secptransferoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *number* = EVMConstants.SECPXFEROUTPUTID

*Overrides [AmountOutput](api_evm_outputs.amountoutput.md).[_typeID](api_evm_outputs.amountoutput.md#protected-_typeid)*

*Defined in [src/apis/evm/outputs.ts:86](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L86)*

___

### `Protected` _typeName

• **_typeName**: *string* = "SECPTransferOutput"

*Overrides [AmountOutput](api_evm_outputs.amountoutput.md).[_typeName](api_evm_outputs.amountoutput.md#protected-_typename)*

*Defined in [src/apis/evm/outputs.ts:85](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L85)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Inherited from [OutputOwners](common_output.outputowners.md).[addresses](common_output.outputowners.md#protected-addresses)*

*Defined in [src/common/output.ts:198](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L198)*

___

### `Protected` amount

• **amount**: *Buffer* = Buffer.alloc(8)

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[amount](common_output.standardamountoutput.md#protected-amount)*

*Defined in [src/common/output.ts:562](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L562)*

___

### `Protected` amountValue

• **amountValue**: *BN* = new BN(0)

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[amountValue](common_output.standardamountoutput.md#protected-amountvalue)*

*Defined in [src/common/output.ts:563](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L563)*

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

*Defined in [src/apis/evm/outputs.ts:101](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L101)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [Output](common_output.output.md).[create](common_output.output.md#abstract-create)*

*Defined in [src/apis/evm/outputs.ts:97](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L97)*

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

*Defined in [src/common/output.ts:550](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L550)*

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

*Defined in [src/common/output.ts:575](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L575)*

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

###  getAmount

▸ **getAmount**(): *BN*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[getAmount](common_output.standardamountoutput.md#getamount)*

*Defined in [src/common/output.ts:568](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L568)*

Returns the amount as a [BN](https://github.com/indutny/bn.js/).

**Returns:** *BN*

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

*Defined in [src/apis/evm/outputs.ts:93](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L93)*

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

▸ **makeTransferable**(`assetID`: Buffer): *[TransferableOutput](api_evm_outputs.transferableoutput.md)*

*Inherited from [AmountOutput](api_evm_outputs.amountoutput.md).[makeTransferable](api_evm_outputs.amountoutput.md#maketransferable)*

*Overrides [Output](common_output.output.md).[makeTransferable](common_output.output.md#abstract-maketransferable)*

*Defined in [src/apis/evm/outputs.ts:72](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L72)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  |

**Returns:** *[TransferableOutput](api_evm_outputs.transferableoutput.md)*

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

###  select

▸ **select**(`id`: number, ...`args`: any[]): *[Output](common_output.output.md)*

*Inherited from [AmountOutput](api_evm_outputs.amountoutput.md).[select](api_evm_outputs.amountoutput.md#select)*

*Defined in [src/apis/evm/outputs.ts:76](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/evm/outputs.ts#L76)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *[Output](common_output.output.md)*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Inherited from [StandardAmountOutput](common_output.standardamountoutput.md).[serialize](common_output.standardamountoutput.md#serialize)*

*Overrides [OutputOwners](common_output.outputowners.md).[serialize](common_output.outputowners.md#serialize)*

*Defined in [src/common/output.ts:537](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L537)*

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

*Defined in [src/common/output.ts:585](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L585)*

Returns the buffer representing the [StandardAmountOutput](../modules/src_common.md#standardamountoutput) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [OutputOwners](common_output.outputowners.md).[toString](common_output.outputowners.md#tostring)*

*Defined in [src/common/output.ts:355](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L355)*

Returns a base-58 string representing the [Output](../modules/src_common.md#output).

**Returns:** *string*
