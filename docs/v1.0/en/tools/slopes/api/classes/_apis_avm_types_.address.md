[slopes - v1.4.3](../README.md) › [Globals](../globals.md) › ["apis/avm/types"](../modules/_apis_avm_types_.md) › [Address](_apis_avm_types_.address.md)

# Class: Address

Class for representing an address used in [Output](_apis_avm_outputs_.output.md) types

## Hierarchy

* [NBytes](_utils_types_.nbytes.md)

  ↳ **Address**

## Index

### Constructors

* [constructor](_apis_avm_types_.address.md#constructor)

### Properties

* [bsize](_apis_avm_types_.address.md#protected-bsize)
* [bytes](_apis_avm_types_.address.md#protected-bytes)

### Methods

* [fromBuffer](_apis_avm_types_.address.md#frombuffer)
* [fromString](_apis_avm_types_.address.md#fromstring)
* [getSize](_apis_avm_types_.address.md#getsize)
* [toBuffer](_apis_avm_types_.address.md#tobuffer)
* [toString](_apis_avm_types_.address.md#tostring)
* [comparitor](_apis_avm_types_.address.md#static-comparitor)

## Constructors

###  constructor

\+ **new Address**(): *[Address](_apis_avm_types_.address.md)*

*Overrides [NBytes](_utils_types_.nbytes.md).[constructor](_utils_types_.nbytes.md#constructor)*

*Defined in [apis/avm/types.ts:102](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/types.ts#L102)*

Class for representing an address used in [Output](_apis_avm_outputs_.output.md) types

**Returns:** *[Address](_apis_avm_types_.address.md)*

## Properties

### `Protected` bsize

• **bsize**: *number*

*Inherited from [NBytes](_utils_types_.nbytes.md).[bsize](_utils_types_.nbytes.md#protected-bsize)*

*Defined in [utils/types.ts:400](https://github.com/ava-labs/slopes/blob/709e172/src/utils/types.ts#L400)*

___

### `Protected` bytes

• **bytes**: *Buffer*

*Inherited from [NBytes](_utils_types_.nbytes.md).[bytes](_utils_types_.nbytes.md#protected-bytes)*

*Defined in [utils/types.ts:399](https://github.com/ava-labs/slopes/blob/709e172/src/utils/types.ts#L399)*

## Methods

###  fromBuffer

▸ **fromBuffer**(`buff`: Buffer): *number*

*Inherited from [NBytes](_utils_types_.nbytes.md).[fromBuffer](_utils_types_.nbytes.md#frombuffer)*

*Defined in [utils/types.ts:433](https://github.com/ava-labs/slopes/blob/709e172/src/utils/types.ts#L433)*

Takes a [[Buffer]], verifies its length, and stores it.

**Parameters:**

Name | Type |
------ | ------ |
`buff` | Buffer |

**Returns:** *number*

The size of the [Buffer](https://github.com/feross/buffer)

___

###  fromString

▸ **fromString**(`addr`: string): *number*

*Overrides [NBytes](_utils_types_.nbytes.md).[fromString](_utils_types_.nbytes.md#fromstring)*

*Defined in [apis/avm/types.ts:86](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/types.ts#L86)*

Takes a base-58 string containing an [Address](_apis_avm_types_.address.md), parses it, populates the class, and returns the length of the Address in bytes.

**Parameters:**

Name | Type |
------ | ------ |
`addr` | string |

**Returns:** *number*

The length of the raw [Address](_apis_avm_types_.address.md)

___

###  getSize

▸ **getSize**(): *number*

*Inherited from [NBytes](_utils_types_.nbytes.md)*

*Defined in [utils/types.ts:407](https://github.com/ava-labs/slopes/blob/709e172/src/utils/types.ts#L407)*

Returns the length of the [Buffer](https://github.com/feross/buffer).

**Returns:** *number*

The exact length requirement of this class

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [NBytes](_utils_types_.nbytes.md).[toBuffer](_utils_types_.nbytes.md#tobuffer)*

*Defined in [utils/types.ts:454](https://github.com/ava-labs/slopes/blob/709e172/src/utils/types.ts#L454)*

Returns the stored [Buffer](https://github.com/feross/buffer).

**Returns:** *Buffer*

A reference to the stored [Buffer](https://github.com/feross/buffer)

___

###  toString

▸ **toString**(): *string*

*Overrides [NBytes](_utils_types_.nbytes.md).[toString](_utils_types_.nbytes.md#tostring)*

*Defined in [apis/avm/types.ts:76](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/types.ts#L76)*

Returns a base-58 representation of the [Address](_apis_avm_types_.address.md).

**Returns:** *string*

___

### `Static` comparitor

▸ **comparitor**(): *function*

*Defined in [apis/avm/types.ts:68](https://github.com/ava-labs/slopes/blob/709e172/src/apis/avm/types.ts#L68)*

Returns a function used to sort an array of [Address](_apis_avm_types_.address.md)es

**Returns:** *function*

▸ (`a`: [Address](_apis_avm_types_.address.md), `b`: [Address](_apis_avm_types_.address.md)): *0 | 1 | -1*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [Address](_apis_avm_types_.address.md) |
`b` | [Address](_apis_avm_types_.address.md) |
