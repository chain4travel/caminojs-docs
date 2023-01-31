[@c4tplatform/caminojs](../README.md) › [API-PlatformVM-Builder](../modules/api_platformvm_builder.md) › [Builder](api_platformvm_builder.builder.md)

# Class: Builder

## Hierarchy

* **Builder**

## Index

### Constructors

* [constructor](api_platformvm_builder.builder.md#constructor)

### Properties

* [caminoEnabled](api_platformvm_builder.builder.md#caminoenabled)
* [spender](api_platformvm_builder.builder.md#spender)

### Methods

* [_feeCheck](api_platformvm_builder.builder.md#_feecheck)
* [buildAddDelegatorTx](api_platformvm_builder.builder.md#buildadddelegatortx)
* [buildAddSubnetValidatorTx](api_platformvm_builder.builder.md#buildaddsubnetvalidatortx)
* [buildAddValidatorTx](api_platformvm_builder.builder.md#buildaddvalidatortx)
* [buildAddressStateTx](api_platformvm_builder.builder.md#buildaddressstatetx)
* [buildBaseTx](api_platformvm_builder.builder.md#buildbasetx)
* [buildCaminoAddValidatorTx](api_platformvm_builder.builder.md#buildcaminoaddvalidatortx)
* [buildCreateChainTx](api_platformvm_builder.builder.md#buildcreatechaintx)
* [buildCreateSubnetTx](api_platformvm_builder.builder.md#buildcreatesubnettx)
* [buildDepositTx](api_platformvm_builder.builder.md#builddeposittx)
* [buildExportTx](api_platformvm_builder.builder.md#buildexporttx)
* [buildImportTx](api_platformvm_builder.builder.md#buildimporttx)
* [buildRegisterNodeTx](api_platformvm_builder.builder.md#buildregisternodetx)

## Constructors

###  constructor

\+ **new Builder**(`spender`: [MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md), `caminoEnabled`: boolean): *[Builder](api_platformvm_builder.builder.md)*

*Defined in [src/apis/platformvm/builder.ts:60](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L60)*

**Parameters:**

Name | Type |
------ | ------ |
`spender` | [MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md) |
`caminoEnabled` | boolean |

**Returns:** *[Builder](api_platformvm_builder.builder.md)*

## Properties

###  caminoEnabled

• **caminoEnabled**: *boolean*

*Defined in [src/apis/platformvm/builder.ts:60](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L60)*

___

###  spender

• **spender**: *[MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md)*

*Defined in [src/apis/platformvm/builder.ts:59](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L59)*

## Methods

###  _feeCheck

▸ **_feeCheck**(`fee`: BN, `feeAssetID`: Buffer): *boolean*

*Defined in [src/apis/platformvm/builder.ts:1277](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L1277)*

**Parameters:**

Name | Type |
------ | ------ |
`fee` | BN |
`feeAssetID` | Buffer |

**Returns:** *boolean*

___

###  buildAddDelegatorTx

▸ **buildAddDelegatorTx**(`networkID`: number, `blockchainID`: Buffer, `avaxAssetID`: Buffer, `toAddresses`: Buffer[], `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `rewardLocktime`: BN, `rewardThreshold`: number, `rewardAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:538](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L538)*

Class representing an unsigned [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`avaxAssetID` | Buffer | - | [Buffer](https://github.com/feross/buffer) of the asset ID for AVAX |
`toAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) recieves the stake at the end of the staking period |
`fromAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who pays the fees and the stake |
`changeAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who gets the change leftover from the staking payment |
`nodeID` | Buffer | - | The node ID of the validator being added. |
`startTime` | BN | - | The Unix time when the validator starts validating the Primary Network. |
`endTime` | BN | - | The Unix time when the validator stops validating the Primary Network (and staked AVAX is returned). |
`stakeAmount` | BN | - | A [BN](https://github.com/indutny/bn.js/) for the amount of stake to be delegated in nAVAX. |
`rewardLocktime` | BN | - | The locktime field created in the resulting reward outputs |
`rewardThreshold` | number | - | The number of signatures required to spend the funds in the resultant reward UTXO |
`rewardAddresses` | Buffer[] | - | The addresses the validator reward goes. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned. |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`toThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the stake UTXO |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildAddSubnetValidatorTx

▸ **buildAddSubnetValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `weight`: BN, `subnetID`: string, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `subnetAuthCredentials`: [][], `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:439](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L439)*

Class representing an unsigned [AddSubnetValidatorTx](../modules/src_apis_platformvm.md#addsubnetvalidatortx) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who pays the fees in AVAX |
`changeAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who gets the change leftover from the fee payment |
`nodeID` | Buffer | - | The node ID of the validator being added. |
`startTime` | BN | - | The Unix time when the validator starts validating the Primary Network. |
`endTime` | BN | - | The Unix time when the validator stops validating the Primary Network (and staked AVAX is returned). |
`weight` | BN | - | The amount of weight for this subnet validator. |
`subnetID` | string | - | - |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned. |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`subnetAuthCredentials` | [][] | [] | Optional. An array of index and address to sign for each SubnetAuth. |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildAddValidatorTx

▸ **buildAddValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `toAddresses`: Buffer[], `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `stakeAssetID`: Buffer, `rewardLocktime`: BN, `rewardThreshold`: number, `rewardAddresses`: Buffer[], `delegationFee`: number, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:664](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L664)*

Class representing an unsigned [AddValidatorTx](api_platformvm_validationtx.addvalidatortx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | NetworkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | BlockchainID, default undefined |
`toAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) recieves the stake at the end of the staking period |
`fromAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who pays the fees and the stake |
`changeAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who gets the change leftover from the staking payment |
`nodeID` | Buffer | - | The node ID of the validator being added. |
`startTime` | BN | - | The Unix time when the validator starts validating the Primary Network. |
`endTime` | BN | - | The Unix time when the validator stops validating the Primary Network (and staked AVAX is returned). |
`stakeAmount` | BN | - | A [BN](https://github.com/indutny/bn.js/) for the amount of stake to be delegated in nAVAX. |
`stakeAssetID` | Buffer | - | - |
`rewardLocktime` | BN | - | The locktime field created in the resulting reward outputs |
`rewardThreshold` | number | - | The number of signatures required to spend the funds in the resultant reward UTXO |
`rewardAddresses` | Buffer[] | - | The addresses the validator reward goes. |
`delegationFee` | number | - | A number for the percentage of reward to be given to the validator when someone delegates to them. Must be between 0 and 100. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned. |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | UnixNow() | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`toThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the stake UTXO |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

___

###  buildAddressStateTx

▸ **buildAddressStateTx**(`networkID`: number, `blockchainID`: Buffer, `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `address`: Buffer, `state`: number, `remove`: boolean, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1057](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L1057)*

Build an unsigned [AddressStateTx](api_platformvm_addressstatetx.addressstatetx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`address` | Buffer | - | The address to alter state. |
`state` | number | - | The state to set or remove on the given address |
`remove` | boolean | false | Optional. Flag if state should be applied or removed |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned AddressStateTx created from the passed in parameters.

___

###  buildBaseTx

▸ **buildBaseTx**(`networkID`: number, `blockchainID`: Buffer, `amount`: BN, `amountAssetID`: Buffer, `toAddresses`: Buffer[], `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `lockTime`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:89](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L89)*

Creates an [UnsignedTx](api_evm_transactions.unsignedtx.md) wrapping a [BaseTx](api_avm_basetx.basetx.md). For more granular control, you may create your own
[UnsignedTx](api_evm_transactions.unsignedtx.md) wrapping a [BaseTx](api_avm_basetx.basetx.md) manually (with their corresponding [TransferableInput](api_evm_inputs.transferableinput.md)s and [TransferableOutput](api_evm_outputs.transferableoutput.md)s).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | - | The number representing NetworkID of the node |
`blockchainID` | Buffer | - | The [Buffer](https://github.com/feross/buffer) representing the BlockchainID for the transaction |
`amount` | BN | - | The amount of the asset to be spent in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/). |
`amountAssetID` | Buffer | - | - |
`toAddresses` | Buffer[] | - | The addresses to send the funds |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | undefined | Optional. The addresses that can spend the change remaining from the spent UTXOs. Default: toAddresses |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned. Default: assetID |
`memo` | Buffer | undefined | Optional. Contains arbitrary data, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`lockTime` | BN | zero | - |
`toThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant UTXO |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildCaminoAddValidatorTx

▸ **buildCaminoAddValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `to`: Buffer[], `from`: Buffer[], `change`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `stakeAssetID`: Buffer, `rewards`: Buffer[], `rewardLocktime`: BN, `rewardThreshold`: number, `memo`: Buffer, `asOf`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:965](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L965)*

Helper function which creates an unsigned [CaminoAddValidatorTx](api_platformvm_validationtx.caminoaddvalidatortx.md). For more granular control, you may create your own
[UnsignedTx](api_evm_transactions.unsignedtx.md) manually and import the [CaminoAddValidatorTx](api_platformvm_validationtx.caminoaddvalidatortx.md) class directly.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`to` | Buffer[] | - | - |
`from` | Buffer[] | - | - |
`change` | Buffer[] | - | - |
`nodeID` | Buffer | - | The node ID of the validator being added. |
`startTime` | BN | - | The Unix time when the validator starts validating the Primary Network. |
`endTime` | BN | - | The Unix time when the validator stops validating the Primary Network (and staked AVAX is returned). |
`stakeAmount` | BN | - | The amount being delegated as a [BN](https://github.com/indutny/bn.js/) |
`stakeAssetID` | Buffer | - | - |
`rewards` | Buffer[] | - | - |
`rewardLocktime` | BN | zero | Optional. The locktime field created in the resulting reward outputs |
`rewardThreshold` | number | 1 | Opional. The number of signatures required to spend the funds in the resultant reward UTXO. Default 1. |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`toThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the received UTXO |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildCreateChainTx

▸ **buildCreateChainTx**(`networkID`: number, `blockchainID`: Buffer, `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `subnetID`: string | Buffer, `chainName`: string, `vmID`: string, `fxIDs`: string[], `genesisData`: string | [GenesisData](api_avm_genesisdata.genesisdata.md), `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `subnetAuthCredentials`: [][], `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:874](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L874)*

Build an unsigned [CreateChainTx](api_platformvm_createchaintx.createchaintx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`subnetID` | string &#124; Buffer | undefined | Optional ID of the Subnet that validates this blockchain |
`chainName` | string | undefined | Optional A human readable name for the chain; need not be unique |
`vmID` | string | undefined | Optional ID of the VM running on the new chain |
`fxIDs` | string[] | undefined | Optional IDs of the feature extensions running on the new chain |
`genesisData` | string &#124; [GenesisData](api_avm_genesisdata.genesisdata.md) | undefined | Optional Byte representation of genesis state of the new chain |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`subnetAuthCredentials` | [][] | [] | Optional. An array of index and address to sign for each SubnetAuth. |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned CreateChainTx created from the passed in parameters.

___

###  buildCreateSubnetTx

▸ **buildCreateSubnetTx**(`networkID`: number, `blockchainID`: Buffer, `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `subnetOwnerAddresses`: Buffer[], `subnetOwnerThreshold`: number, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:795](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L795)*

Class representing an unsigned [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`subnetOwnerAddresses` | Buffer[] | - | An array of [Buffer](https://github.com/feross/buffer) for the addresses to add to a subnet |
`subnetOwnerThreshold` | number | - | The number of owners's signatures required to add a validator to the network |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildDepositTx

▸ **buildDepositTx**(`networkID`: number, `blockchainID`: Buffer, `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `depositOfferID`: string | Buffer, `depositDuration`: number | Buffer, `rewardsOwner`: [OutputOwners](common_output.outputowners.md), `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1215](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L1215)*

Build an unsigned [DepositTx](api_platformvm_deposittx.deposittx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`depositOfferID` | string &#124; Buffer | - | ID of the deposit offer. |
`depositDuration` | number &#124; Buffer | - | Duration of the deposit |
`rewardsOwner` | [OutputOwners](common_output.outputowners.md) | - | Optional The owners of the reward. If omitted, all inputs must have the same owner |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned DepositTx created from the passed in parameters.

___

###  buildExportTx

▸ **buildExportTx**(`networkID`: number, `blockchainID`: Buffer, `amount`: BN, `amountAssetID`: Buffer, `toAddresses`: Buffer[], `fromAddresses`: Buffer[], `destinationChain`: Buffer, `changeAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `locktime`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:328](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L328)*

Creates an unsigned ExportTx transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | - | The number representing NetworkID of the node |
`blockchainID` | Buffer | - | The [Buffer](https://github.com/feross/buffer) representing the BlockchainID for the transaction |
`amount` | BN | - | The amount being exported as a [BN](https://github.com/indutny/bn.js/) |
`amountAssetID` | Buffer | - | - |
`toAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who recieves the AVAX |
`fromAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who owns the AVAX |
`destinationChain` | Buffer | - | Optional. A [Buffer](https://github.com/feross/buffer) for the chainid where to send the asset. |
`changeAddresses` | Buffer[] | undefined | An array of addresses as [Buffer](https://github.com/feross/buffer) who gets the change leftover of the AVAX |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned. |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`locktime` | BN | zero | Optional. The locktime field created in the resulting outputs |
`toThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the received UTXO |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildImportTx

▸ **buildImportTx**(`networkID`: number, `blockchainID`: Buffer, `toAddresses`: Buffer[], `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `atomics`: [UTXO](api_platformvm_utxos.utxo.md)[], `sourceChain`: Buffer, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `locktime`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:180](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L180)*

Creates an unsigned ImportTx transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | - | The number representing NetworkID of the node |
`blockchainID` | Buffer | - | The [Buffer](https://github.com/feross/buffer) representing the BlockchainID for the transaction |
`toAddresses` | Buffer[] | - | The addresses to send the funds |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | Optional. The addresses that can spend the change remaining from the spent UTXOs. Default: toAddresses |
`atomics` | [UTXO](api_platformvm_utxos.utxo.md)[] | - | - |
`sourceChain` | Buffer | undefined | A [Buffer](https://github.com/feross/buffer) for the chainid where the imports are coming from. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/). Fee will come from the inputs first, if they can. |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned. |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | - |
`locktime` | BN | zero | Optional. The locktime field created in the resulting outputs |
`toThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the received UTXO |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildRegisterNodeTx

▸ **buildRegisterNodeTx**(`networkID`: number, `blockchainID`: Buffer, `fromAddresses`: Buffer[], `changeAddresses`: Buffer[], `oldNodeID`: string | Buffer, `newNodeID`: string | Buffer, `address`: Buffer, `consortiumMemberAuthCredentials`: [][], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1132](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/platformvm/builder.ts#L1132)*

Build an unsigned [RegisterNodeTx](api_platformvm_registernodetx.registernodetx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromAddresses` | Buffer[] | - | The addresses being used to send the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`oldNodeID` | string &#124; Buffer | undefined | Optional. ID of the existing NodeID to replace or remove. |
`newNodeID` | string &#124; Buffer | undefined | Optional. ID of the newNodID to register address. |
`address` | Buffer | undefined | The consortiumMemberAddress, single or multi-sig. |
`consortiumMemberAuthCredentials` | [][] | [] | An array of index and address to sign for each SubnetAuth. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned RegisterNodeTx created from the passed in parameters.
