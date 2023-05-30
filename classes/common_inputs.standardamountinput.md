[@c4tplatform/caminojs](../api.md) › [Common-Inputs](../modules/common_inputs.md) › [StandardAmountInput](common_inputs.standardamountinput.md)

# Class: StandardAmountInput

An [Input](common_inputs.input.md) class which specifies a token amount .

## Hierarchy

  ↳ [Input](common_inputs.input.md)

  ↳ **StandardAmountInput**

  ↳ [AmountInput](api_evm_inputs.amountinput.md)

  ↳ [AmountInput](api_avm_inputs.amountinput.md)

  ↳ [AmountInput](api_platformvm_inputs.amountinput.md)

## Index

### Constructors

* [constructor](common_inputs.standardamountinput.md#constructor)

### Properties

* [_codecID](common_inputs.standardamountinput.md#protected-_codecid)
* [_typeID](common_inputs.standardamountinput.md#protected-_typeid)
* [_typeName](common_inputs.standardamountinput.md#protected-_typename)
* [amount](common_inputs.standardamountinput.md#protected-amount)
* [amountValue](common_inputs.standardamountinput.md#protected-amountvalue)
* [sigCount](common_inputs.standardamountinput.md#protected-sigcount)
* [sigIdxs](common_inputs.standardamountinput.md#protected-sigidxs)

### Methods

* [addSignatureIdx](common_inputs.standardamountinput.md#addsignatureidx)
* [clone](common_inputs.standardamountinput.md#abstract-clone)
* [create](common_inputs.standardamountinput.md#abstract-create)
* [deserialize](common_inputs.standardamountinput.md#deserialize)
* [fromBuffer](common_inputs.standardamountinput.md#frombuffer)
* [getAmount](common_inputs.standardamountinput.md#getamount)
* [getCodecID](common_inputs.standardamountinput.md#getcodecid)
* [getCredentialID](common_inputs.standardamountinput.md#abstract-getcredentialid)
* [getInput](common_inputs.standardamountinput.md#getinput)
* [getInputID](common_inputs.standardamountinput.md#abstract-getinputid)
* [getSigIdxs](common_inputs.standardamountinput.md#getsigidxs)
* [getTypeID](common_inputs.standardamountinput.md#gettypeid)
* [getTypeName](common_inputs.standardamountinput.md#gettypename)
* [sanitizeObject](common_inputs.standardamountinput.md#sanitizeobject)
* [select](common_inputs.standardamountinput.md#abstract-select)
* [serialize](common_inputs.standardamountinput.md#serialize)
* [toBuffer](common_inputs.standardamountinput.md#tobuffer)
* [toString](common_inputs.standardamountinput.md#tostring)

## Constructors

###  constructor

\+ **new StandardAmountInput**(`amount`: BN): *[StandardAmountInput](common_inputs.standardamountinput.md)*

*Defined in [src/common/input.ts:406](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L406)*

An [AmountInput](api_evm_inputs.amountinput.md) class which issues a payment on an assetID.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the input  |

**Returns:** *[StandardAmountInput](common_inputs.standardamountinput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Input](common_inputs.input.md).[_typeID](common_inputs.input.md#protected-_typeid)*

*Defined in [src/common/input.ts:353](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L353)*

___

### `Protected` _typeName

• **_typeName**: *string* = "StandardAmountInput"

*Overrides [Input](common_inputs.input.md).[_typeName](common_inputs.input.md#protected-_typename)*

*Defined in [src/common/input.ts:352](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L352)*

___

### `Protected` amount

• **amount**: *Buffer* = Buffer.alloc(8)

*Defined in [src/common/input.ts:380](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L380)*

___

### `Protected` amountValue

• **amountValue**: *BN* = new BN(0)

*Defined in [src/common/input.ts:381](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L381)*

___

### `Protected` sigCount

• **sigCount**: *Buffer* = Buffer.alloc(4)

*Inherited from [Input](common_inputs.input.md).[sigCount](common_inputs.input.md#protected-sigcount)*

*Defined in [src/common/input.ts:82](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L82)*

___

### `Protected` sigIdxs

• **sigIdxs**: *[SigIdx](common_signature.sigidx.md)[]* = []

*Inherited from [Input](common_inputs.input.md).[sigIdxs](common_inputs.input.md#protected-sigidxs)*

*Defined in [src/common/input.ts:83](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L83)*

## Methods

###  addSignatureIdx

▸ **addSignatureIdx**(`addressIdx`: number, `address`: Buffer): *void*

*Inherited from [Input](common_inputs.input.md).[addSignatureIdx](common_inputs.input.md#addsignatureidx)*

*Defined in [src/common/input.ts:104](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L104)*

Creates and adds a [SigIdx](common_signature.sigidx.md) to the [Input](common_inputs.input.md).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`addressIdx` | number | The index of the address to reference in the signatures |
`address` | Buffer | The address of the source of the signature  |

**Returns:** *void*

___

### `Abstract` clone

▸ **clone**(): *this*

*Inherited from [Input](common_inputs.input.md).[clone](common_inputs.input.md#abstract-clone)*

*Defined in [src/common/input.ts:148](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L148)*

**Returns:** *this*

___

### `Abstract` create

▸ **create**(...`args`: any[]): *this*

*Inherited from [Input](common_inputs.input.md).[create](common_inputs.input.md#abstract-create)*

*Defined in [src/common/input.ts:150](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L150)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Overrides [Input](common_inputs.input.md).[deserialize](common_inputs.input.md#deserialize)*

*Defined in [src/common/input.ts:368](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L368)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [Input](common_inputs.input.md).[fromBuffer](common_inputs.input.md#frombuffer)*

*Defined in [src/common/input.ts:391](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L391)*

Popuates the instance from a [Buffer](https://github.com/feross/buffer) representing the [AmountInput](api_evm_inputs.amountinput.md) and returns the size of the input.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAmount

▸ **getAmount**(): *BN*

*Defined in [src/common/input.ts:386](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L386)*

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

### `Abstract` getCredentialID

▸ **getCredentialID**(): *number*

*Inherited from [Input](common_inputs.input.md).[getCredentialID](common_inputs.input.md#abstract-getcredentialid)*

*Defined in [src/common/input.ts:96](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L96)*

**Returns:** *number*

___

###  getInput

▸ **getInput**(): *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [Input](common_inputs.input.md).[getInput](common_inputs.input.md#getinput)*

*Defined in [src/common/input.ts:85](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L85)*

**Returns:** *[BaseInput](../interfaces/common_inputs.baseinput.md)*

___

### `Abstract` getInputID

▸ **getInputID**(): *number*

*Inherited from [Input](common_inputs.input.md).[getInputID](common_inputs.input.md#abstract-getinputid)*

*Defined in [src/common/input.ts:89](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L89)*

**Returns:** *number*

___

###  getSigIdxs

▸ **getSigIdxs**(): *[SigIdx](common_signature.sigidx.md)[]*

*Inherited from [Input](common_inputs.input.md).[getSigIdxs](common_inputs.input.md#getsigidxs)*

*Defined in [src/common/input.ts:94](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L94)*

Returns the array of [SigIdx](common_signature.sigidx.md) for this [Input](common_inputs.input.md)

**Returns:** *[SigIdx](common_signature.sigidx.md)[]*

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

### `Abstract` select

▸ **select**(`id`: number, ...`args`: any[]): *[BaseInput](../interfaces/common_inputs.baseinput.md)*

*Inherited from [Input](common_inputs.input.md).[select](common_inputs.input.md#abstract-select)*

*Defined in [src/common/input.ts:152](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L152)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *[BaseInput](../interfaces/common_inputs.baseinput.md)*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Overrides [Input](common_inputs.input.md).[serialize](common_inputs.input.md#serialize)*

*Defined in [src/common/input.ts:355](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L355)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [Input](common_inputs.input.md).[toBuffer](common_inputs.input.md#tobuffer)*

*Defined in [src/common/input.ts:401](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L401)*

Returns the buffer representing the [AmountInput](api_evm_inputs.amountinput.md) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [Input](common_inputs.input.md).[toString](common_inputs.input.md#tostring)*

*Defined in [src/common/input.ts:144](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L144)*

Returns a base-58 representation of the [Input](common_inputs.input.md).

**Returns:** *string*
