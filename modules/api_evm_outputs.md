[@c4tplatform/caminojs](../api.md) › [API-EVM-Outputs](api_evm_outputs.md)

# Module: API-EVM-Outputs

## Index

### Classes

* [AmountOutput](../classes/api_evm_outputs.amountoutput.md)
* [EVMOutput](../classes/api_evm_outputs.evmoutput.md)
* [SECPTransferOutput](../classes/api_evm_outputs.secptransferoutput.md)
* [TransferableOutput](../classes/api_evm_outputs.transferableoutput.md)

### Variables

* [bintools](api_evm_outputs.md#const-bintools)
* [serializer](api_evm_outputs.md#const-serializer)

### Functions

* [SelectOutputClass](api_evm_outputs.md#const-selectoutputclass)

## Variables

### `Const` bintools

• **bintools**: *[BinTools](../classes/utils_bintools.bintools.md)* = BinTools.getInstance()

*Defined in [src/apis/evm/outputs.ts:18](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/evm/outputs.ts#L18)*

___

### `Const` serializer

• **serializer**: *[Serialization](../classes/utils_serialization.serialization.md)‹›* = Serialization.getInstance()

*Defined in [src/apis/evm/outputs.ts:19](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/evm/outputs.ts#L19)*

## Functions

### `Const` SelectOutputClass

▸ **SelectOutputClass**(`outputID`: number, ...`args`: any[]): *[Output](../classes/common_output.output.md)*

*Defined in [src/apis/evm/outputs.ts:28](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/apis/evm/outputs.ts#L28)*

Takes a buffer representing the output and returns the proper Output instance.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`outputID` | number | A number representing the outputID parsed prior to the bytes passed in  |
`...args` | any[] | - |

**Returns:** *[Output](../classes/common_output.output.md)*

An instance of an [Output](src_common.md#output)-extended class.
