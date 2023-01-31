[@c4tplatform/caminojs](../README.md) › [Common-Output](common_output.md)

# Module: Common-Output

## Index

### Classes

* [Address](../classes/common_output.address.md)
* [BaseNFTOutput](../classes/common_output.basenftoutput.md)
* [Output](../classes/common_output.output.md)
* [OutputOwners](../classes/common_output.outputowners.md)
* [StandardAmountOutput](../classes/common_output.standardamountoutput.md)
* [StandardParseableOutput](../classes/common_output.standardparseableoutput.md)
* [StandardTransferableOutput](../classes/common_output.standardtransferableoutput.md)

### Interfaces

* [BaseOutput](../interfaces/common_output.baseoutput.md)

### Variables

* [serialization](common_output.md#const-serialization)

### Functions

* [BaseOutputComparator](common_output.md#const-baseoutputcomparator)

## Variables

### `Const` serialization

• **serialization**: *[Serialization](../classes/utils_serialization.serialization.md)* = Serialization.getInstance()

*Defined in [src/common/output.ts:22](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L22)*

## Functions

### `Const` BaseOutputComparator

▸ **BaseOutputComparator**(): *function*

*Defined in [src/common/output.ts:42](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/output.ts#L42)*

**Returns:** *function*

▸ (`a`: [BaseOutput](../interfaces/common_output.baseoutput.md), `b`: [BaseOutput](../interfaces/common_output.baseoutput.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [BaseOutput](../interfaces/common_output.baseoutput.md) |
`b` | [BaseOutput](../interfaces/common_output.baseoutput.md) |
