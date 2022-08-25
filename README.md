# Lesson_19
# Primary application file

You will need to make the following updates to the provided Python file for this Challenge, which already contains the basic PyChain ledger structure that you created throughout module 18.


---

## Technologies

The following Technologies were used to develop this program:

Python 
    Version 3.9.7

Terminal
    Version 2.12.5 (444)

Visual Studio Code
    Version: 1.66.2 (Universal)
    Commit: dfd34e8260c270da74b5c2d86d61aee4b6d56977
    Date: 2022-04-11T07:49:20.994Z
    Electron: 17.2.0
    Chromium: 98.0.4758.109
    Node.js: 16.13.0
    V8: 9.8.177.11-electron.0
    OS: Darwin x64 21.4.0
    
---

## General information about analysis.
There are four parts to this Lesson:

### Create a Record Data Class

In the first part you will define a new Python data class named Record. Give this new class a formalized data structure that consists of the sender, receiver, and amount attributes. 

To do so, complete the following steps:

Define a new class named Record.  Next, add the @dataclass decorator immediately before the Record class definition.  Then, add an attribute named sender of type str, receiver of type str, and amount of type float.


### Modify the Existing Block Data Class to Store Record Data

In the second part modify the Existing Block Data Class to Store Record Data, rename the data attribute in your Block class to record, and then set it to use an instance of the new Record class that you created in the previous section. 

To do so, complete the following steps:

In the Block class, rename the data attribute to record and set the data type of the record attribute to Record.


### Add Relevant User Inputs to the Streamlit Interface

Code additional input areas for the user interface of your Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the Block record. To do so, complete the following steps:

Delete the input_data variable from the Streamlit interface.  Add an input area where you can get a value for sender from the user, receiver from the user, and amount from the user.

As part of the Add Block button functionality, update new_block so that Block consists of an attribute named record, which is set equal to a Record that contains the sender, receiver, and amount values. The updated Blockshould also include the attributes for creator_id and prev_hash.


### Test the PyChain Ledger by Storing Records

Test your complete PyChain ledger and user interface by running your Streamlit application and storing some mined blocks in your PyChain ledger. Then test the blockchain validation process by using your PyChain ledger. To do so, complete the following steps:

In the terminal, navigate to the project folder where you've coded the Challenge, and run the Streamlit application by using streamlit run pychain.py.

Enter values for the sender, receiver, and amount, and then click the Add Block button. Do this several times to store several blocks in the ledger.

Verify the block contents and hashes in the Streamlit drop-down menu. Take a screenshot of the Streamlit application page, which should detail a blockchain that consists of multiple blocks. Include the screenshot in the README.md file for your Challenge repository.


![PyChain](Lesson_18_Pychain.png)

![Full_Ledger](PyChain_full_ledger.png)

Test the blockchain validation process by using the web interface. Take a screenshot of the Streamlit application page, which should indicate the validity of the blockchain. Include the screenshot in the README.md file for your Challenge repository.


![Validate](Validate_block_chain.png)






---

## Information about datasets

Create a data class for sender, receiver, and amount:

@dataclass
Class: Record

Block data class to store and record data:

@dataclass
class Block:

Function for hash block:

def hash_block(self)

PyChain data class:

@dataclass
class PyChain:


Function to add block to the block chain:

def add_block(self, candidate_block):


Function for checking validity of block;

def is_valid(self):

---

## Libraries used in analysis

Streamlit

dataclass

typing

datetime

pandas

hashlib

---

## Contributors


**Chris Miskovich**

Contact Information:

Email: cmiskovich@verizon.net

[LinkedIn](https://www.linkedin.com/in/christopher-miskovich-9a61b0234/) 

---

## License

[MIT](/license.txt)
