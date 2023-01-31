[@c4tplatform/caminojs](../README.md) › [Common-Output](../modules/common_output.md) › [BaseOutput](common_output.baseoutput.md)

# Interface: BaseOutput

## Hierarchy

* **BaseOutput**

## Index

### Methods

* [clone](common_output.baseoutput.md#clone)
* [create](common_output.baseoutput.md#create)
* [deserialize](common_output.baseoutput.md#deserialize)
* [fromBuffer](common_output.baseoutput.md#frombuffer)
* [getAddresses](common_output.baseoutput.md#getaddresses)
* [getLocktime](common_output.baseoutput.md#getlocktime)
* [getOutputID](common_output.baseoutput.md#getoutputid)
* [getThreshold](common_output.baseoutput.md#getthreshold)
* [getTypeID](common_output.baseoutput.md#gettypeid)
* [meetsThreshold](common_output.baseoutput.md#meetsthreshold)
* [serialize](common_output.baseoutput.md#serialize)
* [toBuffer](common_output.baseoutput.md#tobuffer)

## Methods

###  clone

▸ **clone**(): *this*

*Defined in [src/common/output.ts:38](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L38)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/common/output.ts:39](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L39)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Defined in [src/common/output.ts:28](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L28)*

**Parameters:**

Name | Type |
------ | ------ |
`fields` | object |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Defined in [src/common/output.ts:29](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L29)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset` | number |

**Returns:** *number*

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Defined in [src/common/output.ts:34](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L34)*

**Returns:** *Buffer[]*

___

###  getLocktime

▸ **getLocktime**(): *BN*

*Defined in [src/common/output.ts:33](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L33)*

**Returns:** *BN*

___

###  getOutputID

▸ **getOutputID**(): *number*

*Defined in [src/common/output.ts:37](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L37)*

**Returns:** *number*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Defined in [src/common/output.ts:32](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L32)*

**Returns:** *number*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Defined in [src/common/output.ts:25](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L25)*

**Returns:** *number*

___

###  meetsThreshold

▸ **meetsThreshold**(`addrs`: Buffer[], `asOf`: BN): *boolean*

*Defined in [src/common/output.ts:35](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L35)*

**Parameters:**

Name | Type |
------ | ------ |
`addrs` | Buffer[] |
`asOf` | BN |

**Returns:** *boolean*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Defined in [src/common/output.ts:27](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L27)*

**Parameters:**

Name | Type |
------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/common/output.ts:30](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L30)*

**Returns:** *Buffer*
