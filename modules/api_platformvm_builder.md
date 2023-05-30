[@c4tplatform/caminojs](../api.md) › [API-PlatformVM-Builder](api_platformvm_builder.md)

# Module: API-PlatformVM-Builder

## Index

### Classes

* [Builder](../classes/api_platformvm_builder.builder.md)

### Interfaces

* [MinimumSpendable](../interfaces/api_platformvm_builder.minimumspendable.md)

### Type aliases

* [Auth](api_platformvm_builder.md#auth)
* [FromSigner](api_platformvm_builder.md#fromsigner)
* [LockMode](api_platformvm_builder.md#lockmode)
* [NodeOwner](api_platformvm_builder.md#nodeowner)

### Variables

* [zero](api_platformvm_builder.md#const-zero)

## Type aliases

###  Auth

Ƭ **Auth**: *object*

*Defined in [src/apis/platformvm/builder.ts:76](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L76)*

#### Type declaration:

* **addresses**: *Buffer[]*

* **signer**: *[][]*

* **threshold**: *number*

___

###  FromSigner

Ƭ **FromSigner**: *object*

*Defined in [src/apis/platformvm/builder.ts:66](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L66)*

#### Type declaration:

* **from**: *Buffer[]*

* **signer**: *Buffer[]*

___

###  LockMode

Ƭ **LockMode**: *"Unlocked" | "Bond" | "Deposit" | "Stake"*

*Defined in [src/apis/platformvm/builder.ts:55](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L55)*

___

###  NodeOwner

Ƭ **NodeOwner**: *object*

*Defined in [src/apis/platformvm/builder.ts:71](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L71)*

#### Type declaration:

* **address**: *Buffer*

* **auth**: *[][]*

## Variables

### `Const` zero

• **zero**: *BN* = new BN(0)

*Defined in [src/apis/platformvm/builder.ts:82](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/platformvm/builder.ts#L82)*
