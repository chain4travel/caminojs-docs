[@c4tplatform/caminojs](../api.md) › [src/utils](../modules/src_utils.md) › [AddressError](src_utils.addresserror.md)

# Class: AddressError

## Hierarchy

  ↳ [CaminoError](src_utils.caminoerror.md)

  ↳ **AddressError**

## Index

### Constructors

* [constructor](src_utils.addresserror.md#constructor)

### Properties

* [errorCode](src_utils.addresserror.md#errorcode)
* [message](src_utils.addresserror.md#message)
* [name](src_utils.addresserror.md#name)
* [stack](src_utils.addresserror.md#optional-stack)

### Methods

* [getCode](src_utils.addresserror.md#getcode)

## Constructors

###  constructor

\+ **new AddressError**(`m`: string): *[AddressError](src_utils.addresserror.md)*

*Overrides [CaminoError](src_utils.caminoerror.md).[constructor](src_utils.caminoerror.md#constructor)*

*Defined in [src/utils/errors.ts:60](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/errors.ts#L60)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[AddressError](src_utils.addresserror.md)*

## Properties

###  errorCode

• **errorCode**: *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[errorCode](src_utils.caminoerror.md#errorcode)*

*Defined in [src/utils/errors.ts:48](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/errors.ts#L48)*

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

*Defined in [src/utils/errors.ts:55](https://github.com/chain4travel/caminojs/blob/8077d740/src/utils/errors.ts#L55)*

**Returns:** *string*
