# ImplementationAuthority









## Methods

### getImplementation

```solidity
function getImplementation() external view returns (address)
```



*See {IImplementationAuthority-getImplementation}.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### owner

```solidity
function owner() external view returns (address)
```



*Returns the address of the current owner.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### renounceOwnership

```solidity
function renounceOwnership() external nonpayable
```



*Leaves the contract without owner. It will not be possible to call `onlyOwner` functions. Can only be called by the current owner. NOTE: Renouncing ownership will leave the contract without an owner, thereby disabling any functionality that is only available to the owner.*


### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |

### updateImplementation

```solidity
function updateImplementation(address _newImplementation) external nonpayable
```



*See {IImplementationAuthority-updateImplementation}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _newImplementation | address | undefined |



## Events

### OwnershipTransferred

```solidity
event OwnershipTransferred(address indexed previousOwner, address indexed newOwner)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| previousOwner `indexed` | address | undefined |
| newOwner `indexed` | address | undefined |

### UpdatedImplementation

```solidity
event UpdatedImplementation(address newAddress)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| newAddress  | address | undefined |



