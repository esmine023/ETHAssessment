# ETHAssessment

This program initializes the very core of using solidity assessment and that is creating a token between all those modules accumulated into one.

## Description

This is a special program that certifies as something evolutionary throughout decades to come and this will be able to help us navigate through the blockchain Ethereum. And by doing so in a most conventional way; Through the world of coding! this serves as a testament that blockchain is the stepping stone beyond the horizon.

## Getting started
 ### Installing the software
   This is the easy and most efficient way to get through the Blockchain stuff. Just get to https://remix.ethereum.org/. and get started with your token! Of course, it's not THAT easy isn't it? well just press the plus (+) button and you're good to code! (with minor adjustments like naming your file with .sol whichever you like )
   Secondly, you'd need to copy and paste the code regarding the final assessment and then follow Chris' instructions on how to efficiently use the remix and the coding altogether

```javascript
contract MyToken {

    // public variables here
    string public tokenName = "LOVER";
    string public tokenAbbrv = "LVR";
    uint public totalSupply = 0;


    // mapping variable here
    mapping(address => uint) public balances;


```

You'll need to put variables of your Token name and the Abbreviation of that token (as stated in here, i did caps-on 'lover' and the abbreviation of it being 'lvr' with all caps) 
and initiating with mapping the variable (making the Address => uint as your public balances)

```javascript

 // mint function
    function mint (address _address, uint _value) public {
        totalSupply += _value;
        balances [_address] += _value;
     }

    // burn function
    function burn (address _address, uint _value) public {
        if (balances [_address ] >= _value) {

        totalSupply -= _value;
        balances [_address] -= _value;
        }
        
    }

```
in the second one we would need to do the burn and minting function which is basically the same except using the functions of  '+=' on the mint function while in the burn function 
you'll be using the opposite which is '-='
and calling the total supply and the balances altogether

once this is all connected you'll need to open the "solidity compiler" on the left side of the remix.etherium.org (which you'll be doing your compiling) and use the 'compile my token.sol' which is located at the left side. once that's done it will run on the bottom of the website saying it ran. 

4th thing you'll need to do is deploy and run tab which is located below at the solidity compiler button. with it opening, you'll see the orange button that says deploy which grants you to see if your token is available or not. You'll have to test the waters a.k.a the tokens(abbrv, name, and total supply buttons) within the 'deployed contracts'

lastly and most importantly youll need to copy your account which is directed at the depoly and run transactions and copy paste it and opening the mint and burn below the deployed contracts. Giving them value and pasting the account numbers you just got and putting them into the address section and giving value to the value section. When ran by the token abbrv it will give the certain amount of you just did (500 for example) and giving it the total supply of also 500. the same with Burn section, same sequence different number (1000 for example) and testing it with the totalsupply section and the token abbrv and you're done! that's the whole sequence of mytoken! 


   ### Advice
   Any advice can ask @ the discord with faith/Chris as my guide!

   ### Authors
   Rafanan, Jay-Ann
   @sakiwaree on discord
