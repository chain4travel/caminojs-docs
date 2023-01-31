[@c4tplatform/caminojs](../README.md) › [Utils-Networks](utils_networks.md)

# Module: Utils-Networks

## Index

### Classes

* [Networks](../classes/utils_networks.networks.md)

### Interfaces

* [C](../interfaces/utils_networks.c.md)
* [Network](../interfaces/utils_networks.network.md)
* [P](../interfaces/utils_networks.p.md)
* [X](../interfaces/utils_networks.x.md)

### Object literals

* [AvaxMainNetwork](utils_networks.md#const-avaxmainnetwork)
* [TestNetwork](utils_networks.md#const-testnetwork)

## Object literals

### `Const` AvaxMainNetwork

### ▪ **AvaxMainNetwork**: *object*

*Defined in [src/utils/networks.ts:128](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L128)*

###  hrp

• **hrp**: *string* = "avax"

*Defined in [src/utils/networks.ts:129](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L129)*

▪ **C**: *object*

*Defined in [src/utils/networks.ts:160](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L160)*

* **alias**: *string* = CChainAlias

* **blockchainID**: *string* = "2q9e4r6Mu3U68nU1fYjgbR6JvwrRx36CohpAX5UQxse55x1Q5"

* **chainID**: *number* = 43114

* **costPerSignature**: *number* = 1000

* **gasPrice**: *BN‹›* = GWEI.mul(new BN(225))

* **maxGasPrice**: *BN‹›* = GWEI.mul(new BN(1000))

* **minGasPrice**: *BN‹›* = GWEI.mul(new BN(25))

* **txBytesGas**: *number* = 1

* **txFee**: *BN‹›* = MILLIAVAX

* **vm**: *string* = CChainVMName

▪ **P**: *object*

*Defined in [src/utils/networks.ts:140](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L140)*

* **alias**: *string* = PChainAlias

* **blockchainID**: *string* = DefaultPlatformChainID

* **createChainTx**: *BN‹›* = ONEAVAX

* **createSubnetTx**: *BN‹›* = ONEAVAX

* **creationTxFee**: *BN‹›* = CENTIAVAX

* **lockModeBondDeposit**: *false* = false

* **maxConsumption**: *number* = 0.12

* **maxStakeDuration**: *number* = 365 * 24 * 60 * 60

* **maxStakingDuration**: *BN‹›* = new BN(31536000)

* **maxSupply**: *BN‹›* = new BN(720000000).mul(ONEAVAX)

* **minConsumption**: *number* = 0.1

* **minDelegationFee**: *BN‹›* = new BN(2)

* **minDelegationStake**: *BN‹›* = ONEAVAX.mul(new BN(25))

* **minStake**: *BN‹›* = ONEAVAX.mul(new BN(2000))

* **minStakeDuration**: *number* = 2 * 7 * 24 * 60 * 60

* **txFee**: *BN‹›* = MILLIAVAX

* **verifyNodeSignature**: *false* = false

* **vm**: *string* = PChainVMName

▪ **X**: *object*

*Defined in [src/utils/networks.ts:130](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L130)*

* **alias**: *string* = XChainAlias

* **avaxAssetAlias**: *string* = "AVAX"

* **avaxAssetID**: *string* = "FvwEAhmxKfeiG8SnEvq42hc6whRyY3EFYAvebMqDNDGCgxN5Z"

* **blockchainID**: *string* = "2oYMBNV4eNHyqk2fjjV5nVQLDbtmNJzq5s3qs3Lo6ftnC6FByM"

* **creationTxFee**: *BN‹›* = CENTIAVAX

* **mintTxFee**: *BN‹›* = MILLIAVAX

* **txFee**: *BN‹›* = MILLIAVAX

* **vm**: *string* = XChainVMName

___

### `Const` TestNetwork

### ▪ **TestNetwork**: *object*

*Defined in [src/utils/networks.ts:81](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L81)*

###  hrp

• **hrp**: *string* = TestHRP

*Defined in [src/utils/networks.ts:82](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L82)*

▪ **C**: *object*

*Defined in [src/utils/networks.ts:113](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L113)*

* **alias**: *string* = CChainAlias

* **blockchainID**: *string* = TestCBlockchainID

* **chainID**: *number* = 43112

* **costPerSignature**: *number* = 1000

* **gasPrice**: *BN‹›* = GWEI.mul(new BN(225))

* **maxGasPrice**: *BN‹›* = GWEI.mul(new BN(1000))

* **minGasPrice**: *BN‹›* = GWEI.mul(new BN(25))

* **txBytesGas**: *number* = 1

* **txFee**: *BN‹›* = MILLIAVAX

* **vm**: *string* = CChainVMName

▪ **P**: *object*

*Defined in [src/utils/networks.ts:93](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L93)*

* **alias**: *string* = PChainAlias

* **blockchainID**: *string* = DefaultPlatformChainID

* **createChainTx**: *BN‹›* = ONEAVAX

* **createSubnetTx**: *BN‹›* = ONEAVAX

* **creationTxFee**: *BN‹›* = CENTIAVAX

* **lockModeBondDeposit**: *false* = false

* **maxConsumption**: *number* = 0.12

* **maxStakeDuration**: *number* = 365 * 24 * 60 * 60

* **maxStakingDuration**: *BN‹›* = new BN(31536000)

* **maxSupply**: *BN‹›* = new BN(720000000).mul(ONEAVAX)

* **minConsumption**: *number* = 0.1

* **minDelegationFee**: *BN‹›* = new BN(2)

* **minDelegationStake**: *BN‹›* = ONEAVAX

* **minStake**: *BN‹›* = ONEAVAX

* **minStakeDuration**: *number* = 24 * 60 * 60

* **txFee**: *BN‹›* = MILLIAVAX

* **verifyNodeSignature**: *false* = false

* **vm**: *string* = PChainVMName

▪ **X**: *object*

*Defined in [src/utils/networks.ts:83](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/networks.ts#L83)*

* **alias**: *string* = XChainAlias

* **avaxAssetAlias**: *string* = "AVAX"

* **avaxAssetID**: *string* = TestAvaxAssetID

* **blockchainID**: *string* = TestXBlockchainID

* **creationTxFee**: *BN‹›* = CENTIAVAX

* **mintTxFee**: *BN‹›* = MILLIAVAX

* **txFee**: *BN‹›* = MILLIAVAX

* **vm**: *string* = XChainVMName
