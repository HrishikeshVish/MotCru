# MotCru
CodeFundoo 2019

codefundoo++ 2019 contest GitHub repo

What it's all About - The plan here is to design a way of improving the security of elections and making them more transparent. Blockchain shall be used to implement the solution

How does it Work? We are not primarily concerned if a person is being coerced. It's easier to ensure that a person votes only once by introducing some form of biometric tool. There's little use of Blockchain unless you store the biometric details on a blockchain. Again, it is one solution that we might be able to implement.

Our main concern is to make the machines foolproof. As in, they should not, for any reason, be tampered with. There's also a scenario where the votes are not recorded or rejected for some reason. While it's highly unlikely that it happens all the time, there's a 0.89% - 1.23% chance that the machine rejects a vote. This percentage has been determined using the statistics published by the government of India.

This can be reduced, if the machine uses a combination of biometric data and storage of records that contain the votes that each candidate has recieved on block chain.

Whenever a candidate recieves a vote, which is determined by the press of the button, the tally corresponding to that particular candidate is incremented by 1. We use time stamps to periodically append the modified record to the block chain. 

We will need to create a key map associating each key with the particular candidate. As with the case of any standard keyboard, we use a function that detects key press to update the tally of the candidate with whom the key is mapped. 

The records shall be accessible only by the authorized members of the election commission, who can access it but not modify it. They shall have read permission. 

To ensure that the entire set up is foolproof, we will need a dedicated Operating Systems, not unlike the ones they have implemented in medical instruments. The operating system shall have no user interface. It shall, for all purposes be inaccessible, save for the tech support. On startup, the tally application, which will be the only application on the OS, shall be invoked. 
The block chain is accessed to see if there are any records present. The most recently accessed record is retrieved and the tally shall commence. 

In case there's a software failure or the internet connection is temporarily lost, the most recently created record present on the chain is retrieved. The count is compared with the manual tally recorded by the machine. Any discrepancy is fixed by replacing the data on the record with the one manually stored in the machine.  
