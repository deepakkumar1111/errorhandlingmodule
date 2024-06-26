code for errorhandling module of metacrafter

// SPDX-License-Identifier: MIT

pragma solidity ^0.8.24;

contract Deepak_error_handelling{

    uint public count=0;

    function Calories_Require(uint Calories) public{
        require(Calories > 2000,"Calories  greater than 2000");
        count++;
    }

    function Calories_Revert(uint Calories) public {
        if(!(Calories > 2000)){
            revert("Calories should be greater than 2000");
        }
        count++;
    }

    function Calories_Assert(uint Calories) public{
        assert(Calories > 2000);
        count++;
    }
    }# errorhandlingmodule
