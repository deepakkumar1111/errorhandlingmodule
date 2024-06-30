# Intermediate module 1
### This is the code for errorhandling module of calories of a person..


Contract Initialization
```
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.24;

contract Deepak_error_handelling{

    uint public count=0;
```
Function for required calories

```
    function Calories_Require(uint Calories) public{
        require(Calories > 2000,"Calories  greater than 2000");
        count++;
    }
```
Function for calories revert

```
    function Calories_Revert(uint Calories) public {
        if(!(Calories > 2000)){
            revert("Calories should be greater than 2000");
        }
        count++;
    }
```

Function for calories assert

```
    function Calories_Assert(uint Calories) public{
        assert(Calories > 2000);
        count++;
    }
    }
```
ThankYou
