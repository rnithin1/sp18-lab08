### What's going on in `Mystery.sol`?

##### Answer: <br>
The function sets o_code equal to the next available memory address, and invokes
the default function of the contract on the address initially passed in. Its input
is a copy of the calldata, and it writes the output to o_code. If it threw, then 
jump to the bad memory address 0x02. Else, return o_code.
