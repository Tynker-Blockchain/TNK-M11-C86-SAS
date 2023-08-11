Create a Block Class
===================


In this activity, you will learn to create the block class and use it to create new blockdata.




<img src= "https://s3-whjr-curriculum-uploads.whjr.online/e75b0a27-ff9c-4b28-b9be-82b0169e1208.gif" width = "536" height = "244">


* Open file blockchain.py.


* Create a new class for the block.


    ` class Block:`   


* Create the constructor using the __init__ function and pass the attributes index, timestamp, transaction, and previousHash.


    ` def __init__(self, index, timestamp, transaction, previousHash):`
`


* Store index, transaction, timeStamp, and previousHash in the respective object variables.

    ` self.index = index   `

    `          self.transaction = transaction`

    `         self.timestamp = timestamp`

    `         self.previousHash = previousHash`

    `  self.currentHash = self.calculateHash()`

* Declare a calculateHash() function to generate and return the hashstring using the block data.


    ` def calculateHash(self):`
`



* Create a variable blockString and store a string made by concatenating index, timestamp, previousHash, and transaction in it.


    ` blockString = str(self.index) + str(self.timestamp) + str(self.previousHash) + str(self.transaction)`
    
    `        return generateHash(blockString)’`
    
    `

* Use the bBlock class and blockData to create a newBlock object.


    ` newBlock = Block(blockData["index"], `

    `    blockData["timestamp"], `

    `                  blockData["transaction"], `
                 `          blockData['previousHash'])`
 
* Print the block data to check the content stored in the newBlock.


    ` print(newBlock.index) `

    ` print(newBlock.timestamp)`

    ` print(newBlock.transaction) `

    ` print(newBlock.previousHash) `

    ` print(newBlock.currentHash)`
` 
* Save and run the code to check the output.
