[@c4tplatform/caminojs](../api.md) › [Common-KeyChain](../modules/common_keychain.md) › [StandardKeyPair](common_keychain.standardkeypair.md)

# Class: StandardKeyPair

Class for representing a private and public keypair in Camino.
All APIs that need key pairs should extend on this class.

## Hierarchy

* [SignerKeyPair](common_keychain.signerkeypair.md)

  ↳ **StandardKeyPair**

  ↳ [SECP256k1KeyPair](common_secp256k1keychain.secp256k1keypair.md)

  ↳ [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)

## Index

### Properties

* [privk](common_keychain.standardkeypair.md#protected-privk)
* [pubk](common_keychain.standardkeypair.md#protected-pubk)

### Methods

* [clone](common_keychain.standardkeypair.md#abstract-clone)
* [create](common_keychain.standardkeypair.md#abstract-create)
* [generateKey](common_keychain.standardkeypair.md#abstract-generatekey)
* [getAddress](common_keychain.standardkeypair.md#abstract-getaddress)
* [getAddressString](common_keychain.standardkeypair.md#abstract-getaddressstring)
* [getPrivateKey](common_keychain.standardkeypair.md#getprivatekey)
* [getPrivateKeyString](common_keychain.standardkeypair.md#abstract-getprivatekeystring)
* [getPublicKey](common_keychain.standardkeypair.md#getpublickey)
* [getPublicKeyString](common_keychain.standardkeypair.md#abstract-getpublickeystring)
* [importKey](common_keychain.standardkeypair.md#abstract-importkey)
* [recover](common_keychain.standardkeypair.md#abstract-recover)
* [sign](common_keychain.standardkeypair.md#abstract-sign)
* [verify](common_keychain.standardkeypair.md#abstract-verify)

## Properties

### `Protected` privk

• **privk**: *Buffer*

*Overrides [SignerKeyPair](common_keychain.signerkeypair.md).[privk](common_keychain.signerkeypair.md#protected-privk)*

*Defined in [src/common/keychain.ts:31](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L31)*

___

### `Protected` pubk

• **pubk**: *Buffer*

*Overrides [SignerKeyPair](common_keychain.signerkeypair.md).[pubk](common_keychain.signerkeypair.md#protected-pubk)*

*Defined in [src/common/keychain.ts:30](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L30)*

## Methods

### `Abstract` clone

▸ **clone**(): *this*

*Defined in [src/common/keychain.ts:120](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L120)*

**Returns:** *this*

___

### `Abstract` create

▸ **create**(...`args`: any[]): *this*

*Defined in [src/common/keychain.ts:118](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L118)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

### `Abstract` generateKey

▸ **generateKey**(`entropy?`: Buffer): *void*

*Defined in [src/common/keychain.ts:38](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L38)*

Generates a new keypair.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`entropy?` | Buffer | Optional parameter that may be necessary to produce secure keys  |

**Returns:** *void*

___

### `Abstract` getAddress

▸ **getAddress**(): *Buffer*

*Defined in [src/common/keychain.ts:109](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L109)*

Returns the address.

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer)  representation of the address

___

### `Abstract` getAddressString

▸ **getAddressString**(): *string*

*Defined in [src/common/keychain.ts:116](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L116)*

Returns the address's string representation.

**Returns:** *string*

A string representation of the address

___

###  getPrivateKey

▸ **getPrivateKey**(): *Buffer*

*Defined in [src/common/keychain.ts:77](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L77)*

Returns a reference to the private key.

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the private key

___

### `Abstract` getPrivateKeyString

▸ **getPrivateKeyString**(): *string*

*Defined in [src/common/keychain.ts:95](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L95)*

Returns a string representation of the private key.

**Returns:** *string*

A string representation of the public key

___

###  getPublicKey

▸ **getPublicKey**(): *Buffer*

*Defined in [src/common/keychain.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L86)*

Returns a reference to the public key.

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the public key

___

### `Abstract` getPublicKeyString

▸ **getPublicKeyString**(): *string*

*Defined in [src/common/keychain.ts:102](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L102)*

Returns the public key.

**Returns:** *string*

A string representation of the public key

___

### `Abstract` importKey

▸ **importKey**(`privk`: Buffer): *boolean*

*Defined in [src/common/keychain.ts:47](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L47)*

Imports a private key and generates the appropriate public key.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`privk` | Buffer | A [Buffer](https://github.com/feross/buffer) representing the private key  |

**Returns:** *boolean*

true on success, false on failure

___

### `Abstract` recover

▸ **recover**(`msg`: Buffer, `sig`: Buffer): *Buffer*

*Defined in [src/common/keychain.ts:58](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L58)*

Recovers the public key of a message signer from a message and its associated signature.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | The message that's signed |
`sig` | Buffer | The signature that's signed on the message  |

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the public
key of the signer

___

### `Abstract` sign

▸ **sign**(`msg`: Buffer): *Buffer*

*Inherited from [SignerKeyPair](common_keychain.signerkeypair.md).[sign](common_keychain.signerkeypair.md#abstract-sign)*

*Defined in [src/common/keychain.ts:22](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L22)*

Takes a message, signs it, and returns the signature.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | The message to sign  |

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the signature

___

### `Abstract` verify

▸ **verify**(`msg`: Buffer, `sig`: Buffer, `pubk`: Buffer): *boolean*

*Defined in [src/common/keychain.ts:70](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L70)*

Verifies that the private key associated with the provided public key produces the
signature associated with the given message.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | The message associated with the signature |
`sig` | Buffer | The signature of the signed message |
`pubk` | Buffer | The public key associated with the message signature  |

**Returns:** *boolean*

True on success, false on failure
