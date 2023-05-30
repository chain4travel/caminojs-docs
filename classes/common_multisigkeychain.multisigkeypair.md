[@c4tplatform/caminojs](../api.md) › [Common-MultisigKeyChain](../modules/common_multisigkeychain.md) › [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)

# Class: MultisigKeyPair

Class for representing a generic multi signature key.

## Hierarchy

  ↳ [StandardKeyPair](common_keychain.standardkeypair.md)

  ↳ **MultisigKeyPair**

## Index

### Constructors

* [constructor](common_multisigkeychain.multisigkeypair.md#constructor)

### Properties

* [keyChain](common_multisigkeychain.multisigkeypair.md#protected-keychain)
* [privk](common_multisigkeychain.multisigkeypair.md#protected-privk)
* [pubk](common_multisigkeychain.multisigkeypair.md#protected-pubk)

### Methods

* [clone](common_multisigkeychain.multisigkeypair.md#clone)
* [create](common_multisigkeychain.multisigkeypair.md#create)
* [generateKey](common_multisigkeychain.multisigkeypair.md#generatekey)
* [getAddress](common_multisigkeychain.multisigkeypair.md#getaddress)
* [getAddressString](common_multisigkeychain.multisigkeypair.md#getaddressstring)
* [getPrivateKey](common_multisigkeychain.multisigkeypair.md#getprivatekey)
* [getPrivateKeyString](common_multisigkeychain.multisigkeypair.md#getprivatekeystring)
* [getPublicKey](common_multisigkeychain.multisigkeypair.md#getpublickey)
* [getPublicKeyString](common_multisigkeychain.multisigkeypair.md#getpublickeystring)
* [importKey](common_multisigkeychain.multisigkeypair.md#importkey)
* [recover](common_multisigkeychain.multisigkeypair.md#recover)
* [sign](common_multisigkeychain.multisigkeypair.md#sign)
* [verify](common_multisigkeychain.multisigkeypair.md#verify)

## Constructors

###  constructor

\+ **new MultisigKeyPair**(`keyChain`: [MultisigKeyChain](common_multisigkeychain.multisigkeychain.md), `address`: Buffer, `signature`: Buffer): *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)*

*Defined in [src/common/multisigkeychain.ts:87](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L87)*

**Parameters:**

Name | Type |
------ | ------ |
`keyChain` | [MultisigKeyChain](common_multisigkeychain.multisigkeychain.md) |
`address` | Buffer |
`signature` | Buffer |

**Returns:** *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)*

## Properties

### `Protected` keyChain

• **keyChain**: *[MultisigKeyChain](common_multisigkeychain.multisigkeychain.md)*

*Defined in [src/common/multisigkeychain.ts:33](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L33)*

___

### `Protected` privk

• **privk**: *Buffer*

*Inherited from [StandardKeyPair](common_keychain.standardkeypair.md).[privk](common_keychain.standardkeypair.md#protected-privk)*

*Overrides [SignerKeyPair](common_keychain.signerkeypair.md).[privk](common_keychain.signerkeypair.md#protected-privk)*

*Defined in [src/common/keychain.ts:31](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L31)*

___

### `Protected` pubk

• **pubk**: *Buffer*

*Inherited from [StandardKeyPair](common_keychain.standardkeypair.md).[pubk](common_keychain.standardkeypair.md#protected-pubk)*

*Overrides [SignerKeyPair](common_keychain.signerkeypair.md).[pubk](common_keychain.signerkeypair.md#protected-pubk)*

*Defined in [src/common/keychain.ts:30](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L30)*

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[clone](common_keychain.standardkeypair.md#abstract-clone)*

*Defined in [src/common/multisigkeychain.ts:77](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L77)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[create](common_keychain.standardkeypair.md#abstract-create)*

*Defined in [src/common/multisigkeychain.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L70)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  generateKey

▸ **generateKey**(): *void*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[generateKey](common_keychain.standardkeypair.md#abstract-generatekey)*

*Defined in [src/common/multisigkeychain.ts:35](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L35)*

**Returns:** *void*

___

###  getAddress

▸ **getAddress**(): *Buffer*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[getAddress](common_keychain.standardkeypair.md#abstract-getaddress)*

*Defined in [src/common/multisigkeychain.ts:55](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L55)*

**Returns:** *Buffer*

___

###  getAddressString

▸ **getAddressString**(): *string*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[getAddressString](common_keychain.standardkeypair.md#abstract-getaddressstring)*

*Defined in [src/common/multisigkeychain.ts:59](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L59)*

**Returns:** *string*

___

###  getPrivateKey

▸ **getPrivateKey**(): *Buffer*

*Inherited from [StandardKeyPair](common_keychain.standardkeypair.md).[getPrivateKey](common_keychain.standardkeypair.md#getprivatekey)*

*Defined in [src/common/keychain.ts:77](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L77)*

Returns a reference to the private key.

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the private key

___

###  getPrivateKeyString

▸ **getPrivateKeyString**(): *string*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[getPrivateKeyString](common_keychain.standardkeypair.md#abstract-getprivatekeystring)*

*Defined in [src/common/multisigkeychain.ts:81](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L81)*

**Returns:** *string*

___

###  getPublicKey

▸ **getPublicKey**(): *Buffer*

*Inherited from [StandardKeyPair](common_keychain.standardkeypair.md).[getPublicKey](common_keychain.standardkeypair.md#getpublickey)*

*Defined in [src/common/keychain.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L86)*

Returns a reference to the public key.

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the public key

___

###  getPublicKeyString

▸ **getPublicKeyString**(): *string*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[getPublicKeyString](common_keychain.standardkeypair.md#abstract-getpublickeystring)*

*Defined in [src/common/multisigkeychain.ts:85](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L85)*

**Returns:** *string*

___

###  importKey

▸ **importKey**(`_`: Buffer): *boolean*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[importKey](common_keychain.standardkeypair.md#abstract-importkey)*

*Defined in [src/common/multisigkeychain.ts:39](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L39)*

**Parameters:**

Name | Type |
------ | ------ |
`_` | Buffer |

**Returns:** *boolean*

___

###  recover

▸ **recover**(`msg`: Buffer, `sig`: Buffer): *Buffer*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[recover](common_keychain.standardkeypair.md#abstract-recover)*

*Defined in [src/common/multisigkeychain.ts:47](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L47)*

**Parameters:**

Name | Type |
------ | ------ |
`msg` | Buffer |
`sig` | Buffer |

**Returns:** *Buffer*

___

###  sign

▸ **sign**(`_`: Buffer): *Buffer*

*Overrides [SignerKeyPair](common_keychain.signerkeypair.md).[sign](common_keychain.signerkeypair.md#abstract-sign)*

*Defined in [src/common/multisigkeychain.ts:43](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L43)*

**Parameters:**

Name | Type |
------ | ------ |
`_` | Buffer |

**Returns:** *Buffer*

___

###  verify

▸ **verify**(`msg`: Buffer, `sig`: Buffer): *boolean*

*Overrides [StandardKeyPair](common_keychain.standardkeypair.md).[verify](common_keychain.standardkeypair.md#abstract-verify)*

*Defined in [src/common/multisigkeychain.ts:51](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L51)*

**Parameters:**

Name | Type |
------ | ------ |
`msg` | Buffer |
`sig` | Buffer |

**Returns:** *boolean*
