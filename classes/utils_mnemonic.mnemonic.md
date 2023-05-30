[@c4tplatform/caminojs](../api.md) › [Utils-Mnemonic](../modules/utils_mnemonic.md) › [Mnemonic](utils_mnemonic.mnemonic.md)

# Class: Mnemonic

BIP39 Mnemonic code for generating deterministic keys.

## Hierarchy

* **Mnemonic**

## Index

### Constructors

* [constructor](utils_mnemonic.mnemonic.md#private-constructor)

### Properties

* [wordlists](utils_mnemonic.mnemonic.md#protected-wordlists)
* [instance](utils_mnemonic.mnemonic.md#static-private-instance)

### Methods

* [entropyToMnemonic](utils_mnemonic.mnemonic.md#entropytomnemonic)
* [generateMnemonic](utils_mnemonic.mnemonic.md#generatemnemonic)
* [getDefaultWordlist](utils_mnemonic.mnemonic.md#getdefaultwordlist)
* [getWordlists](utils_mnemonic.mnemonic.md#getwordlists)
* [mnemonicToEntropy](utils_mnemonic.mnemonic.md#mnemonictoentropy)
* [mnemonicToSeed](utils_mnemonic.mnemonic.md#mnemonictoseed)
* [mnemonicToSeedSync](utils_mnemonic.mnemonic.md#mnemonictoseedsync)
* [setDefaultWordlist](utils_mnemonic.mnemonic.md#setdefaultwordlist)
* [validateMnemonic](utils_mnemonic.mnemonic.md#validatemnemonic)
* [getInstance](utils_mnemonic.mnemonic.md#static-getinstance)

## Constructors

### `Private` constructor

\+ **new Mnemonic**(): *[Mnemonic](utils_mnemonic.mnemonic.md)*

*Defined in [src/utils/mnemonic.ts:26](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L26)*

**Returns:** *[Mnemonic](utils_mnemonic.mnemonic.md)*

## Properties

### `Protected` wordlists

• **wordlists**: *object* = bip39_wordlists

*Defined in [src/utils/mnemonic.ts:28](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L28)*

#### Type declaration:

* \[ **index**: *string*\]: string[]

___

### `Static` `Private` instance

▪ **instance**: *[Mnemonic](utils_mnemonic.mnemonic.md)*

*Defined in [src/utils/mnemonic.ts:26](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L26)*

## Methods

###  entropyToMnemonic

▸ **entropyToMnemonic**(`entropy`: Buffer | string, `wordlist?`: string[]): *string*

*Defined in [src/utils/mnemonic.ts:104](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L104)*

Takes mnemonic and wordlist and returns buffer

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`entropy` | Buffer &#124; string | the entropy as a [Buffer](https://github.com/feross/buffer) or as a string |
`wordlist?` | string[] | Optional, the wordlist as an array of strings  |

**Returns:** *string*

A string

___

###  generateMnemonic

▸ **generateMnemonic**(`strength?`: number, `rng?`: function, `wordlist?`: string[]): *string*

*Defined in [src/utils/mnemonic.ts:149](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L149)*

Generate a random mnemonic (uses crypto.randomBytes under the hood), defaults to 256-bits of entropy

**Parameters:**

▪`Optional`  **strength**: *number*

Optional the strength as a number

▪`Optional`  **rng**: *function*

Optional the random number generator. Defaults to crypto.randomBytes

▸ (`size`: number): *Buffer*

**Parameters:**

Name | Type |
------ | ------ |
`size` | number |

▪`Optional`  **wordlist**: *string[]*

Optional

**Returns:** *string*

___

###  getDefaultWordlist

▸ **getDefaultWordlist**(): *string*

*Defined in [src/utils/mnemonic.ts:137](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L137)*

Returns the language of the default word list

**Returns:** *string*

A string

___

###  getWordlists

▸ **getWordlists**(`language?`: string): *string[]*

*Defined in [src/utils/mnemonic.ts:47](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L47)*

Return wordlists

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`language?` | string | a string specifying the language  |

**Returns:** *string[]*

A [[Wordlist]] object or array of strings

___

###  mnemonicToEntropy

▸ **mnemonicToEntropy**(`mnemonic`: string, `wordlist?`: string[]): *string*

*Defined in [src/utils/mnemonic.ts:92](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L92)*

Takes mnemonic and wordlist and returns buffer

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`mnemonic` | string | the mnemonic as a string |
`wordlist?` | string[] | Optional the wordlist as an array of strings  |

**Returns:** *string*

A string

___

###  mnemonicToSeed

▸ **mnemonicToSeed**(`mnemonic`: string, `password`: string): *Promise‹Buffer›*

*Defined in [src/utils/mnemonic.ts:76](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L76)*

Asynchronously takes mnemonic and password and returns Promise [Buffer](https://github.com/feross/buffer)

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`mnemonic` | string | - | the mnemonic as a string |
`password` | string | "" | the password as a string  |

**Returns:** *Promise‹Buffer›*

A [Buffer](https://github.com/feross/buffer)

___

###  mnemonicToSeedSync

▸ **mnemonicToSeedSync**(`mnemonic`: string, `password`: string): *Buffer*

*Defined in [src/utils/mnemonic.ts:63](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L63)*

Synchronously takes mnemonic and password and returns [Buffer](https://github.com/feross/buffer)

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`mnemonic` | string | - | the mnemonic as a string |
`password` | string | "" | the password as a string  |

**Returns:** *Buffer*

A [Buffer](https://github.com/feross/buffer)

___

###  setDefaultWordlist

▸ **setDefaultWordlist**(`language`: string): *void*

*Defined in [src/utils/mnemonic.ts:128](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L128)*

Sets the default word list

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`language` | string | the language as a string   |

**Returns:** *void*

___

###  validateMnemonic

▸ **validateMnemonic**(`mnemonic`: string, `wordlist?`: string[]): *boolean*

*Defined in [src/utils/mnemonic.ts:118](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L118)*

Validates a mnemonic
11*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`mnemonic` | string | the mnemonic as a string |
`wordlist?` | string[] | Optional the wordlist as an array of strings  |

**Returns:** *boolean*

A string

___

### `Static` getInstance

▸ **getInstance**(): *[Mnemonic](utils_mnemonic.mnemonic.md)*

*Defined in [src/utils/mnemonic.ts:33](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/mnemonic.ts#L33)*

Retrieves the Mnemonic singleton.

**Returns:** *[Mnemonic](utils_mnemonic.mnemonic.md)*
