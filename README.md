# Jacob-Awesome-Course-on-FLOW

Chapter 1 - Day 1 - Learning Blockchain Concepts

1.	Explain what the Blockchain is in your own words. 

Blockchain is an open, decentralized, shared database that allows anyone to store stuff publically. Anyone can interact with it with approval and it belongs to nobody that everyone can store information or view the data on it. 

2.	Explain what a Smart Contract is. 

Smart Contracts are programs, or "rulebooks" that developers make that users can interact with according to a pre-set rules that nobody can change it or play the other way around it, unless it’s designed to be allowed since day 1. 

3.	Explain the difference between a script and a transaction.

A script does not cost any money and it won’t change the data on blockchain but only view it; A transaction does involve fee(gas fee) and change data on blockchain.



Chapter 1 - Day 2 - The Flow Blockchain & Cadence

1.	What are the 5 Cadence Programming Language Pillars?

Safety and Security: It makes smart contract secure by separation between contracts and transactions

Clarity: Its code is easy to read by allowing the developer to express their intentions directly so that users can verify it is safe. 

Approachability: The way Cadence is written is very familiar to other programming languages like Swift and Rust, making it easy to transition to if you have prior experience.

Developer Experience: Cadence let developer debug in an easy mamner by making error messages very clear.

Resource Oriented Programming: Resources are a composite data type, similar to a struct, that expresses direct ownership of assets. Cadence’s resources directly tie an asset’s ownership to the account that owns it by saving the resource in the account’s storage. As a result, ownership isn’t centralized in a smart contract’s storage, but each account owns its assets. 

2.	In your opinion, even without knowing anything about the Blockchain or coding, why could the 5 Pillars be useful (you don't have to answer this for #5)?

In my humble opinion, Dapper Labs did see the problems of Ethereum when they had gained huge success in Cryptokitties: high gas fee, low security and thus scalability in doubt. Instead of making more NFTs, they went further to create another blockchain that is specifically designed for NFT and the coding behind, Cadence. From user perspective, three things would come to our mind: low gas fee, fast speed and high security which are taken care of by three pillars of Cadence; from developer perspective, learning the coding is one thing and debugging the code is another big thing that are also handled by three pillars of Cadence. 

I have little to zero to coding and that’s my 2 percent XD

Chapter 2 - Day 1 - Our First Smart Contract
<img width="1106" alt="Deploy Contract" src="https://user-images.githubusercontent.com/71143903/146767646-7ec577fb-e026-47b4-86c6-6420daaf81e7.png">
<img width="1110" alt="Run Script" src="https://user-images.githubusercontent.com/71143903/146767788-9ab206dc-1bce-4b21-b13b-4482f2e36037.png">

Chapter 2 - Day 2 - Transactions and Scripts
1.	A script can only be used to view data.
2.	To access the data in an account.
3.	Only prepare phase can access the data in an account, but execute phase can call functions and change the data on the blockchain. Prepare phase can do that all but it’s better to separate into prepare and execute phrases for clearer logic.
<img width="1108" alt="Number Contract" src="https://user-images.githubusercontent.com/71143903/154001217-71a18fc2-597a-4245-9066-63490faa9eea.png">
<img width="1110" alt="Number Transaction" src="https://user-images.githubusercontent.com/71143903/154001236-72f87f8e-9096-4a70-a849-fdadda480ae5.png">
<img width="1106" alt="Number Script" src="https://user-images.githubusercontent.com/71143903/154001250-672e2bee-69a3-4084-b5b9-06e076c22787.png">


Chapter 2 Day 3 Arrays, Dictionaries, and Optionals
<img width="1091" alt="People Script" src="https://user-images.githubusercontent.com/71143903/154068408-43856a9f-ef37-4f65-ac01-062cbc008616.png">
<img width="1101" alt="SocialMedia Script" src="https://user-images.githubusercontent.com/71143903/154068425-97fc8bef-abbf-4897-970c-aee87c6d699c.png">


3.1 The force-unwrap operator will remove the optional type, like the example below that Int? is an optional(either Int or nil).
var name1: Int? = 123
var unwrappedName1: Int = name1! 

3.2 The force-unwrap operator will abort the program if it encountered nil, like the example below that Int? is equal to nil.
var name2: Int? = nil
var unwrappedName2: Int = name2! 

4.1 The error message means that this script was expected to return a type String (”Three”) but instead it got a type optional String? (“Three” or nil)

4.1 The reason why we’re getting this error is because when we access elements of a dictionary, it returns the value as an optional that is String? (“Three” or nil)

4.3 Adding a force-unwrap operator after return thing[0x03], like this:
pub fun main(): String {
    let thing: {Address: String} = {0x01: “One”, 0x02: “Two”, 0x03: “Three”}
    return thing[0x03]!



