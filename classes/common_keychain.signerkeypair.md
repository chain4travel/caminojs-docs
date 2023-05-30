[@c4tplatform/caminojs](../api.md) › [Common-KeyChain](../modules/common_keychain.md) › [SignerKeyPair](common_keychain.signerkeypair.md)

# Class: SignerKeyPair

Class for representing an interface for signing in Camino.

## Hierarchy

* **SignerKeyPair**

  ↳ [StandardKeyPair](common_keychain.standardkeypair.md)

## Index

### Properties

* [privk](common_keychain.signerkeypair.md#protected-privk)
* [pubk](common_keychain.signerkeypair.md#protected-pubk)

### Methods

* [sign](common_keychain.signerkeypair.md#abstract-sign)

## Properties

### `Protected` privk

• **privk**: *Buffer*

*Defined in [src/common/keychain.ts:13](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L13)*

___

### `Protected` pubk

• **pubk**: *Buffer*

*Defined in [src/common/keychain.ts:12](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L12)*

## Methods

### `Abstract` sign

▸ **sign**(`msg`: Buffer): *Buffer*

*Defined in [src/common/keychain.ts:22](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L22)*

Takes a message, signs it, and returns the signature.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | The message to sign  |

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer) containing the signature
