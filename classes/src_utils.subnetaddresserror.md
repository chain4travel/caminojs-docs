[camino](../README.md) › [src/utils](../modules/src_utils.md) › [SubnetAddressError](src_utils.subnetaddresserror.md)

# Class: SubnetAddressError

## Hierarchy

  ↳ [CaminoError](src_utils.caminoerror.md)

  ↳ **SubnetAddressError**

## Index

### Constructors

* [constructor](src_utils.subnetaddresserror.md#constructor)

### Properties

* [errorCode](src_utils.subnetaddresserror.md#errorcode)
* [message](src_utils.subnetaddresserror.md#message)
* [name](src_utils.subnetaddresserror.md#name)
* [stack](src_utils.subnetaddresserror.md#optional-stack)

### Methods

* [getCode](src_utils.subnetaddresserror.md#getcode)

## Constructors

###  constructor

\+ **new SubnetAddressError**(`m`: string): *[SubnetAddressError](src_utils.subnetaddresserror.md)*

*Overrides [CaminoError](src_utils.caminoerror.md).[constructor](src_utils.caminoerror.md#constructor)*

*Defined in [src/utils/errors.ts:368](https://github.com/chain4travel/caminojs/blob/ca67b81/src/utils/errors.ts#L368)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[SubnetAddressError](src_utils.subnetaddresserror.md)*

## Properties

###  errorCode

• **errorCode**: *string*

*Inherited from [CaminoError](src_utils.caminoerror.md).[errorCode](src_utils.caminoerror.md#errorcode)*

*Defined in [src/utils/errors.ts:48](https://github.com/chain4travel/caminojs/blob/ca67b81/src/utils/errors.ts#L48)*

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

*Defined in [src/utils/errors.ts:55](https://github.com/chain4travel/caminojs/blob/ca67b81/src/utils/errors.ts#L55)*

**Returns:** *string*
