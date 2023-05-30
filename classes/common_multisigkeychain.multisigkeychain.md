[@c4tplatform/caminojs](../api.md) › [Common-MultisigKeyChain](../modules/common_multisigkeychain.md) › [MultisigKeyChain](common_multisigkeychain.multisigkeychain.md)

# Class: MultisigKeyChain

Class for representing a multisig keyChain in Camino.

**`typeparam`** Class extending [StandardKeyChain](common_keychain.standardkeychain.md)

## Hierarchy

* [StandardKeyChain](common_keychain.standardkeychain.md)‹[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)›

  ↳ **MultisigKeyChain**

## Index

### Constructors

* [constructor](common_multisigkeychain.multisigkeychain.md#constructor)

### Properties

* [chainID](common_multisigkeychain.multisigkeychain.md#protected-chainid)
* [credTypeID](common_multisigkeychain.multisigkeychain.md#protected-credtypeid)
* [hrp](common_multisigkeychain.multisigkeychain.md#protected-hrp)
* [importKey](common_multisigkeychain.multisigkeychain.md#importkey)
* [keys](common_multisigkeychain.multisigkeychain.md#protected-keys)
* [makeKey](common_multisigkeychain.multisigkeychain.md#makekey)
* [msigAliases](common_multisigkeychain.multisigkeychain.md#protected-msigaliases)
* [sigIdxs](common_multisigkeychain.multisigkeychain.md#protected-sigidxs)
* [signedBytes](common_multisigkeychain.multisigkeychain.md#protected-signedbytes)
* [txOwners](common_multisigkeychain.multisigkeychain.md#protected-txowners)

### Methods

* [_traverseOwner](common_multisigkeychain.multisigkeychain.md#protected-_traverseowner)
* [addKey](common_multisigkeychain.multisigkeychain.md#addkey)
* [buildSignatureIndices](common_multisigkeychain.multisigkeychain.md#buildsignatureindices)
* [clone](common_multisigkeychain.multisigkeychain.md#clone)
* [create](common_multisigkeychain.multisigkeychain.md#create)
* [getAddressStrings](common_multisigkeychain.multisigkeychain.md#getaddressstrings)
* [getAddresses](common_multisigkeychain.multisigkeychain.md#getaddresses)
* [getChainID](common_multisigkeychain.multisigkeychain.md#getchainid)
* [getCredentials](common_multisigkeychain.multisigkeychain.md#getcredentials)
* [getHRP](common_multisigkeychain.multisigkeychain.md#gethrp)
* [getKey](common_multisigkeychain.multisigkeychain.md#getkey)
* [getKeys](common_multisigkeychain.multisigkeychain.md#getkeys)
* [hasKey](common_multisigkeychain.multisigkeychain.md#haskey)
* [removeKey](common_multisigkeychain.multisigkeychain.md#removekey)
* [union](common_multisigkeychain.multisigkeychain.md#union)

## Constructors

###  constructor

\+ **new MultisigKeyChain**(`hrp`: string, `chainID`: string, `signedBytes`: Buffer, `credTypeID`: number, `txOwners?`: [OutputOwners](common_output.outputowners.md)[], `msigAliases?`: Map‹string, [OutputOwners](common_output.outputowners.md)›): *[MultisigKeyChain](common_multisigkeychain.multisigkeychain.md)*

*Defined in [src/common/multisigkeychain.ts:289](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L289)*

**Parameters:**

Name | Type |
------ | ------ |
`hrp` | string |
`chainID` | string |
`signedBytes` | Buffer |
`credTypeID` | number |
`txOwners?` | [OutputOwners](common_output.outputowners.md)[] |
`msigAliases?` | Map‹string, [OutputOwners](common_output.outputowners.md)› |

**Returns:** *[MultisigKeyChain](common_multisigkeychain.multisigkeychain.md)*

## Properties

### `Protected` chainID

• **chainID**: *string*

*Defined in [src/common/multisigkeychain.ts:106](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L106)*

___

### `Protected` credTypeID

• **credTypeID**: *number*

*Defined in [src/common/multisigkeychain.ts:116](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L116)*

___

### `Protected` hrp

• **hrp**: *string*

*Defined in [src/common/multisigkeychain.ts:104](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L104)*

___

###  importKey

• **importKey**: *function*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[importKey](common_keychain.standardkeychain.md#importkey)*

*Defined in [src/common/keychain.ts:158](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L158)*

Given a private key, makes a new [StandardKeyPair](common_keychain.standardkeypair.md), returns the address.

**`param`** A [Buffer](https://github.com/feross/buffer) representing the private key

**`returns`** A new [StandardKeyPair](common_keychain.standardkeypair.md)

#### Type declaration:

▸ (`privk`: Buffer): *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)*

**Parameters:**

Name | Type |
------ | ------ |
`privk` | Buffer |

___

### `Protected` keys

• **keys**: *object*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[keys](common_keychain.standardkeychain.md#protected-keys)*

*Defined in [src/common/keychain.ts:142](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L142)*

#### Type declaration:

* \[ **address**: *string*\]: [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)

___

###  makeKey

• **makeKey**: *function*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[makeKey](common_keychain.standardkeychain.md#makekey)*

*Defined in [src/common/keychain.ts:149](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L149)*

Makes a new [StandardKeyPair](common_keychain.standardkeypair.md), returns the address.

**`returns`** Address of the new [StandardKeyPair](common_keychain.standardkeypair.md)

#### Type declaration:

▸ (): *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)*

___

### `Protected` msigAliases

• **msigAliases**: *Map‹string, [OutputOwners](common_output.outputowners.md)›*

*Defined in [src/common/multisigkeychain.ts:112](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L112)*

___

### `Protected` sigIdxs

• **sigIdxs**: *[SigIdx](common_signature.sigidx.md)[][]*

*Defined in [src/common/multisigkeychain.ts:114](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L114)*

___

### `Protected` signedBytes

• **signedBytes**: *Buffer*

*Defined in [src/common/multisigkeychain.ts:108](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L108)*

___

### `Protected` txOwners

• **txOwners**: *[OutputOwners](common_output.outputowners.md)[]*

*Defined in [src/common/multisigkeychain.ts:110](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L110)*

## Methods

### `Protected` _traverseOwner

▸ **_traverseOwner**(`owner`: [OutputOwners](common_output.outputowners.md)): *void*

*Defined in [src/common/multisigkeychain.ts:191](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L191)*

**Parameters:**

Name | Type |
------ | ------ |
`owner` | [OutputOwners](common_output.outputowners.md) |

**Returns:** *void*

___

###  addKey

▸ **addKey**(`newKey`: [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)): *void*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[addKey](common_keychain.standardkeychain.md#addkey)*

*Defined in [src/common/keychain.ts:182](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L182)*

Adds the key pair to the list of the keys managed in the [StandardKeyChain](common_keychain.standardkeychain.md).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`newKey` | [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md) | A key pair of the appropriate class to be added to the [StandardKeyChain](common_keychain.standardkeychain.md)  |

**Returns:** *void*

___

###  buildSignatureIndices

▸ **buildSignatureIndices**(): *void*

*Defined in [src/common/multisigkeychain.ts:171](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L171)*

**Returns:** *void*

___

###  clone

▸ **clone**(): *this*

*Overrides [StandardKeyChain](common_keychain.standardkeychain.md).[clone](common_keychain.standardkeychain.md#abstract-clone)*

*Defined in [src/common/multisigkeychain.ts:138](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L138)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [StandardKeyChain](common_keychain.standardkeychain.md).[create](common_keychain.standardkeychain.md#abstract-create)*

*Defined in [src/common/multisigkeychain.ts:126](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L126)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  getAddressStrings

▸ **getAddressStrings**(): *string[]*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[getAddressStrings](common_keychain.standardkeychain.md#getaddressstrings)*

*Defined in [src/common/keychain.ts:174](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L174)*

Gets an array of addresses stored in the [StandardKeyChain](common_keychain.standardkeychain.md).

**Returns:** *string[]*

An array of string representations of the addresses

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[getAddresses](common_keychain.standardkeychain.md#getaddresses)*

*Defined in [src/common/keychain.ts:166](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L166)*

Gets an array of addresses stored in the [StandardKeyChain](common_keychain.standardkeychain.md).

**Returns:** *Buffer[]*

An array of [Buffer](https://github.com/feross/buffer)  representations
of the addresses

___

###  getChainID

▸ **getChainID**(): *string*

*Defined in [src/common/multisigkeychain.ts:122](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L122)*

**Returns:** *string*

___

###  getCredentials

▸ **getCredentials**(): *[Credential](common_signature.credential.md)[]*

*Defined in [src/common/multisigkeychain.ts:176](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L176)*

**Returns:** *[Credential](common_signature.credential.md)[]*

___

###  getHRP

▸ **getHRP**(): *string*

*Defined in [src/common/multisigkeychain.ts:118](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L118)*

**Returns:** *string*

___

###  getKey

▸ **getKey**(`address`: Buffer): *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[getKey](common_keychain.standardkeychain.md#getkey)*

*Defined in [src/common/keychain.ts:225](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L225)*

Returns the [StandardKeyPair](common_keychain.standardkeypair.md) listed under the provided address

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | Buffer | The [Buffer](https://github.com/feross/buffer) of the address to retrieve from the keys database  |

**Returns:** *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)*

A reference to the [StandardKeyPair](common_keychain.standardkeypair.md) in the keys database

___

###  getKeys

▸ **getKeys**(`address`: Buffer): *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)[]*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[getKeys](common_keychain.standardkeychain.md#getkeys)*

*Defined in [src/common/keychain.ts:235](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L235)*

Returns the [StandardKeyPair](common_keychain.standardkeypair.md)'s listed under the provided address

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | Buffer | The [Buffer](https://github.com/feross/buffer) of the address to retrieve from the keys database  |

**Returns:** *[MultisigKeyPair](common_multisigkeychain.multisigkeypair.md)[]*

A reference to the [StandardKeyPair](common_keychain.standardkeypair.md)'s in the keys database

___

###  hasKey

▸ **hasKey**(`address`: Buffer): *boolean*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[hasKey](common_keychain.standardkeychain.md#haskey)*

*Defined in [src/common/keychain.ts:215](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L215)*

Checks if there is a key associated with the provided address.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | Buffer | The address to check for existence in the keys database  |

**Returns:** *boolean*

True on success, false if not found

___

###  removeKey

▸ **removeKey**(`key`: [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md) | Buffer): *boolean*

*Inherited from [StandardKeyChain](common_keychain.standardkeychain.md).[removeKey](common_keychain.standardkeychain.md#removekey)*

*Defined in [src/common/keychain.ts:194](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/keychain.ts#L194)*

Removes the key pair from the list of they keys managed in the [StandardKeyChain](common_keychain.standardkeychain.md).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | [MultisigKeyPair](common_multisigkeychain.multisigkeypair.md) &#124; Buffer | A [Buffer](https://github.com/feross/buffer) for the address or KPClass to remove  |

**Returns:** *boolean*

The boolean true if a key was removed.

___

###  union

▸ **union**(`kc`: this): *this*

*Overrides [StandardKeyChain](common_keychain.standardkeychain.md).[union](common_keychain.standardkeychain.md#abstract-union)*

*Defined in [src/common/multisigkeychain.ts:155](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L155)*

**Parameters:**

Name | Type |
------ | ------ |
`kc` | this |

**Returns:** *this*
