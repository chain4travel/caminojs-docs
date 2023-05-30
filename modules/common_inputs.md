[@c4tplatform/caminojs](../api.md) › [Common-Inputs](common_inputs.md)

# Module: Common-Inputs

## Index

### Classes

* [Input](../classes/common_inputs.input.md)
* [StandardAmountInput](../classes/common_inputs.standardamountinput.md)
* [StandardParseableInput](../classes/common_inputs.standardparseableinput.md)
* [StandardTransferableInput](../classes/common_inputs.standardtransferableinput.md)

### Interfaces

* [BaseInput](../interfaces/common_inputs.baseinput.md)

### Variables

* [serialization](common_inputs.md#const-serialization)

### Functions

* [BaseInputComparator](common_inputs.md#const-baseinputcomparator)

## Variables

### `Const` serialization

• **serialization**: *[Serialization](../classes/utils_serialization.serialization.md)* = Serialization.getInstance()

*Defined in [src/common/input.ts:19](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L19)*

## Functions

### `Const` BaseInputComparator

▸ **BaseInputComparator**(): *function*

*Defined in [src/common/input.ts:39](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/common/input.ts#L39)*

**Returns:** *function*

▸ (`a`: [BaseInput](../interfaces/common_inputs.baseinput.md), `b`: [BaseInput](../interfaces/common_inputs.baseinput.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [BaseInput](../interfaces/common_inputs.baseinput.md) |
`b` | [BaseInput](../interfaces/common_inputs.baseinput.md) |
