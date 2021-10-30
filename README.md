# Challenge_18

***

**Background**

I am a fintech engineer who’s working at one of the five largest banks in the world. I was recently promoted to act as the lead developer on their decentralized finance team. My task is to build a blockchain-based ledger system, complete with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions and to verify the integrity of the data in the ledger.

***

**What I Created**

I made the following updates to the provided Python file for this Challenge, which already contains the basic PyChain ledger structure that I created throughout the module:

1. I created a new data class named Record. This class will serve as the blueprint for the financial transaction records that the blocks of the ledger will store.

2. I changed the existing Block data class by replacing the generic data attribute with a record attribute that’s of type Record.

3. I created additional user input areas in the Streamlit application. These input areas collect the relevant information for each financial record that the user stores in the PyChain ledger.

4. Finally I tested my complete PyChain ledger.

5. I then uploaded the Python file for this Challenge to your GitHub repository.

***

**Instructions**

I opened the pychain.py file that my Challenge files include. I  used this file to complete the steps for this Challenge. 
 The steps for this Challenge are divided into the following sections:

1.Create a Record Data Class

2. Modify the Existing Block Data Class to Store Record Data

3. Add Relevant User Inputs to the Streamlit Interface

4. Test the PyChain Ledger by Storing Records

***

**Step 1: Create a Record Data Class**

I defined a new class named Record.

I then added the @dataclass decorator immediately before the Record class definition. I then added the following things:

I add an attribute named sender of type str.

I add an attribute named receiver of type str.

I add an attribute named amount of type float.

***

**Step 2: Modify the Existing Block Data Class to Store Record Data**

In the Block class, I renamed the data attribute to record.

I then set the data type of the record attribute to Record.

***

**Step 3: Add Relevant User Inputs to the Streamlit Interface**

I deleted the input_data variable from the Streamlit interface.

I then Added an input area where I can get a value for sender from the user.

I then Added an input area where I can get a value for receiver from the user.

I then Add an input area where I could get a value for amount from the user.

As part of the Add Block button functionality, I updated new_block so that Block consists of an attribute named record, which is set equal to a Record that contains the sender, receiver, and amount values. The updated Blockshould also include the attributes for creator_id and prev_hash.

***

**Step 4: Test the PyChain Ledger by Storing Records**

In the terminal, I navigated to the project folder where you've coded the Challenge.

In the terminal, I then ran the Streamlit application by using streamlit run pychain.py.

I entered values for the sender, receiver, and amount, and then I clicked the Add Block button. 

I verified the block contents and hashes in the Streamlit drop-down menu. I then took a screenshot of the Streamlit application page, 

I tested the blockchain validation process by using the web interface. I created a screenshot of the Streamlit application page, which indicated the validity of the blockchain. I then included the screenshot in the README.md file for my Challenge repository.


<img width="755" alt="Screen Shot 2021-10-30 at 10 29 44 AM" src="https://user-images.githubusercontent.com/85910138/139543295-69ba77bf-5dda-4bba-a70a-66391c840074.png">
