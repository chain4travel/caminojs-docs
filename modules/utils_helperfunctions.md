[@c4tplatform/caminojs](../README.md) › [Utils-HelperFunctions](utils_helperfunctions.md)

# Module: Utils-HelperFunctions

## Index

### Functions

* [MaxWeightFormula](utils_helperfunctions.md#maxweightformula)
* [NodeIDStringToBuffer](utils_helperfunctions.md#nodeidstringtobuffer)
* [UnixNow](utils_helperfunctions.md#unixnow)
* [bufferToNodeIDString](utils_helperfunctions.md#buffertonodeidstring)
* [bufferToPrivateKeyString](utils_helperfunctions.md#buffertoprivatekeystring)
* [calcBytesCost](utils_helperfunctions.md#calcbytescost)
* [costExportTx](utils_helperfunctions.md#costexporttx)
* [costImportTx](utils_helperfunctions.md#costimporttx)
* [privateKeyStringToBuffer](utils_helperfunctions.md#privatekeystringtobuffer)

## Functions

###  MaxWeightFormula

▸ **MaxWeightFormula**(`staked`: BN, `cap`: BN): *BN*

*Defined in [src/utils/helperfunctions.ts:18](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L18)*

**Parameters:**

Name | Type |
------ | ------ |
`staked` | BN |
`cap` | BN |

**Returns:** *BN*

___

###  NodeIDStringToBuffer

▸ **NodeIDStringToBuffer**(`pk`: string): *Buffer*

*Defined in [src/utils/helperfunctions.ts:67](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L67)*

Takes a nodeID string and produces a nodeID [Buffer](https://github.com/feross/buffer).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`pk` | string | A string for the nodeID.  |

**Returns:** *Buffer*

___

###  UnixNow

▸ **UnixNow**(): *BN*

*Defined in [src/utils/helperfunctions.ts:25](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L25)*

Function providing the current UNIX time using a [BN](https://github.com/indutny/bn.js/).

**Returns:** *BN*

___

###  bufferToNodeIDString

▸ **bufferToNodeIDString**(`pk`: Buffer): *string*

*Defined in [src/utils/helperfunctions.ts:58](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L58)*

Takes a nodeID buffer and produces a nodeID string with prefix.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`pk` | Buffer | A [Buffer](https://github.com/feross/buffer) for the nodeID.  |

**Returns:** *string*

___

###  bufferToPrivateKeyString

▸ **bufferToPrivateKeyString**(`pk`: Buffer): *string*

*Defined in [src/utils/helperfunctions.ts:34](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L34)*

Takes a private key buffer and produces a private key string with prefix.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`pk` | Buffer | A [Buffer](https://github.com/feross/buffer) for the private key.  |

**Returns:** *string*

___

###  calcBytesCost

▸ **calcBytesCost**(`c`: [C](../interfaces/utils_networks.c.md), `len`: number): *number*

*Defined in [src/utils/helperfunctions.ts:88](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L88)*

**Parameters:**

Name | Type |
------ | ------ |
`c` | [C](../interfaces/utils_networks.c.md) |
`len` | number |

**Returns:** *number*

___

###  costExportTx

▸ **costExportTx**(`c`: [C](../interfaces/utils_networks.c.md), `tx`: [UnsignedTx](../classes/api_evm_transactions.unsignedtx.md)): *number*

*Defined in [src/utils/helperfunctions.ts:92](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L92)*

**Parameters:**

Name | Type |
------ | ------ |
`c` | [C](../interfaces/utils_networks.c.md) |
`tx` | [UnsignedTx](../classes/api_evm_transactions.unsignedtx.md) |

**Returns:** *number*

___

###  costImportTx

▸ **costImportTx**(`c`: [C](../interfaces/utils_networks.c.md), `tx`: [UnsignedTx](../classes/api_evm_transactions.unsignedtx.md)): *number*

*Defined in [src/utils/helperfunctions.ts:77](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L77)*

**Parameters:**

Name | Type |
------ | ------ |
`c` | [C](../interfaces/utils_networks.c.md) |
`tx` | [UnsignedTx](../classes/api_evm_transactions.unsignedtx.md) |

**Returns:** *number*

___

###  privateKeyStringToBuffer

▸ **privateKeyStringToBuffer**(`pk`: string): *Buffer*

*Defined in [src/utils/helperfunctions.ts:43](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/helperfunctions.ts#L43)*

Takes a private key string and produces a private key [Buffer](https://github.com/feross/buffer).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`pk` | string | A string for the private key.  |

**Returns:** *Buffer*
