Prepare the Data for the Block
==============================


In this activity, you will learn to prepare the data for the block and print it.


<img src= "https://s3-whjr-curriculum-uploads.whjr.online/464746bd-acd6-4f6c-98a1-c6a6b84ffa4e.gif" width = "440" height = "248">

Follow the given steps to complete this activity.

* Open file app.py.


* Import the time module from the time file.


    `from time import time`


* Rename the encryptedData to the transaction, which contains sender, receiver, and amount information.


    ` transaction = { `

    `                "sender": sender, `

    `                "receiver": receiver, `

    `                "amount": amount } `

* Create an object blockData and add the transaction data and other data such as an index, timestamp, and hash.


    ` blockData = {`

    `                'index': 1,` 


    `                'timestamp': time(),`

    `                'transaction': transaction,`

    `                'previousHash': "No Previous Hash Present. Since this is the first block." }`
       
* Display the data inside the blockData to see the values in it.


	`print(blockData)`


* Pass the blockData instead of encryptedData to the HTML file to display it on the web page.


	`return render_template('index.html', originalData = originalData, blockData = blockData)`


* Save and run the code to check the output.
