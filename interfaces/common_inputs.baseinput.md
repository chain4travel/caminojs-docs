[@c4tplatform/caminojs](../api.md) › [Common-Inputs](../modules/common_inputs.md) › [BaseInput](common_inputs.baseinput.md)

# Interface: BaseInput

## Hierarchy

* **BaseInput**

## Index

### Methods

* [addSignatureIdx](common_inputs.baseinput.md#addsignatureidx)
* [clone](common_inputs.baseinput.md#clone)
* [create](common_inputs.baseinput.md#create)
* [deserialize](common_inputs.baseinput.md#deserialize)
* [fromBuffer](common_inputs.baseinput.md#frombuffer)
* [getCredentialID](common_inputs.baseinput.md#getcredentialid)
* [getInput](common_inputs.baseinput.md#getinput)
* [getInputID](common_inputs.baseinput.md#getinputid)
* [getSigIdxs](common_inputs.baseinput.md#getsigidxs)
* [getTypeID](common_inputs.baseinput.md#gettypeid)
* [serialize](common_inputs.baseinput.md#serialize)
* [toBuffer](common_inputs.baseinput.md#tobuffer)

## Methods

###  addSignatureIdx

▸ **addSignatureIdx**(`addressIdx`: number, `address`: Buffer): *void*

*Defined in [src/common/input.ts:32](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L32)*

**Parameters:**

Name | Type |
------ | ------ |
`addressIdx` | number |
`address` | Buffer |

**Returns:** *void*

___

###  clone

▸ **clone**(): *this*

*Defined in [src/common/input.ts:35](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L35)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/common/input.ts:36](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L36)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Defined in [src/common/input.ts:25](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L25)*

**Parameters:**

Name | Type |
------ | ------ |
`fields` | object |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Defined in [src/common/input.ts:26](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L26)*

**Parameters:**

Name | Type |
------ | ------ |
`bytes` | Buffer |
`offset` | number |

**Returns:** *number*

___

###  getCredentialID

▸ **getCredentialID**(): *number*

*Defined in [src/common/input.ts:31](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L31)*

**Returns:** *number*

___

###  getInput

▸ **getInput**(): *[BaseInput](common_inputs.baseinput.md)*

*Defined in [src/common/input.ts:29](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L29)*

**Returns:** *[BaseInput](common_inputs.baseinput.md)*

___

###  getInputID

▸ **getInputID**(): *number*

*Defined in [src/common/input.ts:30](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L30)*

**Returns:** *number*

___

###  getSigIdxs

▸ **getSigIdxs**(): *[SigIdx](../classes/common_signature.sigidx.md)[]*

*Defined in [src/common/input.ts:33](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L33)*

**Returns:** *[SigIdx](../classes/common_signature.sigidx.md)[]*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Defined in [src/common/input.ts:22](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L22)*

**Returns:** *number*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Defined in [src/common/input.ts:24](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L24)*

**Parameters:**

Name | Type |
------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Defined in [src/common/input.ts:27](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/input.ts#L27)*

**Returns:** *Buffer*
