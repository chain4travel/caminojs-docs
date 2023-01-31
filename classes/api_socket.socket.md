[@c4tplatform/caminojs](../api.md) › [API-Socket](../modules/api_socket.md) › [Socket](api_socket.socket.md)

# Class: Socket

## Hierarchy

* any

  ↳ **Socket**

## Index

### Constructors

* [constructor](api_socket.socket.md#constructor)

### Properties

* [onclose](api_socket.socket.md#onclose)
* [onerror](api_socket.socket.md#onerror)
* [onmessage](api_socket.socket.md#onmessage)
* [onopen](api_socket.socket.md#onopen)

### Methods

* [close](api_socket.socket.md#close)
* [send](api_socket.socket.md#send)

## Constructors

###  constructor

\+ **new Socket**(`url`: string, `options?`: WebSocket.ClientOptions | ClientRequestArgs): *[Socket](api_socket.socket.md)*

*Defined in [src/apis/socket/socket.ts:35](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L35)*

Provides the API for creating and managing a WebSocket connection to a server, as well as for sending and receiving data on the connection.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`url` | string | Defaults to [[MainnetAPI]] |
`options?` | WebSocket.ClientOptions &#124; ClientRequestArgs | Optional  |

**Returns:** *[Socket](api_socket.socket.md)*

## Properties

###  onclose

• **onclose**: *any*

*Defined in [src/apis/socket/socket.ts:13](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L13)*

___

###  onerror

• **onerror**: *any*

*Defined in [src/apis/socket/socket.ts:15](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L15)*

___

###  onmessage

• **onmessage**: *any*

*Defined in [src/apis/socket/socket.ts:11](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L11)*

___

###  onopen

• **onopen**: *any*

*Defined in [src/apis/socket/socket.ts:9](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L9)*

## Methods

###  close

▸ **close**(`mcode?`: number, `data?`: string): *void*

*Defined in [src/apis/socket/socket.ts:33](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L33)*

Terminates the connection completely

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`mcode?` | number | Optional |
`data?` | string | Optional  |

**Returns:** *void*

___

###  send

▸ **send**(`data`: any, `cb?`: any): *void*

*Defined in [src/apis/socket/socket.ts:23](https://github.com/chain4travel/caminojs/blob/8077d740/src/apis/socket/socket.ts#L23)*

Send a message to the server

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`data` | any | - |
`cb?` | any | Optional  |

**Returns:** *void*
