In this code we have created a kind of wallet or mechanism which mints or burns tokens. 

//PUBLIC VARIABLES
For this we have created three variables:
1) token_Name which stores token name
2) token_Abbrev which stores the abbrevation of the token
3) total_Supply which stores the total supply of the tokens

//MAPING
Then we mapped the variables and returned the balances.

// MINT FUNCTION
After this we have created a MINT function which takes (input) the 
1) _address in which token are to be minted and
2) _value that how much token are to be minted.

The function adds the number of token (specified in the _value variable) to the total supply.
And add the same number of tokens to the balances of the the given address(Specifies in _address variable)

// BURN FUNCTION
Then we have created a BURN function which is opposite of MINT function:
1) _address(the address from which the tokens are to be deducted) and
2) _value(the number of tokens to be deducted).

This BURN function works on the following condition:
If total_Supply is greater than or equal to _value.
If the condition satisfied then
1) total_Supply is reduced by _value and
2) balances of the given _address is reduced by _value.
