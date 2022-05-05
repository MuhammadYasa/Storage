// SPDX-License-Identifier: MIT

pragma solidity >=0.6.0 <0.9.0;

contract Storage {

    // default value to 0
    uint256 addressNumber;

    
    struct People {
        // default to internal
        uint256 addressNumber; 
        string name;
    }

    People[] public people;
    mapping(string => uint256) public nameToAddressNumber;

    function store(uint256 _addressNumber) public {
        addressNumber = _addressNumber;
    }
    
    function retrieve() public view returns (uint256){
        return addressNumber;
    }

    function addPerson(string memory _name, uint256 _addressNumber) public {
        people.push(People(_addressNumber, _name));
        nameToAddressNumber[_name] = _addressNumber;
    }
}
