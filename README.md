# Clamp.sol
Clamp.sol
pragma solidity ^0.8.20;
contract Clamp {
    function clamp(uint x, uint min, uint max) public pure returns(uint) {
        if(x < min) return min;
        if(x > max) return max;
        return x;
    }
}
