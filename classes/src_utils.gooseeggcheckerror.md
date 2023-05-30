[@c4tplatform/caminojs](../api.md) › [src/utils](../modules/src_utils.md) › [GooseEggCheckError](src_utils.gooseeggcheckerror.md)

# Class: GooseEggCheckError

## Hierarchy

  ↳ [CaminoError](src_utils.caminoerror.md)

  ↳ **GooseEggCheckError**

## Index

### Constructors

* [constructor](src_utils.gooseeggcheckerror.md#constructor)

### Properties

* [errorCode](src_utils.gooseeggcheckerror.md#errorcode)
* [message](src_utils.gooseeggcheckerror.md#message)
* [name](src_utils.gooseeggcheckerror.md#name)
* [stack](src_utils.gooseeggcheckerror.md#optional-stack)

### Methods

* [getCode](src_utils.gooseeggcheckerror.md#getcode)

## Constructors

###  constructor

\+ **new GooseEggCheckError**(`m`: string): *[GooseEggCheckError](src_utils.gooseeggcheckerror.md)*

*Overrides [CaminoError](src_utils.caminoerror.md).[constructor](src_utils.caminoerror.md#constructor)*

*Defined in [src/utils/errors.ts:67](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/utils/errors.ts#L67)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[GooseEggCheckError](src_utils.gooseeggcheckerror.md)*

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
