### What's going on in `Mystery.sol`?

Partner: Julian Cervantes

##### Answer: 
Mystery applies the default function of the contract onto the passed in address. Its input is the call data and writes the output over o_code. The function then outputs o_code if there were no errors, but if there was an error (retval == 0), then we jump to a bad destination to signifiy erroring out.
