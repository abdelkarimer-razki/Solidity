# Making the Zombie Factory

In this readme, I'll go through the code of the first course on the CryptoZombies website to explain the things that I believe were new for me.
First of all,

```solidity
pragma solidity >=0.5.0 <0.6.0;
```

This line is meant for the solidity compiler to know the version of solidity that is being used on this file, in order to prevent issues with future updates of the compiler, in this case, it’s between 0.5.0 and 0.6.0.

Secondly,

```solidity
event NewZombie(uint zombieId, string name, uint dna);
```

Event is a concept that I saw the first time here in solidity, and it is actually meant to notify the client application that an action has been done in the smart contract.

Read [this](https://betterprogramming.pub/what-is-an-event-in-solidity-420caeb38859) to see a case of use. 

```solidity
emit NewZombie(id, _name, _dna);
```

The `emit` keyword is used to throw out a specific event to notify that an action has been done, in this case, the event is `NewZombie` to notify the client application that a new zombie has been created.

More informations about how the events being emited in etheruem blockchain [here](https://www.notion.so/Making-the-Zombie-Factory-690acf11e75a4fd7824d73d253a51172).
