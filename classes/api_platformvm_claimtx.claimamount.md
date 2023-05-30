[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-ClaimTx](../modules/api_platformvm_claimtx.md) › [ClaimAmount](api_platformvm_claimtx.claimamount.md)

# Class: ClaimAmount

## Hierarchy

* **ClaimAmount**

## Index

### Constructors

* [constructor](api_platformvm_claimtx.claimamount.md#constructor)

### Properties

* [amount](api_platformvm_claimtx.claimamount.md#protected-amount)
* [auth](api_platformvm_claimtx.claimamount.md#protected-auth)
* [id](api_platformvm_claimtx.claimamount.md#protected-id)
* [type](api_platformvm_claimtx.claimamount.md#protected-type)

### Methods

* [deserialize](api_platformvm_claimtx.claimamount.md#deserialize)
* [fromBuffer](api_platformvm_claimtx.claimamount.md#frombuffer)
* [getAmount](api_platformvm_claimtx.claimamount.md#getamount)
* [getID](api_platformvm_claimtx.claimamount.md#getid)
* [getType](api_platformvm_claimtx.claimamount.md#gettype)
* [serialize](api_platformvm_claimtx.claimamount.md#serialize)
* [toBuffer](api_platformvm_claimtx.claimamount.md#tobuffer)

## Constructors

###  constructor

\+ **new ClaimAmount**(`id`: Buffer, `claimType`: [ClaimType](../enums/api_platformvm_claimtx.claimtype.md), `amount`: BN, `auth`: Buffer[]): *[ClaimAmount](api_platformvm_claimtx.claimamount.md)*

*Defined in [src/apis/platformvm/claimtx.ts:95](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L95)*

Class representing a ClaimAmount.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`id` | Buffer | undefined | Optional either depositTxID or OwnableHash, depends on claimType |
`claimType` | [ClaimType](../enums/api_platformvm_claimtx.claimtype.md) | undefined | Optional specifies the type of reward to claim |
`amount` | BN | undefined | Optional the amount to claim from this reward source  |
`auth` | Buffer[] | undefined | - |

**Returns:** *[ClaimAmount](api_platformvm_claimtx.claimamount.md)*

## Properties

### `Protected` amount

• **amount**: *Buffer‹›* = Buffer.alloc(8)

*Defined in [src/apis/platformvm/claimtx.ts:36](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L36)*

___

### `Protected` auth

• **auth**: *[SubnetAuth](api_platformvm_subnetauth.subnetauth.md)‹›* = new SubnetAuth()

*Defined in [src/apis/platformvm/claimtx.ts:37](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L37)*

___

### `Protected` id

• **id**: *Buffer‹›* = Buffer.alloc(32)

*Defined in [src/apis/platformvm/claimtx.ts:34](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L34)*

___

### `Protected` type

• **type**: *Buffer‹›* = Buffer.alloc(8)

*Defined in [src/apis/platformvm/claimtx.ts:35](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L35)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *this*

*Defined in [src/apis/platformvm/claimtx.ts:39](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L39)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *this*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Defined in [src/apis/platformvm/claimtx.ts:77](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L77)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAmount

▸ **getAmount**(): *Buffer*

*Defined in [src/apis/platformvm/claimtx.ts:124](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L124)*

**Returns:** *Buffer*

___

###  getID

▸ **getID**(): *Buffer*

*Defined in [src/apis/platformvm/claimtx.ts:118](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L118)*

**Returns:** *Buffer*

___

###  getType

▸ **getType**(): *Buffer*

*Defined in [src/apis/platformvm/claimtx.ts:121](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L121)*

**Returns:** *Buffer*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Defined in [src/apis/platformvm/claimtx.ts:59](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L59)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/claimtx.ts:89](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/claimtx.ts#L89)*

**Returns:** *Buffer*
