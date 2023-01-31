[@c4tplatform/caminojs](../api.md) › [API-Health](../modules/api_health.md) › [HealthAPI](api_health.healthapi.md)

# Class: HealthAPI

Class for interacting with a node API that is using the node's HealthApi.

**`remarks`** This extends the [JRPCAPI](../modules/src_common.md#jrpcapi) class. This class should not be directly called. Instead, use the [Camino.addAPI](camino.camino-1.md#addapi) function to register this interface with Camino.

## Hierarchy

  ↳ [JRPCAPI](common_jrpcapi.jrpcapi.md)

  ↳ **HealthAPI**

## Index

### Constructors

* [constructor](api_health.healthapi.md#constructor)

### Properties

* [baseURL](api_health.healthapi.md#protected-baseurl)
* [core](api_health.healthapi.md#protected-core)
* [db](api_health.healthapi.md#protected-db)
* [jrpcVersion](api_health.healthapi.md#protected-jrpcversion)
* [rpcID](api_health.healthapi.md#protected-rpcid)

### Methods

* [callMethod](api_health.healthapi.md#callmethod)
* [getBaseURL](api_health.healthapi.md#getbaseurl)
* [getDB](api_health.healthapi.md#getdb)
* [getRPCID](api_health.healthapi.md#getrpcid)
* [health](api_health.healthapi.md#health)
* [setBaseURL](api_health.healthapi.md#setbaseurl)

## Constructors

###  constructor

\+ **new HealthAPI**(`core`: [CaminoCore](caminocore.caminocore-1.md), `baseURL`: string): *[HealthAPI](api_health.healthapi.md)*

*Overrides [JRPCAPI](common_jrpcapi.jrpcapi.md).[constructor](common_jrpcapi.jrpcapi.md#constructor)*

*Defined in [src/apis/health/api.ts:25](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/health/api.ts#L25)*

This class should not be instantiated directly. Instead use the [Camino.addAPI](camino.camino-1.md#addapi) method.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`core` | [CaminoCore](caminocore.caminocore-1.md) | - | A reference to the Camino class |
`baseURL` | string | "/ext/health" | Defaults to the string "/ext/health" as the path to rpc's baseURL  |

**Returns:** *[HealthAPI](api_health.healthapi.md)*

## Properties

### `Protected` baseURL

• **baseURL**: *string*

*Inherited from [APIBase](common_apibase.apibase.md).[baseURL](common_apibase.apibase.md#protected-baseurl)*

*Defined in [src/common/apibase.ts:29](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/apibase.ts#L29)*

___

### `Protected` core

• **core**: *[CaminoCore](caminocore.caminocore-1.md)*

*Inherited from [APIBase](common_apibase.apibase.md).[core](common_apibase.apibase.md#protected-core)*

*Defined in [src/common/apibase.ts:28](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/apibase.ts#L28)*

___

### `Protected` db

• **db**: *StoreAPI*

*Inherited from [APIBase](common_apibase.apibase.md).[db](common_apibase.apibase.md#protected-db)*

*Defined in [src/common/apibase.ts:30](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/apibase.ts#L30)*

___

### `Protected` jrpcVersion

• **jrpcVersion**: *string* = "2.0"

*Inherited from [EVMAPI](api_evm.evmapi.md).[jrpcVersion](api_evm.evmapi.md#protected-jrpcversion)*

*Defined in [src/common/jrpcapi.ts:13](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/jrpcapi.ts#L13)*

___

### `Protected` rpcID

• **rpcID**: *number* = 1

*Inherited from [EVMAPI](api_evm.evmapi.md).[rpcID](api_evm.evmapi.md#protected-rpcid)*

*Defined in [src/common/jrpcapi.ts:14](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/jrpcapi.ts#L14)*

## Methods

###  callMethod

▸ **callMethod**(`method`: string, `params?`: object[] | object, `baseURL?`: string, `headers?`: object): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [EVMAPI](api_evm.evmapi.md).[callMethod](api_evm.evmapi.md#callmethod)*

*Defined in [src/common/jrpcapi.ts:16](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/jrpcapi.ts#L16)*

**Parameters:**

Name | Type |
------ | ------ |
`method` | string |
`params?` | object[] &#124; object |
`baseURL?` | string |
`headers?` | object |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

___

###  getBaseURL

▸ **getBaseURL**(): *string*

*Inherited from [APIBase](common_apibase.apibase.md).[getBaseURL](common_apibase.apibase.md#getbaseurl)*

*Defined in [src/common/apibase.ts:53](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/apibase.ts#L53)*

Returns the baseURL's path.

**Returns:** *string*

___

###  getDB

▸ **getDB**(): *StoreAPI*

*Inherited from [APIBase](common_apibase.apibase.md).[getDB](common_apibase.apibase.md#getdb)*

*Defined in [src/common/apibase.ts:58](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/apibase.ts#L58)*

Returns the baseURL's database.

**Returns:** *StoreAPI*

___

###  getRPCID

▸ **getRPCID**(): *number*

*Inherited from [EVMAPI](api_evm.evmapi.md).[getRPCID](api_evm.evmapi.md#getrpcid)*

*Defined in [src/common/jrpcapi.ts:79](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/jrpcapi.ts#L79)*

Returns the rpcid, a strictly-increasing number, starting from 1, indicating the next
request ID that will be sent.

**Returns:** *number*

___

###  health

▸ **health**(): *Promise‹[HealthResponse](../interfaces/health_interfaces.healthresponse.md)›*

*Defined in [src/apis/health/api.ts:22](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/health/api.ts#L22)*

**Returns:** *Promise‹[HealthResponse](../interfaces/health_interfaces.healthresponse.md)›*

Promise for a [HealthResponse](../interfaces/health_interfaces.healthresponse.md)

___

###  setBaseURL

▸ **setBaseURL**(`baseURL`: string): *void*

*Inherited from [APIBase](common_apibase.apibase.md).[setBaseURL](common_apibase.apibase.md#setbaseurl)*

*Defined in [src/common/apibase.ts:37](https://github.com/chain4travel/caminojs/blob/8077d740/src/common/apibase.ts#L37)*

Sets the path of the APIs baseURL.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`baseURL` | string | Path of the APIs baseURL - ex: "/ext/bc/X"  |

**Returns:** *void*
