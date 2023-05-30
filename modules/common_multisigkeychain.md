[@c4tplatform/caminojs](../api.md) › [Common-MultisigKeyChain](common_multisigkeychain.md)

# Module: Common-MultisigKeyChain

## Index

### Classes

* [MultisigKeyChain](../classes/common_multisigkeychain.multisigkeychain.md)
* [MultisigKeyPair](../classes/common_multisigkeychain.multisigkeypair.md)
* [SignatureError](../classes/common_multisigkeychain.signatureerror.md)

### Variables

* [MaxSignatures](common_multisigkeychain.md#const-maxsignatures)
* [NotImplemented](common_multisigkeychain.md#const-notimplemented)
* [TooManySignatures](common_multisigkeychain.md#const-toomanysignatures)
* [bintools](common_multisigkeychain.md#const-bintools)
* [serialization](common_multisigkeychain.md#const-serialization)

## Variables

### `Const` MaxSignatures

• **MaxSignatures**: *256* = 256

*Defined in [src/common/multisigkeychain.ts:26](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L26)*

___

### `Const` NotImplemented

• **NotImplemented**: *[Error](../classes/src_utils.caminoerror.md#static-error)* = new Error("not implemented in MultiSig KeyPair")

*Defined in [src/common/multisigkeychain.ts:21](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L21)*

___

### `Const` TooManySignatures

• **TooManySignatures**: *[SignatureError](../classes/common_multisigkeychain.signatureerror.md)‹›* = new SignatureError("too many signatures")

*Defined in [src/common/multisigkeychain.ts:22](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L22)*

___

### `Const` bintools

• **bintools**: *[BinTools](../classes/utils_bintools.bintools.md)* = BinTools.getInstance()

*Defined in [src/common/multisigkeychain.ts:25](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L25)*

___

### `Const` serialization

• **serialization**: *[Serialization](../classes/utils_serialization.serialization.md)* = Serialization.getInstance()

*Defined in [src/common/multisigkeychain.ts:24](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/multisigkeychain.ts#L24)*
