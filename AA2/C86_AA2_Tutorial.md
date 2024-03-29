Generate Automatic Index Number
===================


In this activity, you will learn to generate an automatic index number by increasing the index number for each new block.


<img src= "https://media.slid.es/uploads/1525749/images/10651578/pasted-from-clipboard.png" width = "450" height = "250">




Follow the given steps to complete this activity.


* Open the file blockchain.py.


* Create a class variable named “index” and set its value to 0 at start. 


    ` index = 0`


* Remove the index from the list of parameters in the __init__ function. 


    ` def __init__(self, timestamp, transaction, previousHash):`
    	    
* Set the self index using the Block.index method.


    ` self.index = Block.index`   


* Once the index is set for the particular block, increment the index by 1, to use it for the next block.


    ` Block.index+=1 `
    


* Remove the index from arguments of the first block.


    ` block1 = Block(`
    
    `                blockData1["timestamp"], `
    
    `             blockData1["transaction"], `
    
    `             blockData1['previousHash'])` 


* Remove index from arguments of the second block.


    ` block2 = Block(`
    
    `             blockData2["timestamp"], `
    
    `             blockData2["transaction"], `
    
    `             blockData2['previousHash'])`


* Remove index from arguments of the third block.


    ` block3 = Block( `
    
    `           blockData3["timestamp"], `
    
    `             blockData3["transaction"], 
`

    `             blockData3['previousHash'])`  


* Save and run the code to check the output.


