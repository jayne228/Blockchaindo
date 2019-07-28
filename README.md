# Blockchaindo
## Motivation

1)  The method in which Indian elections are conducted require the physical presence of the voter in their registered          constituency. This poses a difficulty to majority of the population like college students who might be studying in a different state which isn’t their registered constituency, voters with physical disabilities and senior citizens. Generally speaking, it is a hassle for the average Indian citizen to stand in queues with a long waiting line in the summer months.
2)	EVM Hacking, tampering of the ballot and other security issues is a serious threat to democracy.
3)	The amount of money and resources spent overall even for a single election is a heavy amount.
4)	An ideal voting system should have transparency, completeness (only the eligible voters can vote and they can vote only once).
5)	Making online voting completely anonymous.

## Idea

We plan to build and deploy an Ethereum based Blockchain for online voting using Azure Blockchain Workbench. The said Blockchain will involve a smart contract that will authenticate the voter's identity. Our idea is to exploit Blockchain technology with cryptographic hash and digital signatures to implement a decentralised online voting system without the requirement of any third party while also maintaining complete anonymity of the voter. This system also provides for users presently residing outside their registered constituencies to excercise their right to vote. In a Blockchain, any new block is added with a reference to the previous block. This creates an immutable chain which prevents tampering and solves the problem of an EVM hacking accusation. Counting and tallying of votes is made faster as the system is based online. Announcement of election results can be done sooner this way.

## Workflow

1) Registration of the candidates and voters: The voting administrator logs in and registers the details of all candidates such as name, mobile number aadhar number, standing party and constituency. The details of all eligible voters such as name, mobile number, aadhar number, registered contituency are also registered.
2) Online voting: The voter logs into the mobile app with aadhar number. An OTP is sent to the mobile number linked to his aadhar card and hence the voter is authenticated with the list of registered voters. The authetication succeeds if the voter is voting for the first time then the details of candidates in registered constituency is displayed. Vote is cast, voter confirms the vote which is further encrypted. This transaction is added as a block to the blockchain.
3) Privacy and Tallying of votes: We intend to provide voter privacy on all ballots by encrypting every vote, homomorphically tallying, and revealing the vote count using Paillier cryptosystem decryption process. This ensures secrecy since votes are homorphically tallied and aren't decrypted at all.

## What is next?
1) In case of online voting, there is a chance that the voter can easily be coerced to cast his vote for a particular candidate. We can solve this issue by providing the voter an option to recast his vote. 
2) Prepare our proposed online voting solution for the post quantum era by implementing suitable hard hashing and encryption algorithms.
3) Polling booths equipped with computers(loaded with proposed application) can be setup in remote rural areas so people who don't have smartphones and those who require technical assistance can also exert their right to vote. 




