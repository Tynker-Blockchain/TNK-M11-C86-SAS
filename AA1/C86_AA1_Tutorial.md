
Add New Blocks with Transactions  
================================


In this activity, you will learn to create new blocks with transactions and show multiple blocks together on the console.


<img src= "https://media.slid.es/uploads/1525749/images/10651567/pasted-from-clipboard.png" width = "450" height = "250">




Follow the given steps to complete this activity.


* Open file blockchain.py.


* Create an empty list named chain.


     `chain = []`
    	    
* Create the new block as block2 using blockData2.


    ` block2 = Block(blockData2["index"], `

    `                 blockData2["timestamp"], `

    `                 blockData2["transaction"], `

    `                 blockData2['previousHash'])`   


*  Similarly, create one more block as block3 using blockData3.


    ` block3 = Block(blockData3["index"], ` 

    `                 blockData3["timestamp"], `

    `                 blockData3["transaction"], `

    `                 blockData3['previousHash'])` 


* Append all the blocks, block1, block2, and block3 to the chain.


     `chain.append(block1)
	chain.append(block2)
chain.append(block3)`


* Run the for loop to display the block details of each block in the chain using the block.showBlockdetails() method.


     `for block in chain:
      block.showBlockDetails()`


* Save and run the code to check the output.