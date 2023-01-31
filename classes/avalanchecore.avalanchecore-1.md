[@c4tplatform/caminojs](../README.md) › [AvalancheCore](../modules/avalanchecore.md) › [AvalancheCore](avalanchecore.avalanchecore-1.md)

# Class: AvalancheCore

AvalancheCore is middleware for interacting with Avalanche node RPC APIs.

Example usage:
```js
let avalanche = new AvalancheCore("127.0.0.1", 9650, "https")
```

## Hierarchy

* **AvalancheCore**

  ↳ [Avalanche](avalanche.avalanche-1.md)

## Index

### Constructors

* [constructor](avalanchecore.avalanchecore-1.md#constructor)

### Properties

* [apis](avalanchecore.avalanchecore-1.md#protected-apis)
* [auth](avalanchecore.avalanchecore-1.md#protected-auth)
* [baseEndpoint](avalanchecore.avalanchecore-1.md#protected-baseendpoint)
* [headers](avalanchecore.avalanchecore-1.md#protected-headers)
* [host](avalanchecore.avalanchecore-1.md#protected-host)
* [ip](avalanchecore.avalanchecore-1.md#protected-ip)
* [network](avalanchecore.avalanchecore-1.md#protected-network)
* [networkID](avalanchecore.avalanchecore-1.md#protected-networkid)
* [port](avalanchecore.avalanchecore-1.md#protected-port)
* [protocol](avalanchecore.avalanchecore-1.md#protected-protocol)
* [requestConfig](avalanchecore.avalanchecore-1.md#protected-requestconfig)
* [url](avalanchecore.avalanchecore-1.md#protected-url)

### Methods

* [_setHeaders](avalanchecore.avalanchecore-1.md#protected-_setheaders)
* [addAPI](avalanchecore.avalanchecore-1.md#addapi)
* [api](avalanchecore.avalanchecore-1.md#api)
* [delete](avalanchecore.avalanchecore-1.md#delete)
* [get](avalanchecore.avalanchecore-1.md#get)
* [getBaseEndpoint](avalanchecore.avalanchecore-1.md#getbaseendpoint)
* [getHRP](avalanchecore.avalanchecore-1.md#gethrp)
* [getHeaders](avalanchecore.avalanchecore-1.md#getheaders)
* [getHost](avalanchecore.avalanchecore-1.md#gethost)
* [getIP](avalanchecore.avalanchecore-1.md#getip)
* [getNetwork](avalanchecore.avalanchecore-1.md#getnetwork)
* [getNetworkID](avalanchecore.avalanchecore-1.md#getnetworkid)
* [getPort](avalanchecore.avalanchecore-1.md#getport)
* [getPrimaryAssetAlias](avalanchecore.avalanchecore-1.md#getprimaryassetalias)
* [getProtocol](avalanchecore.avalanchecore-1.md#getprotocol)
* [getRequestConfig](avalanchecore.avalanchecore-1.md#getrequestconfig)
* [getURL](avalanchecore.avalanchecore-1.md#geturl)
* [patch](avalanchecore.avalanchecore-1.md#patch)
* [post](avalanchecore.avalanchecore-1.md#post)
* [put](avalanchecore.avalanchecore-1.md#put)
* [removeAllHeaders](avalanchecore.avalanchecore-1.md#removeallheaders)
* [removeAllRequestConfigs](avalanchecore.avalanchecore-1.md#removeallrequestconfigs)
* [removeHeader](avalanchecore.avalanchecore-1.md#removeheader)
* [removeRequestConfig](avalanchecore.avalanchecore-1.md#removerequestconfig)
* [setAuthToken](avalanchecore.avalanchecore-1.md#setauthtoken)
* [setHeader](avalanchecore.avalanchecore-1.md#setheader)
* [setNetwork](avalanchecore.avalanchecore-1.md#setnetwork)
* [setRequestConfig](avalanchecore.avalanchecore-1.md#setrequestconfig)

## Constructors

###  constructor

\+ **new AvalancheCore**(`host`: string, `port`: number, `protocol`: string, `networkID`: number): *[AvalancheCore](avalanchecore.avalanchecore-1.md)*

*Defined in [src/camino.ts:471](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L471)*

Creates a new Avalanche instance. Sets the address and port of the main Avalanche Client.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`host` | string | The hostname to resolve to reach the Avalanche Client APIs |
`port` | number | The port to resolve to reach the Avalanche Client APIs |
`protocol` | string | The protocol string to use before a "://" in a request, ex: "http", "https", "git", "ws", etc ... |
`networkID` | number | The networkID of the network URL belongs to  |

**Returns:** *[AvalancheCore](avalanchecore.avalanchecore-1.md)*

## Properties

### `Protected` apis

• **apis**: *object*

*Defined in [src/camino.ts:38](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L38)*

#### Type declaration:

* \[ **k**: *string*\]: [APIBase](common_apibase.apibase.md)

___

### `Protected` auth

• **auth**: *string* = undefined

*Defined in [src/camino.ts:35](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L35)*

___

### `Protected` baseEndpoint

• **baseEndpoint**: *string*

*Defined in [src/camino.ts:33](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L33)*

___

### `Protected` headers

• **headers**: *object*

*Defined in [src/camino.ts:36](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L36)*

#### Type declaration:

* \[ **k**: *string*\]: string

___

### `Protected` host

• **host**: *string*

*Defined in [src/camino.ts:31](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L31)*

___

### `Protected` ip

• **ip**: *string*

*Defined in [src/camino.ts:30](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L30)*

___

### `Protected` network

• **network**: *[Network](../interfaces/utils_networks.network.md)* = undefined

*Defined in [src/camino.ts:39](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L39)*

___

### `Protected` networkID

• **networkID**: *number* = 0

*Defined in [src/camino.ts:28](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L28)*

___

### `Protected` port

• **port**: *number*

*Defined in [src/camino.ts:32](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L32)*

___

### `Protected` protocol

• **protocol**: *string*

*Defined in [src/camino.ts:29](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L29)*

___

### `Protected` requestConfig

• **requestConfig**: *AxiosRequestConfig*

*Defined in [src/camino.ts:37](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L37)*

___

### `Protected` url

• **url**: *string*

*Defined in [src/camino.ts:34](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L34)*

## Methods

### `Protected` _setHeaders

▸ **_setHeaders**(`headers`: any): *AxiosRequestHeaders*

*Defined in [src/camino.ts:227](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L227)*

**Parameters:**

Name | Type |
------ | ------ |
`headers` | any |

**Returns:** *AxiosRequestHeaders*

___

###  addAPI

▸ **addAPI**‹**GA**›(`apiName`: string, `ConstructorFN`: object, `baseurl`: string, ...`args`: any[]): *void*

*Defined in [src/camino.ts:266](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L266)*

Adds an API to the middleware. The API resolves to a registered blockchain's RPC.

In TypeScript:
```js
avalanche.addAPI<MyVMClass>("mychain", MyVMClass, "/ext/bc/mychain")
```

In Javascript:
```js
avalanche.addAPI("mychain", MyVMClass, "/ext/bc/mychain")
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

*Defined in [src/camino.ts:288](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L288)*

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

*Defined in [src/camino.ts:373](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L373)*

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

###  get

▸ **get**(`baseurl`: string, `getdata`: object, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Defined in [src/camino.ts:347](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L347)*

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

*Defined in [src/camino.ts:129](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L129)*

Returns the base endpoint for the Avalanche node.

**Returns:** *string*

___

###  getHRP

▸ **getHRP**(): *string*

*Defined in [src/camino.ts:156](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L156)*

Returns the Human-Readable-Part of the network associated with this key.

**Returns:** *string*

The [KeyPair](api_evm_keychain.keypair.md)'s Human-Readable-Part of the network's Bech32 addressing scheme

___

###  getHeaders

▸ **getHeaders**(): *object*

*Defined in [src/camino.ts:139](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L139)*

Returns the custom headers

**Returns:** *object*

___

###  getHost

▸ **getHost**(): *string*

*Defined in [src/camino.ts:114](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L114)*

Returns the host for the Avalanche node.

**Returns:** *string*

___

###  getIP

▸ **getIP**(): *string*

*Defined in [src/camino.ts:119](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L119)*

Returns the IP for the Avalanche node.

**Returns:** *string*

___

###  getNetwork

▸ **getNetwork**(): *[Network](../interfaces/utils_networks.network.md)*

*Defined in [src/camino.ts:104](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L104)*

Returns the network configuration.

**Returns:** *[Network](../interfaces/utils_networks.network.md)*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Defined in [src/camino.ts:149](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L149)*

Returns the networkID

**Returns:** *number*

___

###  getPort

▸ **getPort**(): *number*

*Defined in [src/camino.ts:124](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L124)*

Returns the port for the Avalanche node.

**Returns:** *number*

___

###  getPrimaryAssetAlias

▸ **getPrimaryAssetAlias**(): *string*

*Defined in [src/camino.ts:243](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L243)*

Returns the primary asset alias.

**Returns:** *string*

___

###  getProtocol

▸ **getProtocol**(): *string*

*Defined in [src/camino.ts:109](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L109)*

Returns the protocol such as "http", "https", "git", "ws", etc.

**Returns:** *string*

___

###  getRequestConfig

▸ **getRequestConfig**(): *AxiosRequestConfig*

*Defined in [src/camino.ts:144](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L144)*

Returns the custom request config

**Returns:** *AxiosRequestConfig*

___

###  getURL

▸ **getURL**(): *string*

*Defined in [src/camino.ts:134](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L134)*

Returns the URL of the Avalanche node (ip + port)

**Returns:** *string*

___

###  patch

▸ **patch**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Defined in [src/camino.ts:457](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L457)*

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

*Defined in [src/camino.ts:400](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L400)*

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

*Defined in [src/camino.ts:428](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L428)*

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

*Defined in [src/camino.ts:180](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L180)*

Removes all headers.

**Returns:** *void*

___

###  removeAllRequestConfigs

▸ **removeAllRequestConfigs**(): *void*

*Defined in [src/camino.ts:210](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L210)*

Removes all request configs.

**Returns:** *void*

___

###  removeHeader

▸ **removeHeader**(`key`: string): *void*

*Defined in [src/camino.ts:173](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L173)*

Removes a previously added custom header.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  removeRequestConfig

▸ **removeRequestConfig**(`key`: string): *void*

*Defined in [src/camino.ts:203](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L203)*

Removes a previously added request config.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  setAuthToken

▸ **setAuthToken**(`auth`: string): *void*

*Defined in [src/camino.ts:223](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L223)*

Sets the temporary auth token used for communicating with the node.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`auth` | string | A temporary token provided by the node enabling access to the endpoints on the node.  |

**Returns:** *void*

___

###  setHeader

▸ **setHeader**(`key`: string, `value`: string): *void*

*Defined in [src/camino.ts:164](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L164)*

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

*Defined in [src/camino.ts:53](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L53)*

Sets the address and port of the main Avalanche Client.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`host` | string | - | The hostname to resolve to reach the Avalanche Client RPC APIs. |
`port` | number | - | The port to resolve to reach the Avalanche Client RPC APIs. |
`protocol` | string | - | The protocol string to use before a "://" in a request, ex: "http", "https", etc. Defaults to http |
`networkID` | number | - | - |
`baseEndpoint` | string | "" | the base endpoint to reach the Avalanche Client RPC APIs, ex: "/rpc". Defaults to "/" The following special characters are removed from host and protocol &#,@+()$~%'":*?{} also less than and greater than signs  |

**Returns:** *void*

___

###  setRequestConfig

▸ **setRequestConfig**(`key`: string, `value`: string | boolean): *void*

*Defined in [src/camino.ts:194](https://github.com/chain4travel/caminojs/blob/8077d740/src/camino.ts#L194)*

Adds a new custom config value to be included with all requests.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Config name |
`value` | string &#124; boolean | Config value  |

**Returns:** *void*
