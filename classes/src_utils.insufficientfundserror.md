[@c4tplatform/caminojs](../api.md) › [src/utils](../modules/src_utils.md) › [InsufficientFundsError](src_utils.insufficientfundserror.md)

# Class: InsufficientFundsError

## Hierarchy

  ↳ [CaminoError](src_utils.caminoerror.md)

  ↳ **InsufficientFundsError**

## Index

### Constructors

* [constructor](src_utils.insufficientfundserror.md#constructor)

### Properties

* [errorCode](src_utils.insufficientfundserror.md#errorcode)
* [message](src_utils.insufficientfundserror.md#message)
* [name](src_utils.insufficientfundserror.md#name)
* [stack](src_utils.insufficientfundserror.md#optional-stack)

### Methods

* [getCode](src_utils.insufficientfundserror.md#getcode)

## Constructors

###  constructor

\+ **new InsufficientFundsError**(`m`: string): *[InsufficientFundsError](src_utils.insufficientfundserror.md)*

*Overrides [CaminoError](src_utils.caminoerror.md).[constructor](src_utils.caminoerror.md#constructor)*

*Defined in [src/utils/errors.ts:179](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/errors.ts#L179)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[InsufficientFundsError](src_utils.insufficientfundserror.md)*

## Properties

###  errorCode

• **errorCode**: *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[errorCode](src_utils.caminoerror.md#errorcode)*

*Defined in [src/utils/errors.ts:48](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/errors.ts#L48)*

___

###  message

• **message**: *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[message](src_utils.caminoerror.md#message)*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1029

___

###  name

• **name**: *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[name](src_utils.caminoerror.md#name)*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1028

___

### `Optional` stack

• **stack**? : *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[stack](src_utils.caminoerror.md#optional-stack)*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1030

## Methods

###  getCode

▸ **getCode**(): *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[getCode](src_utils.caminoerror.md#getcode)*

*Defined in [src/utils/errors.ts:55](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/errors.ts#L55)*

**Returns:** *string*
