[@c4tplatform/caminojs](../api.md) › [Common-Signature](../modules/common_signature.md) › [SECPMultisigCredential](common_signature.secpmultisigcredential.md)

# Class: SECPMultisigCredential

## Hierarchy

  ↳ [Credential](common_signature.credential.md)

  ↳ **SECPMultisigCredential**

## Index

### Constructors

* [constructor](common_signature.secpmultisigcredential.md#constructor)

### Properties

* [_codecID](common_signature.secpmultisigcredential.md#protected-_codecid)
* [_typeID](common_signature.secpmultisigcredential.md#protected-_typeid)
* [_typeName](common_signature.secpmultisigcredential.md#protected-_typename)
* [sigArray](common_signature.secpmultisigcredential.md#protected-sigarray)
* [sigIdxs](common_signature.secpmultisigcredential.md#protected-sigidxs)

### Methods

* [addSSignatureIndex](common_signature.secpmultisigcredential.md#addssignatureindex)
* [addSignature](common_signature.secpmultisigcredential.md#addsignature)
* [clone](common_signature.secpmultisigcredential.md#clone)
* [create](common_signature.secpmultisigcredential.md#create)
* [deserialize](common_signature.secpmultisigcredential.md#deserialize)
* [fromBuffer](common_signature.secpmultisigcredential.md#frombuffer)
* [getCodecID](common_signature.secpmultisigcredential.md#getcodecid)
* [getCredentialID](common_signature.secpmultisigcredential.md#getcredentialid)
* [getTypeID](common_signature.secpmultisigcredential.md#gettypeid)
* [getTypeName](common_signature.secpmultisigcredential.md#gettypename)
* [sanitizeObject](common_signature.secpmultisigcredential.md#sanitizeobject)
* [select](common_signature.secpmultisigcredential.md#select)
* [serialize](common_signature.secpmultisigcredential.md#serialize)
* [setCodecID](common_signature.secpmultisigcredential.md#setcodecid)
* [toBuffer](common_signature.secpmultisigcredential.md#tobuffer)

## Constructors

###  constructor

\+ **new SECPMultisigCredential**(`typeID`: number, `sigIdxs?`: [SigIdx](common_signature.sigidx.md)[], `sigarray?`: [Signature](common_signature.signature.md)[]): *[SECPMultisigCredential](common_signature.secpmultisigcredential.md)*

*Overrides [Credential](common_signature.credential.md).[constructor](common_signature.credential.md#constructor)*

*Defined in [src/common/credentials.ts:255](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L255)*

**Parameters:**

Name | Type |
------ | ------ |
`typeID` | number |
`sigIdxs?` | [SigIdx](common_signature.sigidx.md)[] |
`sigarray?` | [Signature](common_signature.signature.md)[] |

**Returns:** *[SECPMultisigCredential](common_signature.secpmultisigcredential.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L51)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [Credential](common_signature.credential.md).[_typeID](common_signature.credential.md#protected-_typeid)*

*Defined in [src/common/credentials.ts:198](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L198)*

___

### `Protected` _typeName

• **_typeName**: *string* = "SECPMultisigCredential"

*Overrides [Credential](common_signature.credential.md).[_typeName](common_signature.credential.md#protected-_typename)*

*Defined in [src/common/credentials.ts:197](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L197)*

___

### `Protected` sigArray

• **sigArray**: *[Signature](common_signature.signature.md)[]* = []

*Inherited from [Credential](common_signature.credential.md).[sigArray](common_signature.credential.md#protected-sigarray)*

*Defined in [src/common/credentials.ts:135](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L135)*

___

### `Protected` sigIdxs

• **sigIdxs**: *[SigIdx](common_signature.sigidx.md)[]* = []

*Defined in [src/common/credentials.ts:200](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L200)*

## Methods

###  addSSignatureIndex

▸ **addSSignatureIndex**(`sigIdx`: [SigIdx](common_signature.sigidx.md)): *void*

*Defined in [src/common/credentials.ts:205](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L205)*

Adds a SignatureIndex to the credentials.

**Parameters:**

Name | Type |
------ | ------ |
`sigIdx` | [SigIdx](common_signature.sigidx.md) |

**Returns:** *void*

___

###  addSignature

▸ **addSignature**(`sig`: [Signature](common_signature.signature.md)): *number*

*Inherited from [Credential](common_signature.credential.md).[addSignature](common_signature.credential.md#addsignature)*

*Defined in [src/common/credentials.ts:152](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L152)*

Adds a signature to the credentials and returns the index off the added signature.

**Parameters:**

Name | Type |
------ | ------ |
`sig` | [Signature](common_signature.signature.md) |

**Returns:** *number*

___

###  clone

▸ **clone**(): *this*

*Overrides [Credential](common_signature.credential.md).[clone](common_signature.credential.md#abstract-clone)*

*Defined in [src/common/credentials.ts:209](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L209)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [Credential](common_signature.credential.md).[create](common_signature.credential.md#abstract-create)*

*Defined in [src/common/credentials.ts:215](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L215)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Inherited from [Credential](common_signature.credential.md).[deserialize](common_signature.credential.md#deserialize)*

*Overrides [StandardParseableInput](common_inputs.standardparseableinput.md).[deserialize](common_inputs.standardparseableinput.md#deserialize)*

*Defined in [src/common/credentials.ts:126](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L126)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [Credential](common_signature.credential.md).[fromBuffer](common_signature.credential.md#frombuffer)*

*Defined in [src/common/credentials.ts:225](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L225)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/serialization.ts#L70)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getCredentialID

▸ **getCredentialID**(): *number*

*Inherited from [Credential](common_signature.credential.md).[getCredentialID](common_signature.credential.md#getcredentialid)*

*Defined in [src/common/credentials.ts:137](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L137)*

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

###  select

▸ **select**(`id`: number, ...`args`: any[]): *[Credential](common_signature.credential.md)*

*Overrides [Credential](common_signature.credential.md).[select](common_signature.credential.md#abstract-select)*

*Defined in [src/common/credentials.ts:221](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L221)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *[Credential](common_signature.credential.md)*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Inherited from [Credential](common_signature.credential.md).[serialize](common_signature.credential.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/credentials.ts:119](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L119)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  setCodecID

▸ **setCodecID**(`codecID`: number): *void*

*Inherited from [Credential](common_signature.credential.md).[setCodecID](common_signature.credential.md#setcodecid)*

*Defined in [src/common/credentials.ts:147](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L147)*

Set the codecID

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`codecID` | number | The codecID to set  |

**Returns:** *void*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [Credential](common_signature.credential.md).[toBuffer](common_signature.credential.md#tobuffer)*

*Defined in [src/common/credentials.ts:240](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/credentials.ts#L240)*

**Returns:** *Buffer*
