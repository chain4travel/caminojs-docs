[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Builder](../modules/api_platformvm_builder.md) › [Builder](api_platformvm_builder.builder.md)

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
* [buildClaimTx](api_platformvm_builder.builder.md#buildclaimtx)
* [buildCreateChainTx](api_platformvm_builder.builder.md#buildcreatechaintx)
* [buildCreateSubnetTx](api_platformvm_builder.builder.md#buildcreatesubnettx)
* [buildDepositTx](api_platformvm_builder.builder.md#builddeposittx)
* [buildExportTx](api_platformvm_builder.builder.md#buildexporttx)
* [buildImportTx](api_platformvm_builder.builder.md#buildimporttx)
* [buildMultisigAliasTx](api_platformvm_builder.builder.md#buildmultisigaliastx)
* [buildRegisterNodeTx](api_platformvm_builder.builder.md#buildregisternodetx)
* [buildUnlockDepositTx](api_platformvm_builder.builder.md#buildunlockdeposittx)

## Constructors

###  constructor

\+ **new Builder**(`spender`: [MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md), `caminoEnabled`: boolean): *[Builder](api_platformvm_builder.builder.md)*

*Defined in [src/apis/platformvm/builder.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L86)*

**Parameters:**

Name | Type |
------ | ------ |
`spender` | [MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md) |
`caminoEnabled` | boolean |

**Returns:** *[Builder](api_platformvm_builder.builder.md)*

## Properties

###  caminoEnabled

• **caminoEnabled**: *boolean*

*Defined in [src/apis/platformvm/builder.ts:86](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L86)*

___

###  spender

• **spender**: *[MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md)*

*Defined in [src/apis/platformvm/builder.ts:85](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L85)*

## Methods

###  _feeCheck

▸ **_feeCheck**(`fee`: BN, `feeAssetID`: Buffer): *boolean*

*Defined in [src/apis/platformvm/builder.ts:1645](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1645)*

**Parameters:**

Name | Type |
------ | ------ |
`fee` | BN |
`feeAssetID` | Buffer |

**Returns:** *boolean*

___

###  buildAddDelegatorTx

▸ **buildAddDelegatorTx**(`networkID`: number, `blockchainID`: Buffer, `avaxAssetID`: Buffer, `toAddresses`: Buffer[], `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `rewardLocktime`: BN, `rewardThreshold`: number, `rewardAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:599](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L599)*

Class representing an unsigned [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`avaxAssetID` | Buffer | - | [Buffer](https://github.com/feross/buffer) of the asset ID for AVAX |
`toAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) recieves the stake at the end of the staking period |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

▸ **buildAddSubnetValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `weight`: BN, `subnetID`: string, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `subnetAuth`: [Auth](../modules/api_platformvm_builder.md#auth), `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:490](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L490)*

Class representing an unsigned [AddSubnetValidatorTx](api_platformvm_addsubnetvalidatortx.addsubnetvalidatortx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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
`subnetAuth` | [Auth](../modules/api_platformvm_builder.md#auth) | { addresses: [], threshold: 0, signer: [] } | Optional. An Auth struct which contains the subnet Auth and the signers. |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned transaction created from the passed in parameters.

___

###  buildAddValidatorTx

▸ **buildAddValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `toAddresses`: Buffer[], `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `stakeAssetID`: Buffer, `rewardLocktime`: BN, `rewardThreshold`: number, `rewardAddresses`: Buffer[], `delegationFee`: number, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:729](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L729)*

Class representing an unsigned [AddValidatorTx](api_platformvm_validationtx.addvalidatortx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | NetworkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | BlockchainID, default undefined |
`toAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) recieves the stake at the end of the staking period |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

▸ **buildAddressStateTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `address`: Buffer, `state`: number, `remove`: boolean, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1127](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1127)*

Build an unsigned [AddressStateTx](../modules/src_apis_platformvm.md#addressstatetx).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

▸ **buildBaseTx**(`networkID`: number, `blockchainID`: Buffer, `amount`: BN, `amountAssetID`: Buffer, `toAddresses`: Buffer[], `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `lockTime`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:115](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L115)*

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
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

▸ **buildCaminoAddValidatorTx**(`networkID`: number, `blockchainID`: Buffer, `to`: Buffer[], `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `change`: Buffer[], `nodeID`: Buffer, `nodeOwner`: [NodeOwner](../modules/api_platformvm_builder.md#nodeowner), `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `stakeAssetID`: Buffer, `rewards`: Buffer[], `rewardLocktime`: BN, `rewardThreshold`: number, `memo`: Buffer, `asOf`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1025](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1025)*

Helper function which creates an unsigned [CaminoAddValidatorTx](api_platformvm_validationtx.caminoaddvalidatortx.md). For more granular control, you may create your own
[UnsignedTx](api_evm_transactions.unsignedtx.md) manually and import the [CaminoAddValidatorTx](api_platformvm_validationtx.caminoaddvalidatortx.md) class directly.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`to` | Buffer[] | - | - |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`change` | Buffer[] | - | - |
`nodeID` | Buffer | - | The node ID of the validator being added. |
`nodeOwner` | [NodeOwner](../modules/api_platformvm_builder.md#nodeowner) | - | The address and signature indices of the registered nodeId owner. |
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

###  buildClaimTx

▸ **buildClaimTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number, `claimAmounts`: [ClaimAmountParams](../interfaces/platformvm_interfaces.claimamountparams.md)[], `claimTo`: [OutputOwners](common_output.outputowners.md)): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1445](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1445)*

Build an unsigned [ClaimTx](api_platformvm_claimtx.claimtx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | NetworkID, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | BlockchainID, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | @param fromSigner The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO |
`claimAmounts` | [ClaimAmountParams](../interfaces/platformvm_interfaces.claimamountparams.md)[] | - | The specification and authentication what and how much to claim |
`claimTo` | [OutputOwners](common_output.outputowners.md) | undefined | The address to claimed rewards will be directed to  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned ClaimTx created from the passed in parameters.

___

###  buildCreateChainTx

▸ **buildCreateChainTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `subnetID`: string | Buffer, `chainName`: string, `vmID`: string, `fxIDs`: string[], `genesisData`: string | [GenesisData](api_avm_genesisdata.genesisdata.md), `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `subnetAuth`: [Auth](../modules/api_platformvm_builder.md#auth), `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:928](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L928)*

Build an unsigned [CreateChainTx](api_platformvm_createchaintx.createchaintx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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
`subnetAuth` | [Auth](../modules/api_platformvm_builder.md#auth) | { addresses: [], threshold: 0, signer: [] } | Optional. An Auth struct to sign for the Subnet. |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned CreateChainTx created from the passed in parameters.

___

###  buildCreateSubnetTx

▸ **buildCreateSubnetTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `subnetOwnerAddresses`: Buffer[], `subnetOwnerThreshold`: number, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:846](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L846)*

Class representing an unsigned [CreateSubnetTx](api_platformvm_createsubnettx.createsubnettx.md) transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

▸ **buildDepositTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `depositOfferID`: string | Buffer, `depositDuration`: number | Buffer, `rewardsOwner`: [OutputOwners](common_output.outputowners.md), `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `amountToLock`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1295](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1295)*

Build an unsigned [DepositTx](api_platformvm_deposittx.deposittx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`depositOfferID` | string &#124; Buffer | - | ID of the deposit offer. |
`depositDuration` | number &#124; Buffer | - | Duration of the deposit |
`rewardsOwner` | [OutputOwners](common_output.outputowners.md) | - | Optional The owners of the reward. If omitted, all inputs must have the same owner |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`amountToLock` | BN | - | - |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned DepositTx created from the passed in parameters.

___

###  buildExportTx

▸ **buildExportTx**(`networkID`: number, `blockchainID`: Buffer, `amount`: BN, `amountAssetID`: Buffer, `toAddresses`: Buffer[], `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `destinationChain`: Buffer, `changeAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `locktime`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:373](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L373)*

Creates an unsigned ExportTx transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | - | The number representing NetworkID of the node |
`blockchainID` | Buffer | - | The [Buffer](https://github.com/feross/buffer) representing the BlockchainID for the transaction |
`amount` | BN | - | The amount being exported as a [BN](https://github.com/indutny/bn.js/) |
`amountAssetID` | Buffer | - | - |
`toAddresses` | Buffer[] | - | An array of addresses as [Buffer](https://github.com/feross/buffer) who recieves the AVAX |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

▸ **buildImportTx**(`networkID`: number, `blockchainID`: Buffer, `toAddresses`: Buffer[], `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `atomics`: [UTXO](api_platformvm_utxos.utxo.md)[], `sourceChain`: Buffer, `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `locktime`: BN, `toThreshold`: number, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:210](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L210)*

Creates an unsigned ImportTx transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | - | The number representing NetworkID of the node |
`blockchainID` | Buffer | - | The [Buffer](https://github.com/feross/buffer) representing the BlockchainID for the transaction |
`toAddresses` | Buffer[] | - | The addresses to send the funds |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
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

###  buildMultisigAliasTx

▸ **buildMultisigAliasTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `multisigAliasParams`: [MultisigAliasParams](../interfaces/platformvm_interfaces.multisigaliasparams.md), `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1569](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1569)*

Build an unsigned [MultisigAliasTx](api_platformvm_multisigaliastx.multisigaliastx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Network ID, default [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchain ID, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs |
`multisigAliasParams` | [MultisigAliasParams](../interfaces/platformvm_interfaces.multisigaliasparams.md) | - | Parameters of MultisigAliasTx. multisigAliasParams.ID must be empty if it's the new alias |
`fee` | BN | zero | Optional amount of fees to burn in its smallest denomination, represented as BN |
`feeAssetID` | Buffer | undefined | Optional asset ID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional timestamp to verify the transaction against, as BN |
`changeThreshold` | number | 1 | Optional number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned MultisigAliasTx created from the passed-in parameters.

___

###  buildRegisterNodeTx

▸ **buildRegisterNodeTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `oldNodeID`: Buffer, `newNodeID`: Buffer, `address`: Buffer, `addressAuths`: [][], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1205](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1205)*

Build an unsigned [RegisterNodeTx](api_platformvm_registernodetx.registernodetx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`oldNodeID` | Buffer | undefined | Optional. ID of the existing NodeID to replace or remove. |
`newNodeID` | Buffer | undefined | Optional. ID of the newNodID to register address. |
`address` | Buffer | undefined | The consortiumMemberAddress, single or multi-sig. |
`addressAuths` | [][] | [] | An array of index and address to verify ownership of address. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned RegisterNodeTx created from the passed in parameters.

___

###  buildUnlockDepositTx

▸ **buildUnlockDepositTx**(`networkID`: number, `blockchainID`: Buffer, `fromSigner`: [FromSigner](../modules/api_platformvm_builder.md#fromsigner), `changeAddresses`: Buffer[], `fee`: BN, `feeAssetID`: Buffer, `memo`: Buffer, `asOf`: BN, `changeThreshold`: number): *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

*Defined in [src/apis/platformvm/builder.ts:1377](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L1377)*

Build an unsigned [UnlockDepositTx](api_platformvm_unlockdeposittx.unlockdeposittx.md).

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | - | Blockchainid, default undefined |
`fromSigner` | [FromSigner](../modules/api_platformvm_builder.md#fromsigner) | - | @param fromSigner The addresses being used to send and verify the funds from the UTXOs [Buffer](https://github.com/feross/buffer) |
`changeAddresses` | Buffer[] | - | The addresses that can spend the change remaining from the spent UTXOs. |
`fee` | BN | zero | Optional. The amount of fees to burn in its smallest denomination, represented as [BN](https://github.com/indutny/bn.js/) |
`feeAssetID` | Buffer | undefined | Optional. The assetID of the fees being burned |
`memo` | Buffer | undefined | Optional contains arbitrary bytes, up to 256 bytes |
`asOf` | BN | zero | Optional. The timestamp to verify the transaction against as a [BN](https://github.com/indutny/bn.js/) |
`changeThreshold` | number | 1 | Optional. The number of signatures required to spend the funds in the resultant change UTXO  |

**Returns:** *Promise‹[UnsignedTx](api_platformvm_transactions.unsignedtx.md)›*

An unsigned UnlockDepositTx created from the passed in parameters.
