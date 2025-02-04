[@c4tplatform/caminojs](../api.md) › [Camino](../modules/camino.md) › [Camino](camino.camino-1.md)

# Class: Camino

CaminoJS is middleware for interacting with Camino node RPC APIs.

Example usage:
```js
const camino: Camino = new Camino("127.0.0.1", 9650, "https")
```

## Hierarchy

* [CaminoCore](caminocore.caminocore-1.md)

  ↳ **Camino**

## Index

### Constructors

* [constructor](camino.camino-1.md#constructor)

### Properties

* [apis](camino.camino-1.md#protected-apis)
* [auth](camino.camino-1.md#protected-auth)
* [baseEndpoint](camino.camino-1.md#protected-baseendpoint)
* [headers](camino.camino-1.md#protected-headers)
* [host](camino.camino-1.md#protected-host)
* [ip](camino.camino-1.md#protected-ip)
* [network](camino.camino-1.md#protected-network)
* [networkID](camino.camino-1.md#protected-networkid)
* [port](camino.camino-1.md#protected-port)
* [protocol](camino.camino-1.md#protected-protocol)
* [requestConfig](camino.camino-1.md#protected-requestconfig)
* [url](camino.camino-1.md#protected-url)

### Methods

* [Admin](camino.camino-1.md#admin)
* [Auth](camino.camino-1.md#auth)
* [CChain](camino.camino-1.md#cchain)
* [Health](camino.camino-1.md#health)
* [Index](camino.camino-1.md#index)
* [Info](camino.camino-1.md#info)
* [Metrics](camino.camino-1.md#metrics)
* [NodeKeys](camino.camino-1.md#nodekeys)
* [PChain](camino.camino-1.md#pchain)
* [XChain](camino.camino-1.md#xchain)
* [_setHeaders](camino.camino-1.md#protected-_setheaders)
* [addAPI](camino.camino-1.md#addapi)
* [api](camino.camino-1.md#api)
* [delete](camino.camino-1.md#delete)
* [fetchNetworkSettings](camino.camino-1.md#fetchnetworksettings)
* [get](camino.camino-1.md#get)
* [getBaseEndpoint](camino.camino-1.md#getbaseendpoint)
* [getChains](camino.camino-1.md#getchains)
* [getHRP](camino.camino-1.md#gethrp)
* [getHeaders](camino.camino-1.md#getheaders)
* [getHost](camino.camino-1.md#gethost)
* [getIP](camino.camino-1.md#getip)
* [getNetwork](camino.camino-1.md#getnetwork)
* [getNetworkID](camino.camino-1.md#getnetworkid)
* [getPort](camino.camino-1.md#getport)
* [getPrimaryAssetAlias](camino.camino-1.md#getprimaryassetalias)
* [getProtocol](camino.camino-1.md#getprotocol)
* [getRequestConfig](camino.camino-1.md#getrequestconfig)
* [getURL](camino.camino-1.md#geturl)
* [patch](camino.camino-1.md#patch)
* [post](camino.camino-1.md#post)
* [put](camino.camino-1.md#put)
* [removeAllHeaders](camino.camino-1.md#removeallheaders)
* [removeAllRequestConfigs](camino.camino-1.md#removeallrequestconfigs)
* [removeHeader](camino.camino-1.md#removeheader)
* [removeRequestConfig](camino.camino-1.md#removerequestconfig)
* [setAuthToken](camino.camino-1.md#setauthtoken)
* [setHeader](camino.camino-1.md#setheader)
* [setNetwork](camino.camino-1.md#setnetwork)
* [setRequestConfig](camino.camino-1.md#setrequestconfig)
* [setupAPIs](camino.camino-1.md#protected-setupapis)

## Constructors

###  constructor

\+ **new Camino**(`host`: string, `port`: number, `protocol`: string, `networkID`: number, `XChainID`: string, `CChainID`: string): *[Camino](camino.camino-1.md)*

*Overrides [CaminoCore](caminocore.caminocore-1.md).[constructor](caminocore.caminocore-1.md#constructor)*

*Defined in [src/index.ts:99](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L99)*

Creates a new Camino instance. Sets the address and port of the main Camino Client.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`host` | string | - | The hostname to resolve to reach the Camino Client RPC APIs |
`port` | number | - | The port to resolve to reach the Camino Client RPC APIs |
`protocol` | string | - | The protocol string to use before a "://" in a request, ex: "http", "https", "git", "ws", etc. Defaults to http |
`networkID` | number | undefined | Sets the NetworkID of the class. Default [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`XChainID` | string | undefined | Sets the blockchainID for the AVM. Will try to auto-detect, otherwise default "2eNy1mUFdmaxXNj1eQHUe7Np4gju9sJsEtWQ4MX3ToiNKuADed" |
`CChainID` | string | undefined | Sets the blockchainID for the EVM. Will try to auto-detect, otherwise default "2CA6j5zYzasynPsFeNoqWkmTCt3VScMvXUZHbfDJ8k3oGzAPtU" |

**Returns:** *[Camino](camino.camino-1.md)*

## Properties

### `Protected` apis

• **apis**: *object*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[apis](caminocore.caminocore-1.md#protected-apis)*

*Defined in [src/camino.ts:38](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L38)*

#### Type declaration:

* \[ **k**: *string*\]: [APIBase](common_apibase.apibase.md)

___

### `Protected` auth

• **auth**: *string* = undefined

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[auth](caminocore.caminocore-1.md#protected-auth)*

*Defined in [src/camino.ts:35](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L35)*

___

### `Protected` baseEndpoint

• **baseEndpoint**: *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[baseEndpoint](caminocore.caminocore-1.md#protected-baseendpoint)*

*Defined in [src/camino.ts:33](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L33)*

___

### `Protected` headers

• **headers**: *object*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[headers](caminocore.caminocore-1.md#protected-headers)*

*Defined in [src/camino.ts:36](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L36)*

#### Type declaration:

* \[ **k**: *string*\]: string

___

### `Protected` host

• **host**: *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[host](caminocore.caminocore-1.md#protected-host)*

*Defined in [src/camino.ts:31](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L31)*

___

### `Protected` ip

• **ip**: *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[ip](caminocore.caminocore-1.md#protected-ip)*

*Defined in [src/camino.ts:30](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L30)*

___

### `Protected` network

• **network**: *[Network](../interfaces/utils_networks.network.md)* = undefined

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[network](caminocore.caminocore-1.md#protected-network)*

*Defined in [src/camino.ts:39](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L39)*

___

### `Protected` networkID

• **networkID**: *number* = 0

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[networkID](caminocore.caminocore-1.md#protected-networkid)*

*Defined in [src/camino.ts:28](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L28)*

___

### `Protected` port

• **port**: *number*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[port](caminocore.caminocore-1.md#protected-port)*

*Defined in [src/camino.ts:32](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L32)*

___

### `Protected` protocol

• **protocol**: *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[protocol](caminocore.caminocore-1.md#protected-protocol)*

*Defined in [src/camino.ts:29](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L29)*

___

### `Protected` requestConfig

• **requestConfig**: *AxiosRequestConfig*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[requestConfig](caminocore.caminocore-1.md#protected-requestconfig)*

*Defined in [src/camino.ts:37](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L37)*

___

### `Protected` url

• **url**: *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[url](caminocore.caminocore-1.md#protected-url)*

*Defined in [src/camino.ts:34](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L34)*

## Methods

###  Admin

▸ **Admin**(): *[AdminAPI](api_admin.adminapi.md)‹›*

*Defined in [src/index.ts:53](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L53)*

Returns a reference to the Admin RPC.

**Returns:** *[AdminAPI](api_admin.adminapi.md)‹›*

___

###  Auth

▸ **Auth**(): *[AuthAPI](api_auth.authapi.md)‹›*

*Defined in [src/index.ts:58](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L58)*

Returns a reference to the Auth RPC.

**Returns:** *[AuthAPI](api_auth.authapi.md)‹›*

___

###  CChain

▸ **CChain**(): *[EVMAPI](api_evm.evmapi.md)‹›*

*Defined in [src/index.ts:63](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L63)*

Returns a reference to the EVMAPI RPC pointed at the C-Chain.

**Returns:** *[EVMAPI](api_evm.evmapi.md)‹›*

___

###  Health

▸ **Health**(): *[HealthAPI](api_health.healthapi.md)‹›*

*Defined in [src/index.ts:73](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L73)*

Returns a reference to the Health RPC for a node.

**Returns:** *[HealthAPI](api_health.healthapi.md)‹›*

___

###  Index

▸ **Index**(): *[IndexAPI](api_index.indexapi.md)‹›*

*Defined in [src/index.ts:78](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L78)*

Returns a reference to the Index RPC for a node.

**Returns:** *[IndexAPI](api_index.indexapi.md)‹›*

___

###  Info

▸ **Info**(): *[InfoAPI](api_info.infoapi.md)‹›*

*Defined in [src/index.ts:83](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L83)*

Returns a reference to the Info RPC for a node.

**Returns:** *[InfoAPI](api_info.infoapi.md)‹›*

___

###  Metrics

▸ **Metrics**(): *[MetricsAPI](api_metrics.metricsapi.md)‹›*

*Defined in [src/index.ts:88](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L88)*

Returns a reference to the Metrics RPC.

**Returns:** *[MetricsAPI](api_metrics.metricsapi.md)‹›*

___

###  NodeKeys

▸ **NodeKeys**(): *[KeystoreAPI](api_keystore.keystoreapi.md)‹›*

*Defined in [src/index.ts:94](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L94)*

Returns a reference to the Keystore RPC for a node. We label it "NodeKeys" to reduce
confusion about what it's accessing.

**Returns:** *[KeystoreAPI](api_keystore.keystoreapi.md)‹›*

___

###  PChain

▸ **PChain**(): *[PlatformVMAPI](api_platformvm.platformvmapi.md)‹›*

*Defined in [src/index.ts:99](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L99)*

Returns a reference to the PlatformVM RPC pointed at the P-Chain.

**Returns:** *[PlatformVMAPI](api_platformvm.platformvmapi.md)‹›*

___

###  XChain

▸ **XChain**(): *[AVMAPI](api_avm.avmapi.md)‹›*

*Defined in [src/index.ts:68](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L68)*

Returns a reference to the AVM RPC pointed at the X-Chain.

**Returns:** *[AVMAPI](api_avm.avmapi.md)‹›*

___

### `Protected` _setHeaders

▸ **_setHeaders**(`headers`: any): *AxiosRequestHeaders*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[_setHeaders](caminocore.caminocore-1.md#protected-_setheaders)*

*Defined in [src/camino.ts:235](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L235)*

**Parameters:**

Name | Type |
------ | ------ |
`headers` | any |

**Returns:** *AxiosRequestHeaders*

___

###  addAPI

▸ **addAPI**‹**GA**›(`apiName`: string, `ConstructorFN`: object, `baseurl`: string, ...`args`: any[]): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[addAPI](caminocore.caminocore-1.md#addapi)*

*Defined in [src/camino.ts:274](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L274)*

Adds an API to the middleware. The API resolves to a registered blockchain's RPC.

In TypeScript:
```js
camino.addAPI<MyVMClass>("mychain", MyVMClass, "/ext/bc/mychain")
```

In Javascript:
```js
camino.addAPI("mychain", MyVMClass, "/ext/bc/mychain")
```

**Type parameters:**

▪ **GA**: *[APIBase](common_apibase.apibase.md)*

Class of the API being added

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`apiName` | string | - | A label for referencing the API in the future |
`ConstructorFN` | object | - | A reference to the class which instantiates the API |
`baseurl` | string | undefined | Path to resolve to reach the API   |
`...args` | any[] | - | - |

**Returns:** *void*

___

###  api

▸ **api**‹**GA**›(`apiName`: string): *GA*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[api](caminocore.caminocore-1.md#api)*

*Defined in [src/camino.ts:296](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L296)*

Retrieves a reference to an API by its apiName label.

**Type parameters:**

▪ **GA**: *[APIBase](common_apibase.apibase.md)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`apiName` | string | Name of the API to return  |

**Returns:** *GA*

___

###  delete

▸ **delete**(`baseurl`: string, `getdata`: object, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[delete](caminocore.caminocore-1.md#delete)*

*Defined in [src/camino.ts:381](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L381)*

Makes a DELETE call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the API |
`getdata` | object | - | Object containing the key value pairs sent in DELETE |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  fetchNetworkSettings

▸ **fetchNetworkSettings**(): *Promise‹boolean›*

*Defined in [src/index.ts:133](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L133)*

**Returns:** *Promise‹boolean›*

___

###  get

▸ **get**(`baseurl`: string, `getdata`: object, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[get](caminocore.caminocore-1.md#get)*

*Defined in [src/camino.ts:355](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L355)*

Makes a GET call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the api |
`getdata` | object | - | Object containing the key value pairs sent in GET |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  getBaseEndpoint

▸ **getBaseEndpoint**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getBaseEndpoint](caminocore.caminocore-1.md#getbaseendpoint)*

*Defined in [src/camino.ts:137](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L137)*

Returns the base endpoint for the Camino node.

**Returns:** *string*

___

###  getChains

▸ **getChains**(): *[Chain](../interfaces/utils_networks.chain.md)[]*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getChains](caminocore.caminocore-1.md#getchains)*

*Defined in [src/camino.ts:105](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L105)*

Returns the network chains.

**Returns:** *[Chain](../interfaces/utils_networks.chain.md)[]*

___

###  getHRP

▸ **getHRP**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getHRP](caminocore.caminocore-1.md#gethrp)*

*Defined in [src/camino.ts:164](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L164)*

Returns the Human-Readable-Part of the network associated with this key.

**Returns:** *string*

The [KeyPair](api_evm_keychain.keypair.md)'s Human-Readable-Part of the network's Bech32 addressing scheme

___

###  getHeaders

▸ **getHeaders**(): *object*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getHeaders](caminocore.caminocore-1.md#getheaders)*

*Defined in [src/camino.ts:147](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L147)*

Returns the custom headers

**Returns:** *object*

___

###  getHost

▸ **getHost**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getHost](caminocore.caminocore-1.md#gethost)*

*Defined in [src/camino.ts:122](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L122)*

Returns the host for the Camino node.

**Returns:** *string*

___

###  getIP

▸ **getIP**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getIP](caminocore.caminocore-1.md#getip)*

*Defined in [src/camino.ts:127](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L127)*

Returns the IP for the Camino node.

**Returns:** *string*

___

###  getNetwork

▸ **getNetwork**(): *[Network](../interfaces/utils_networks.network.md)*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getNetwork](caminocore.caminocore-1.md#getnetwork)*

*Defined in [src/camino.ts:100](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L100)*

Returns the network configuration.

**Returns:** *[Network](../interfaces/utils_networks.network.md)*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getNetworkID](caminocore.caminocore-1.md#getnetworkid)*

*Defined in [src/camino.ts:157](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L157)*

Returns the networkID

**Returns:** *number*

___

###  getPort

▸ **getPort**(): *number*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getPort](caminocore.caminocore-1.md#getport)*

*Defined in [src/camino.ts:132](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L132)*

Returns the port for the Camino node.

**Returns:** *number*

___

###  getPrimaryAssetAlias

▸ **getPrimaryAssetAlias**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getPrimaryAssetAlias](caminocore.caminocore-1.md#getprimaryassetalias)*

*Defined in [src/camino.ts:251](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L251)*

Returns the primary asset alias.

**Returns:** *string*

___

###  getProtocol

▸ **getProtocol**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getProtocol](caminocore.caminocore-1.md#getprotocol)*

*Defined in [src/camino.ts:117](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L117)*

Returns the protocol such as "http", "https", "git", "ws", etc.

**Returns:** *string*

___

###  getRequestConfig

▸ **getRequestConfig**(): *AxiosRequestConfig*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getRequestConfig](caminocore.caminocore-1.md#getrequestconfig)*

*Defined in [src/camino.ts:152](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L152)*

Returns the custom request config

**Returns:** *AxiosRequestConfig*

___

###  getURL

▸ **getURL**(): *string*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[getURL](caminocore.caminocore-1.md#geturl)*

*Defined in [src/camino.ts:142](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L142)*

Returns the URL of the Camino node (ip + port)

**Returns:** *string*

___

###  patch

▸ **patch**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[patch](caminocore.caminocore-1.md#patch)*

*Defined in [src/camino.ts:465](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L465)*

Makes a PATCH call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the baseurl |
`getdata` | object | - | Object containing the key value pairs sent in PATCH |
`postdata` | string &#124; object &#124; ArrayBuffer &#124; ArrayBufferView | - | Object containing the key value pairs sent in PATCH |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  post

▸ **post**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[post](caminocore.caminocore-1.md#post)*

*Defined in [src/camino.ts:408](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L408)*

Makes a POST call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the API |
`getdata` | object | - | Object containing the key value pairs sent in POST |
`postdata` | string &#124; object &#124; ArrayBuffer &#124; ArrayBufferView | - | Object containing the key value pairs sent in POST |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  put

▸ **put**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[put](caminocore.caminocore-1.md#put)*

*Defined in [src/camino.ts:436](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L436)*

Makes a PUT call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the baseurl |
`getdata` | object | - | Object containing the key value pairs sent in PUT |
`postdata` | string &#124; object &#124; ArrayBuffer &#124; ArrayBufferView | - | Object containing the key value pairs sent in PUT |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  removeAllHeaders

▸ **removeAllHeaders**(): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[removeAllHeaders](caminocore.caminocore-1.md#removeallheaders)*

*Defined in [src/camino.ts:188](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L188)*

Removes all headers.

**Returns:** *void*

___

###  removeAllRequestConfigs

▸ **removeAllRequestConfigs**(): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[removeAllRequestConfigs](caminocore.caminocore-1.md#removeallrequestconfigs)*

*Defined in [src/camino.ts:218](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L218)*

Removes all request configs.

**Returns:** *void*

___

###  removeHeader

▸ **removeHeader**(`key`: string): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[removeHeader](caminocore.caminocore-1.md#removeheader)*

*Defined in [src/camino.ts:181](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L181)*

Removes a previously added custom header.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  removeRequestConfig

▸ **removeRequestConfig**(`key`: string): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[removeRequestConfig](caminocore.caminocore-1.md#removerequestconfig)*

*Defined in [src/camino.ts:211](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L211)*

Removes a previously added request config.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  setAuthToken

▸ **setAuthToken**(`auth`: string): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[setAuthToken](caminocore.caminocore-1.md#setauthtoken)*

*Defined in [src/camino.ts:231](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L231)*

Sets the temporary auth token used for communicating with the node.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`auth` | string | A temporary token provided by the node enabling access to the endpoints on the node.  |

**Returns:** *void*

___

###  setHeader

▸ **setHeader**(`key`: string, `value`: string): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[setHeader](caminocore.caminocore-1.md#setheader)*

*Defined in [src/camino.ts:172](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L172)*

Adds a new custom header to be included with all requests.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name |
`value` | string | Header value  |

**Returns:** *void*

___

###  setNetwork

▸ **setNetwork**(`host`: string, `port`: number, `protocol`: string, `networkID`: number, `baseEndpoint`: string): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[setNetwork](caminocore.caminocore-1.md#setnetwork)*

*Defined in [src/camino.ts:53](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L53)*

Sets the address and port of the main Camino Client.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`host` | string | - | The hostname to resolve to reach the Camino Client RPC APIs. |
`port` | number | - | The port to resolve to reach the Camino Client RPC APIs. |
`protocol` | string | - | The protocol string to use before a "://" in a request, ex: "http", "https", etc. Defaults to http |
`networkID` | number | - | - |
`baseEndpoint` | string | "" | the base endpoint to reach the Camino Client RPC APIs, ex: "/rpc". Defaults to "/" The following special characters are removed from host and protocol &#,@+()$~%'":*?{} also less than and greater than signs  |

**Returns:** *void*

___

###  setRequestConfig

▸ **setRequestConfig**(`key`: string, `value`: string | boolean): *void*

*Inherited from [CaminoCore](caminocore.caminocore-1.md).[setRequestConfig](caminocore.caminocore-1.md#setrequestconfig)*

*Defined in [src/camino.ts:202](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/camino.ts#L202)*

Adds a new custom config value to be included with all requests.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Config name |
`value` | string &#124; boolean | Config value  |

**Returns:** *void*

___

### `Protected` setupAPIs

▸ **setupAPIs**(`XChainID?`: string, `CChainID?`: string): *boolean*

*Defined in [src/index.ts:220](https://github.com/chain4travel/caminojs/blob/ac57b5af/src/index.ts#L220)*

**Parameters:**

Name | Type |
------ | ------ |
`XChainID?` | string |
`CChainID?` | string |

**Returns:** *boolean*
