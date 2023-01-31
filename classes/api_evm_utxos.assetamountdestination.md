[@c4tplatform/caminojs](../README.md) › [API-EVM-UTXOs](../modules/api_evm_utxos.md) › [AssetAmountDestination](api_evm_utxos.assetamountdestination.md)

# Class: AssetAmountDestination

## Hierarchy

* [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md)‹[TransferableOutput](api_evm_outputs.transferableoutput.md), [TransferableInput](api_evm_inputs.transferableinput.md)›

  ↳ **AssetAmountDestination**

## Index

### Constructors

* [constructor](api_evm_utxos.assetamountdestination.md#constructor)

### Properties

* [amountkey](api_evm_utxos.assetamountdestination.md#protected-amountkey)
* [amounts](api_evm_utxos.assetamountdestination.md#protected-amounts)
* [change](api_evm_utxos.assetamountdestination.md#protected-change)
* [changeAddresses](api_evm_utxos.assetamountdestination.md#protected-changeaddresses)
* [changeAddressesThreshold](api_evm_utxos.assetamountdestination.md#protected-changeaddressesthreshold)
* [destinations](api_evm_utxos.assetamountdestination.md#protected-destinations)
* [destinationsThreshold](api_evm_utxos.assetamountdestination.md#protected-destinationsthreshold)
* [inputs](api_evm_utxos.assetamountdestination.md#protected-inputs)
* [outputs](api_evm_utxos.assetamountdestination.md#protected-outputs)
* [senders](api_evm_utxos.assetamountdestination.md#protected-senders)

### Methods

* [addAssetAmount](api_evm_utxos.assetamountdestination.md#addassetamount)
* [addChange](api_evm_utxos.assetamountdestination.md#addchange)
* [addInput](api_evm_utxos.assetamountdestination.md#addinput)
* [addOutput](api_evm_utxos.assetamountdestination.md#addoutput)
* [assetExists](api_evm_utxos.assetamountdestination.md#assetexists)
* [canComplete](api_evm_utxos.assetamountdestination.md#cancomplete)
* [getAllOutputs](api_evm_utxos.assetamountdestination.md#getalloutputs)
* [getAmounts](api_evm_utxos.assetamountdestination.md#getamounts)
* [getAssetAmount](api_evm_utxos.assetamountdestination.md#getassetamount)
* [getChangeAddresses](api_evm_utxos.assetamountdestination.md#getchangeaddresses)
* [getChangeAddressesThreshold](api_evm_utxos.assetamountdestination.md#getchangeaddressesthreshold)
* [getChangeOutputs](api_evm_utxos.assetamountdestination.md#getchangeoutputs)
* [getDestinations](api_evm_utxos.assetamountdestination.md#getdestinations)
* [getDestinationsThreshold](api_evm_utxos.assetamountdestination.md#getdestinationsthreshold)
* [getInputs](api_evm_utxos.assetamountdestination.md#getinputs)
* [getOutputs](api_evm_utxos.assetamountdestination.md#getoutputs)
* [getSenders](api_evm_utxos.assetamountdestination.md#getsenders)

## Constructors

###  constructor

\+ **new AssetAmountDestination**(`destinations`: Buffer[], `destinationsThreshold`: number, `senders`: Buffer[], `changeAddresses`: Buffer[], `changeAddressesThreshold`: number): *[AssetAmountDestination](api_evm_utxos.assetamountdestination.md)*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[constructor](common_assetamount.standardassetamountdestination.md#constructor)*

*Defined in [src/common/assetamount.ts:200](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L200)*

**Parameters:**

Name | Type |
------ | ------ |
`destinations` | Buffer[] |
`destinationsThreshold` | number |
`senders` | Buffer[] |
`changeAddresses` | Buffer[] |
`changeAddressesThreshold` | number |

**Returns:** *[AssetAmountDestination](api_evm_utxos.assetamountdestination.md)*

## Properties

### `Protected` amountkey

• **amountkey**: *object*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[amountkey](common_assetamount.standardassetamountdestination.md#protected-amountkey)*

*Defined in [src/common/assetamount.ts:120](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L120)*

___

### `Protected` amounts

• **amounts**: *[AssetAmount](common_assetamount.assetamount.md)[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[amounts](common_assetamount.standardassetamountdestination.md#protected-amounts)*

*Defined in [src/common/assetamount.ts:114](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L114)*

___

### `Protected` change

• **change**: *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[change](common_assetamount.standardassetamountdestination.md#protected-change)*

*Defined in [src/common/assetamount.ts:123](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L123)*

___

### `Protected` changeAddresses

• **changeAddresses**: *Buffer[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[changeAddresses](common_assetamount.standardassetamountdestination.md#protected-changeaddresses)*

*Defined in [src/common/assetamount.ts:118](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L118)*

___

### `Protected` changeAddressesThreshold

• **changeAddressesThreshold**: *number* = 0

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[changeAddressesThreshold](common_assetamount.standardassetamountdestination.md#protected-changeaddressesthreshold)*

*Defined in [src/common/assetamount.ts:119](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L119)*

___

### `Protected` destinations

• **destinations**: *Buffer[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[destinations](common_assetamount.standardassetamountdestination.md#protected-destinations)*

*Defined in [src/common/assetamount.ts:115](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L115)*

___

### `Protected` destinationsThreshold

• **destinationsThreshold**: *number* = 0

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[destinationsThreshold](common_assetamount.standardassetamountdestination.md#protected-destinationsthreshold)*

*Defined in [src/common/assetamount.ts:116](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L116)*

___

### `Protected` inputs

• **inputs**: *[TransferableInput](api_evm_inputs.transferableinput.md)[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[inputs](common_assetamount.standardassetamountdestination.md#protected-inputs)*

*Defined in [src/common/assetamount.ts:121](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L121)*

___

### `Protected` outputs

• **outputs**: *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[outputs](common_assetamount.standardassetamountdestination.md#protected-outputs)*

*Defined in [src/common/assetamount.ts:122](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L122)*

___

### `Protected` senders

• **senders**: *Buffer[]* = []

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[senders](common_assetamount.standardassetamountdestination.md#protected-senders)*

*Defined in [src/common/assetamount.ts:117](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L117)*

## Methods

###  addAssetAmount

▸ **addAssetAmount**(`assetID`: Buffer, `amount`: BN, `burn`: BN): *void*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[addAssetAmount](common_assetamount.standardassetamountdestination.md#addassetamount)*

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

▸ **addChange**(`output`: [TransferableOutput](api_evm_outputs.transferableoutput.md)): *void*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[addChange](common_assetamount.standardassetamountdestination.md#addchange)*

*Defined in [src/common/assetamount.ts:141](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L141)*

**Parameters:**

Name | Type |
------ | ------ |
`output` | [TransferableOutput](api_evm_outputs.transferableoutput.md) |

**Returns:** *void*

___

###  addInput

▸ **addInput**(`input`: [TransferableInput](api_evm_inputs.transferableinput.md)): *void*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[addInput](common_assetamount.standardassetamountdestination.md#addinput)*

*Defined in [src/common/assetamount.ts:133](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L133)*

**Parameters:**

Name | Type |
------ | ------ |
`input` | [TransferableInput](api_evm_inputs.transferableinput.md) |

**Returns:** *void*

___

###  addOutput

▸ **addOutput**(`output`: [TransferableOutput](api_evm_outputs.transferableoutput.md)): *void*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[addOutput](common_assetamount.standardassetamountdestination.md#addoutput)*

*Defined in [src/common/assetamount.ts:137](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L137)*

**Parameters:**

Name | Type |
------ | ------ |
`output` | [TransferableOutput](api_evm_outputs.transferableoutput.md) |

**Returns:** *void*

___

###  assetExists

▸ **assetExists**(`assetHexStr`: string): *boolean*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[assetExists](common_assetamount.standardassetamountdestination.md#assetexists)*

*Defined in [src/common/assetamount.ts:173](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L173)*

**Parameters:**

Name | Type |
------ | ------ |
`assetHexStr` | string |

**Returns:** *boolean*

___

###  canComplete

▸ **canComplete**(): *boolean*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[canComplete](common_assetamount.standardassetamountdestination.md#cancomplete)*

*Defined in [src/common/assetamount.ts:193](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L193)*

**Returns:** *boolean*

___

###  getAllOutputs

▸ **getAllOutputs**(): *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getAllOutputs](common_assetamount.standardassetamountdestination.md#getalloutputs)*

*Defined in [src/common/assetamount.ts:189](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L189)*

**Returns:** *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]*

___

###  getAmounts

▸ **getAmounts**(): *[AssetAmount](common_assetamount.assetamount.md)[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getAmounts](common_assetamount.standardassetamountdestination.md#getamounts)*

*Defined in [src/common/assetamount.ts:145](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L145)*

**Returns:** *[AssetAmount](common_assetamount.assetamount.md)[]*

___

###  getAssetAmount

▸ **getAssetAmount**(`assetHexStr`: string): *[AssetAmount](common_assetamount.assetamount.md)*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getAssetAmount](common_assetamount.standardassetamountdestination.md#getassetamount)*

*Defined in [src/common/assetamount.ts:169](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L169)*

**Parameters:**

Name | Type |
------ | ------ |
`assetHexStr` | string |

**Returns:** *[AssetAmount](common_assetamount.assetamount.md)*

___

###  getChangeAddresses

▸ **getChangeAddresses**(): *Buffer[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getChangeAddresses](common_assetamount.standardassetamountdestination.md#getchangeaddresses)*

*Defined in [src/common/assetamount.ts:161](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L161)*

**Returns:** *Buffer[]*

___

###  getChangeAddressesThreshold

▸ **getChangeAddressesThreshold**(): *number*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getChangeAddressesThreshold](common_assetamount.standardassetamountdestination.md#getchangeaddressesthreshold)*

*Defined in [src/common/assetamount.ts:165](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L165)*

**Returns:** *number*

___

###  getChangeOutputs

▸ **getChangeOutputs**(): *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getChangeOutputs](common_assetamount.standardassetamountdestination.md#getchangeoutputs)*

*Defined in [src/common/assetamount.ts:185](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L185)*

**Returns:** *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]*

___

###  getDestinations

▸ **getDestinations**(): *Buffer[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getDestinations](common_assetamount.standardassetamountdestination.md#getdestinations)*

*Defined in [src/common/assetamount.ts:149](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L149)*

**Returns:** *Buffer[]*

___

###  getDestinationsThreshold

▸ **getDestinationsThreshold**(): *number*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getDestinationsThreshold](common_assetamount.standardassetamountdestination.md#getdestinationsthreshold)*

*Defined in [src/common/assetamount.ts:153](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L153)*

**Returns:** *number*

___

###  getInputs

▸ **getInputs**(): *[TransferableInput](api_evm_inputs.transferableinput.md)[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getInputs](common_assetamount.standardassetamountdestination.md#getinputs)*

*Defined in [src/common/assetamount.ts:177](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L177)*

**Returns:** *[TransferableInput](api_evm_inputs.transferableinput.md)[]*

___

###  getOutputs

▸ **getOutputs**(): *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getOutputs](common_assetamount.standardassetamountdestination.md#getoutputs)*

*Defined in [src/common/assetamount.ts:181](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L181)*

**Returns:** *[TransferableOutput](api_evm_outputs.transferableoutput.md)[]*

___

###  getSenders

▸ **getSenders**(): *Buffer[]*

*Inherited from [StandardAssetAmountDestination](common_assetamount.standardassetamountdestination.md).[getSenders](common_assetamount.standardassetamountdestination.md#getsenders)*

*Defined in [src/common/assetamount.ts:157](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/assetamount.ts#L157)*

**Returns:** *Buffer[]*
