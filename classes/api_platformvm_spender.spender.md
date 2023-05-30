[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Spender](../modules/api_platformvm_spender.md) › [Spender](api_platformvm_spender.spender.md)

# Class: Spender

## Hierarchy

* **Spender**

## Index

### Constructors

* [constructor](api_platformvm_spender.spender.md#constructor)

### Properties

* [platformAPI](api_platformvm_spender.spender.md#platformapi)

### Methods

* [getMinimumSpendable](api_platformvm_spender.spender.md#getminimumspendable)

## Constructors

###  constructor

\+ **new Spender**(`platformAPI`: [PlatformVMAPI](api_platformvm.platformvmapi.md)): *[Spender](api_platformvm_spender.spender.md)*

*Defined in [src/apis/platformvm/spender.ts:14](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/spender.ts#L14)*

**Parameters:**

Name | Type |
------ | ------ |
`platformAPI` | [PlatformVMAPI](api_platformvm.platformvmapi.md) |

**Returns:** *[Spender](api_platformvm_spender.spender.md)*

## Properties

###  platformAPI

• **platformAPI**: *[PlatformVMAPI](api_platformvm.platformvmapi.md)*

*Defined in [src/apis/platformvm/spender.ts:14](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/spender.ts#L14)*

## Methods

###  getMinimumSpendable

▸ **getMinimumSpendable**(`aad`: [AssetAmountDestination](api_platformvm_utxos.assetamountdestination.md), `asOf`: BN, `lockTime`: BN, `lockMode`: [LockMode](../modules/api_platformvm_builder.md#lockmode)): *Promise‹[Error](src_utils.caminoerror.md#static-error)›*

*Defined in [src/apis/platformvm/spender.ts:20](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/spender.ts#L20)*

**Parameters:**

Name | Type |
------ | ------ |
`aad` | [AssetAmountDestination](api_platformvm_utxos.assetamountdestination.md) |
`asOf` | BN |
`lockTime` | BN |
`lockMode` | [LockMode](../modules/api_platformvm_builder.md#lockmode) |

**Returns:** *Promise‹[Error](src_utils.caminoerror.md#static-error)›*
