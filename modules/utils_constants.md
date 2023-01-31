[@c4tplatform/caminojs](../api.md) › [Utils-Constants](utils_constants.md)

# Module: Utils-Constants

## Index

### Type aliases

* [MergeRule](utils_constants.md#mergerule)

### Variables

* [AVAXGWEI](utils_constants.md#const-avaxgwei)
* [AVAXSTAKECAP](utils_constants.md#const-avaxstakecap)
* [CChainAlias](utils_constants.md#const-cchainalias)
* [CChainVMName](utils_constants.md#const-cchainvmname)
* [CENTIAVAX](utils_constants.md#const-centiavax)
* [DECIAVAX](utils_constants.md#const-deciavax)
* [DefaultEVMLocalGenesisAddress](utils_constants.md#const-defaultevmlocalgenesisaddress)
* [DefaultEVMLocalGenesisPrivateKey](utils_constants.md#const-defaultevmlocalgenesisprivatekey)
* [DefaultLocalGenesisPrivateKey](utils_constants.md#const-defaultlocalgenesisprivatekey)
* [DefaultNetworkID](utils_constants.md#const-defaultnetworkid)
* [DefaultPlatformChainID](utils_constants.md#const-defaultplatformchainid)
* [DummyBlockchainID](utils_constants.md#const-dummyblockchainid)
* [DummyPlatformChainID](utils_constants.md#const-dummyplatformchainid)
* [GWEI](utils_constants.md#const-gwei)
* [MICROAVAX](utils_constants.md#const-microavax)
* [MILLIAVAX](utils_constants.md#const-milliavax)
* [NANOAVAX](utils_constants.md#const-nanoavax)
* [NodeIDPrefix](utils_constants.md#const-nodeidprefix)
* [ONEAVAX](utils_constants.md#const-oneavax)
* [PChainAlias](utils_constants.md#const-pchainalias)
* [PChainVMName](utils_constants.md#const-pchainvmname)
* [PrivateKeyPrefix](utils_constants.md#const-privatekeyprefix)
* [TestAvaxAssetID](utils_constants.md#const-testavaxassetid)
* [TestCBlockchainID](utils_constants.md#const-testcblockchainid)
* [TestCChainID](utils_constants.md#const-testcchainid)
* [TestHRP](utils_constants.md#const-testhrp)
* [TestNetworkID](utils_constants.md#const-testnetworkid)
* [TestXBlockchainID](utils_constants.md#const-testxblockchainid)
* [WEI](utils_constants.md#const-wei)
* [XChainAlias](utils_constants.md#const-xchainalias)
* [XChainVMName](utils_constants.md#const-xchainvmname)
* [mnemonic](utils_constants.md#const-mnemonic)

## Type aliases

###  MergeRule

Ƭ **MergeRule**: *"intersection" | "differenceSelf" | "differenceNew" | "symDifference" | "union" | "unionMinusNew" | "unionMinusSelf" | "ERROR"*

*Defined in [src/utils/constants.ts:62](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L62)*

Rules used when merging sets

## Variables

### `Const` AVAXGWEI

• **AVAXGWEI**: *BN* = NANOAVAX.clone()

*Defined in [src/utils/constants.ts:56](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L56)*

___

### `Const` AVAXSTAKECAP

• **AVAXSTAKECAP**: *BN* = ONEAVAX.mul(new BN(3000000))

*Defined in [src/utils/constants.ts:57](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L57)*

___

### `Const` CChainAlias

• **CChainAlias**: *string* = "C"

*Defined in [src/utils/constants.ts:13](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L13)*

___

### `Const` CChainVMName

• **CChainVMName**: *string* = "evm"

*Defined in [src/utils/constants.ts:16](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L16)*

___

### `Const` CENTIAVAX

• **CENTIAVAX**: *BN* = ONEAVAX.div(new BN(100))

*Defined in [src/utils/constants.ts:49](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L49)*

___

### `Const` DECIAVAX

• **DECIAVAX**: *BN* = ONEAVAX.div(new BN(10))

*Defined in [src/utils/constants.ts:48](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L48)*

___

### `Const` DefaultEVMLocalGenesisAddress

• **DefaultEVMLocalGenesisAddress**: *string* = "0x8db97C7cEcE249c2b98bDC0226Cc4C2A57BF52FC"

*Defined in [src/utils/constants.ts:42](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L42)*

___

### `Const` DefaultEVMLocalGenesisPrivateKey

• **DefaultEVMLocalGenesisPrivateKey**: *string* = "0x56289e99c94b6912bfc12adc093c9b51124f0dc54ac7a766b2bc5ccf558d8027"

*Defined in [src/utils/constants.ts:40](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L40)*

___

### `Const` DefaultLocalGenesisPrivateKey

• **DefaultLocalGenesisPrivateKey**: *string* = "ewoqjP7PxY4yr3iLTpLisriqt94hdyDFNgchSxGGztUrTXtNN"

*Defined in [src/utils/constants.ts:38](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L38)*

___

### `Const` DefaultNetworkID

• **DefaultNetworkID**: *1* = 1

*Defined in [src/utils/constants.ts:8](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L8)*

___

### `Const` DefaultPlatformChainID

• **DefaultPlatformChainID**: *string* = "11111111111111111111111111111111LpoYY"

*Defined in [src/utils/constants.ts:23](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L23)*

___

### `Const` DummyBlockchainID

• **DummyBlockchainID**: *"aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa"* = "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa"

*Defined in [src/utils/constants.ts:31](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L31)*

___

### `Const` DummyPlatformChainID

• **DummyPlatformChainID**: *string* = "11111111111111111111111111111111LpoXX"

*Defined in [src/utils/constants.ts:33](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L33)*

___

### `Const` GWEI

• **GWEI**: *BN* = WEI.mul(new BN(1000000000))

*Defined in [src/utils/constants.ts:55](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L55)*

___

### `Const` MICROAVAX

• **MICROAVAX**: *BN* = ONEAVAX.div(new BN(1000000))

*Defined in [src/utils/constants.ts:51](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L51)*

___

### `Const` MILLIAVAX

• **MILLIAVAX**: *BN* = ONEAVAX.div(new BN(1000))

*Defined in [src/utils/constants.ts:50](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L50)*

___

### `Const` NANOAVAX

• **NANOAVAX**: *BN* = ONEAVAX.div(new BN(1000000000))

*Defined in [src/utils/constants.ts:52](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L52)*

___

### `Const` NodeIDPrefix

• **NodeIDPrefix**: *string* = "NodeID-"

*Defined in [src/utils/constants.ts:11](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L11)*

___

### `Const` ONEAVAX

• **ONEAVAX**: *BN* = new BN(1000000000)

*Defined in [src/utils/constants.ts:47](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L47)*

___

### `Const` PChainAlias

• **PChainAlias**: *string* = "P"

*Defined in [src/utils/constants.ts:14](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L14)*

___

### `Const` PChainVMName

• **PChainVMName**: *string* = "platformvm"

*Defined in [src/utils/constants.ts:17](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L17)*

___

### `Const` PrivateKeyPrefix

• **PrivateKeyPrefix**: *string* = "PrivateKey-"

*Defined in [src/utils/constants.ts:10](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L10)*

___

### `Const` TestAvaxAssetID

• **TestAvaxAssetID**: *"2fombhL7aGPwj3KH4bfrmJwW6PVnMobf9Y2fn9GwxiAAJyFDbe"* = "2fombhL7aGPwj3KH4bfrmJwW6PVnMobf9Y2fn9GwxiAAJyFDbe"

*Defined in [src/utils/constants.ts:21](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L21)*

___

### `Const` TestCBlockchainID

• **TestCBlockchainID**: *"2CA6j5zYzasynPsFeNoqWkmTCt3VScMvXUZHbfDJ8k3oGzAPtU"* = "2CA6j5zYzasynPsFeNoqWkmTCt3VScMvXUZHbfDJ8k3oGzAPtU"

*Defined in [src/utils/constants.ts:27](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L27)*

___

### `Const` TestCChainID

• **TestCChainID**: *42112* = 42112

*Defined in [src/utils/constants.ts:29](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L29)*

___

### `Const` TestHRP

• **TestHRP**: *"local"* = "local"

*Defined in [src/utils/constants.ts:19](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L19)*

___

### `Const` TestNetworkID

• **TestNetworkID**: *12345* = 12345

*Defined in [src/utils/constants.ts:20](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L20)*

___

### `Const` TestXBlockchainID

• **TestXBlockchainID**: *"2eNy1mUFdmaxXNj1eQHUe7Np4gju9sJsEtWQ4MX3ToiNKuADed"* = "2eNy1mUFdmaxXNj1eQHUe7Np4gju9sJsEtWQ4MX3ToiNKuADed"

*Defined in [src/utils/constants.ts:25](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L25)*

___

### `Const` WEI

• **WEI**: *BN* = new BN(1)

*Defined in [src/utils/constants.ts:54](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L54)*

___

### `Const` XChainAlias

• **XChainAlias**: *string* = "X"

*Defined in [src/utils/constants.ts:12](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L12)*

___

### `Const` XChainVMName

• **XChainVMName**: *string* = "avm"

*Defined in [src/utils/constants.ts:15](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L15)*

___

### `Const` mnemonic

• **mnemonic**: *string* = "output tooth keep tooth bracket fox city sustain blood raise install pond stem reject long scene clap gloom purpose mean music piece unknown light"

*Defined in [src/utils/constants.ts:44](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/constants.ts#L44)*
