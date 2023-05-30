[@c4tplatform/caminojs](../api.md) › [Common-KeyChain](../modules/common_keychain.md) › [SignerKeyChain](common_keychain.signerkeychain.md)

# Class: SignerKeyChain

## Hierarchy

* **SignerKeyChain**

## Index

### Methods

* [getKey](common_keychain.signerkeychain.md#abstract-getkey)

## Methods

### `Abstract` getKey

▸ **getKey**(`address`: Buffer): *[SignerKeyPair](common_keychain.signerkeypair.md)*

*Defined in [src/common/keychain.ts:132](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L132)*

Returns the [SignerKeyPair](common_keychain.signerkeypair.md) listed under the provided address

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | Buffer | The [Buffer](https://github.com/feross/buffer) of the address to retrieve from the keys database  |

**Returns:** *[SignerKeyPair](common_keychain.signerkeypair.md)*

A reference to the [SignerKeyPair](common_keychain.signerkeypair.md) in the keys database
