[@c4tplatform/caminojs](../README.md) › [Common-AssetAmount](../modules/common_assetamount.md) › [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md)

# Class: StandardAssetAmountDestination ‹**TO, TI**›

## Type parameters

▪ **TO**: *[StandardTransferableOutput](common_output.standardtransferableoutput.md)*

▪ **TI**: *[StandardTransferableInput](common_inputs.standardtransferableinput.md)*

## Hierarchy

* **StandardAssetAmountDestination**

  ↳ [AssetAmountDestination](api_evm_utxos.assetamountdestination.md)

  ↳ [AssetAmountDestination](api_avm_utxos.assetamountdestination.md)

  ↳ [AssetAmountDestination](api_platformvm_utxos.assetamountdestination.md)

## Index

### Constructors

* [constructor](common_assetamount.standardassetamountdestination.md#constructor)

### Properties

* [amountkey](common_assetamount.standardassetamountdestination.md#protected-amountkey)
* [amounts](common_assetamount.standardassetamountdestination.md#protected-amounts)
* [change](common_assetamount.standardassetamountdestination.md#protected-change)
* [changeAddresses](common_assetamount.standardassetamountdestination.md#protected-changeaddresses)
* [changeAddressesThreshold](common_assetamount.standardassetamountdestination.md#protected-changeaddressesthreshold)
* [destinations](common_assetamount.standardassetamountdestination.md#protected-destinations)
* [destinationsThreshold](common_assetamount.standardassetamountdestination.md#protected-destinationsthreshold)
* [inputs](common_assetamount.standardassetamountdestination.md#protected-inputs)
* [outputs](common_assetamount.standardassetamountdestination.md#protected-outputs)
* [senders](common_assetamount.standardassetamountdestination.md#protected-senders)

### Methods

* [addAssetAmount](common_assetamount.standardassetamountdestination.md#addassetamount)
* [addChange](common_assetamount.standardassetamountdestination.md#addchange)
* [addInput](common_assetamount.standardassetamountdestination.md#addinput)
* [addOutput](common_assetamount.standardassetamountdestination.md#addoutput)
* [assetExists](common_assetamount.standardassetamountdestination.md#assetexists)
* [canComplete](common_assetamount.standardassetamountdestination.md#cancomplete)
* [getAllOutputs](common_assetamount.standardassetamountdestination.md#getalloutputs)
* [getAmounts](common_assetamount.standardassetamountdestination.md#getamounts)
* [getAssetAmount](common_assetamount.standardassetamountdestination.md#getassetamount)
* [getChangeAddresses](common_assetamount.standardassetamountdestination.md#getchangeaddresses)
* [getChangeAddressesThreshold](common_assetamount.standardassetamountdestination.md#getchangeaddressesthreshold)
* [getChangeOutputs](common_assetamount.standardassetamountdestination.md#getchangeoutputs)
* [getDestinations](common_assetamount.standardassetamountdestination.md#getdestinations)
* [getDestinationsThreshold](common_assetamount.standardassetamountdestination.md#getdestinationsthreshold)
* [getInputs](common_assetamount.standardassetamountdestination.md#getinputs)
* [getOutputs](common_assetamount.standardassetamountdestination.md#getoutputs)
* [getSenders](common_assetamount.standardassetamountdestination.md#getsenders)

## Constructors

###  constructor

\+ **new StandardAssetAmountDestination**(`destinations`: Buffer[], `destinationsThreshold`: number, `senders`: Buffer[], `changeAddresses`: Buffer[], `changeAddressesThreshold`: number): *[StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md)*

*Defined in [src/common/assetamount.ts:200](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L200)*

**Parameters:**

Name | Type |
------ | ------ |
`destinations` | Buffer[] |
`destinationsThreshold` | number |
`senders` | Buffer[] |
`changeAddresses` | Buffer[] |
`changeAddressesThreshold` | number |

**Returns:** *[StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md)*

## Properties

### `Protected` amountkey

• **amountkey**: *object*

*Defined in [src/common/assetamount.ts:120](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L120)*

___

### `Protected` amounts

• **amounts**: *[AssetAmount](common_assetamount.assetamount.md)[]* = []

*Defined in [src/common/assetamount.ts:114](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L114)*

___

### `Protected` change

• **change**: *TO[]* = []

*Defined in [src/common/assetamount.ts:123](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L123)*

___

### `Protected` changeAddresses

• **changeAddresses**: *Buffer[]* = []

*Defined in [src/common/assetamount.ts:118](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L118)*

___

### `Protected` changeAddressesThreshold

• **changeAddressesThreshold**: *number* = 0

*Defined in [src/common/assetamount.ts:119](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L119)*

___

### `Protected` destinations

• **destinations**: *Buffer[]* = []

*Defined in [src/common/assetamount.ts:115](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L115)*

___

### `Protected` destinationsThreshold

• **destinationsThreshold**: *number* = 0

*Defined in [src/common/assetamount.ts:116](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L116)*

___

### `Protected` inputs

• **inputs**: *TI[]* = []

*Defined in [src/common/assetamount.ts:121](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L121)*

___

### `Protected` outputs

• **outputs**: *TO[]* = []

*Defined in [src/common/assetamount.ts:122](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L122)*

___

### `Protected` senders

• **senders**: *Buffer[]* = []

*Defined in [src/common/assetamount.ts:117](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L117)*

## Methods

###  addAssetAmount

▸ **addAssetAmount**(`assetID`: Buffer, `amount`: BN, `burn`: BN): *void*

*Defined in [src/common/assetamount.ts:127](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L127)*

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |
`amount` | BN |
`burn` | BN |

**Returns:** *void*

___

###  addChange

▸ **addChange**(`output`: TO): *void*

*Defined in [src/common/assetamount.ts:141](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L141)*

**Parameters:**

Name | Type |
------ | ------ |
`output` | TO |

**Returns:** *void*

___

###  addInput

▸ **addInput**(`input`: TI): *void*

*Defined in [src/common/assetamount.ts:133](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L133)*

**Parameters:**

Name | Type |
------ | ------ |
`input` | TI |

**Returns:** *void*

___

###  addOutput

▸ **addOutput**(`output`: TO): *void*

*Defined in [src/common/assetamount.ts:137](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L137)*

**Parameters:**

Name | Type |
------ | ------ |
`output` | TO |

**Returns:** *void*

___

###  assetExists

▸ **assetExists**(`assetHexStr`: string): *boolean*

*Defined in [src/common/assetamount.ts:173](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L173)*

**Parameters:**

Name | Type |
------ | ------ |
`assetHexStr` | string |

**Returns:** *boolean*

___

###  canComplete

▸ **canComplete**(): *boolean*

*Defined in [src/common/assetamount.ts:193](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L193)*

**Returns:** *boolean*

___

###  getAllOutputs

▸ **getAllOutputs**(): *TO[]*

*Defined in [src/common/assetamount.ts:189](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L189)*

**Returns:** *TO[]*

___

###  getAmounts

▸ **getAmounts**(): *[AssetAmount](common_assetamount.assetamount.md)[]*

*Defined in [src/common/assetamount.ts:145](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L145)*

**Returns:** *[AssetAmount](common_assetamount.assetamount.md)[]*

___

###  getAssetAmount

▸ **getAssetAmount**(`assetHexStr`: string): *[AssetAmount](common_assetamount.assetamount.md)*

*Defined in [src/common/assetamount.ts:169](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L169)*

**Parameters:**

Name | Type |
------ | ------ |
`assetHexStr` | string |

**Returns:** *[AssetAmount](common_assetamount.assetamount.md)*

___

###  getChangeAddresses

▸ **getChangeAddresses**(): *Buffer[]*

*Defined in [src/common/assetamount.ts:161](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L161)*

**Returns:** *Buffer[]*

___

###  getChangeAddressesThreshold

▸ **getChangeAddressesThreshold**(): *number*

*Defined in [src/common/assetamount.ts:165](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L165)*

**Returns:** *number*

___

###  getChangeOutputs

▸ **getChangeOutputs**(): *TO[]*

*Defined in [src/common/assetamount.ts:185](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L185)*

**Returns:** *TO[]*

___

###  getDestinations

▸ **getDestinations**(): *Buffer[]*

*Defined in [src/common/assetamount.ts:149](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L149)*

**Returns:** *Buffer[]*

___

###  getDestinationsThreshold

▸ **getDestinationsThreshold**(): *number*

*Defined in [src/common/assetamount.ts:153](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L153)*

**Returns:** *number*

___

###  getInputs

▸ **getInputs**(): *TI[]*

*Defined in [src/common/assetamount.ts:177](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L177)*

**Returns:** *TI[]*

___

###  getOutputs

▸ **getOutputs**(): *TO[]*

*Defined in [src/common/assetamount.ts:181](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L181)*

**Returns:** *TO[]*

___

###  getSenders

▸ **getSenders**(): *Buffer[]*

*Defined in [src/common/assetamount.ts:157](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L157)*

**Returns:** *Buffer[]*
