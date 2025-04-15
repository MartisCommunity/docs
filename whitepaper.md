---
icon: question
label: Whitepaper
order: 80
---
# Martiscoin-the universal currency on Mars

!!!
This white paper is a work in progress.
!!!

## Introduction and Project goals

Martis comes from Latin, meaning "Mars".

[Martiscoin](https://martiscoin.net/) is a :sparkles: Groundbreaking Layer 1 :sparkles: [!badge The first decentralized mining pool blockchain] Is inspired by Musk’s Mars immigration plan and Musk’s 2021 tweets on X ([Here](https://x.com/elonmusk/status/1361709250561642498)). The goal is to use innovative, cutting-edge algorithms to enable true decentralized finance in a future on Mars.

Martiscoin have developed a brand new mining algorithm (XmarsHash) to combat ASCI miners and Mining pools, a dynamic X13+SHA512 algorithm (supports CPU/GPU).

[Martiscoin]
> “The centralization is essentially an economic distribution problem,\
> Work will definitely pay off.” *- mars-dev*

The centralization problem is essentially a wealth distribution problem! Martiscoin builds a new distribution mechanism (interval reward distribution mechanism) based on the underlying economic model to solve the centralization problem. Centralization cannot bring greater economic benefits. Therefore, the willingness to centralization will be greatly reduced, thereby ultimately achieving the goal of decentralization.


## Satoshi’s vision

Originally, Satoshi Nakamoto had an idealized hope for mining being a democratized way of establishing consensus. This can be seen for example in his famous whitepaper [2] where it says:

'Proof-of-work is essentially one-CPU-one-vote.'

He knew that with the advent of GPU mining, many CPU miners would be kicked out of the network, which would be against his vision of fair, equal and decentralized mining.

We all know that his hopes have not been fulfilled, today Bitcoin is mined on specialized expensive hardware and only those with access to this hardware can participate in mining. After all, Satoshi was not able to solve the issue of centralized mining.

We know that there are many teams working on solving the problem of centralized mining. They tried many methods, but always came up with software and hardware algorithms to solve the centralization problem. In fact, they all ignored an important point: centralization is essentially a question of interest distribution,This is an economic problem that must be solved from a distributional perspective.

Today, Martiscoin integrates a decentralized mining pool into the blockchain for the first time. Through two workload proofs, the problem of centralized mining was perfectly solved and Satoshi Nakamoto’s wish was truly realized.

## Technical Details

Martiscoin core base on Blockcore, is a platform to build Layer 1 consensus networks based on the Bitcoin protocol.We reconstructed the POW algorithm and block allocation consensus above.

#### POW Algorithm (XmarsHash)

!!!
The new algorithm is called "XmarsHash",a dynamic X13+SHA512 algorithm (supports CPU/GPU).
!!!

The main points of the algorithm are:

- CPU and GPU friendly: Both devices should be able to mine efficiently as they are the most common parts and everyone have access to them
- Randomness: The algorithm used for the next hash calculation is automatically matched based on the last calculated hash value.
- ASIC-resistant: ASIC shouldn't provide too much advantage over CPUs and GPUs in efficiency
- Useful POW: Using two layers of proof of work, it is guaranteed that as long as the node participate in the calculation, will be rewarded.

![XmarsHash algorithm process](/static/pow.png)

##### X13 Algorithm

Algorithm   | Description
:---   |
Blake512 |
BlueMidnightWish512 |
Groestl512 |
Skein512 |
JH512 |
Keccak512 |
Luffa512 |
CubeHash512 |
SHAvite3_512 |
SIMD512 |
Echo512 |
Hamsi512 |
Fugue512 |

#### Block Reward Principle (The core of decentralization)

!!!
About the twice of proof of work
!!!

##### Base proof of work
- Complete the basic workload proof and participate in 90% of the block reward distribution.
- The difficulty of the basic work is a fixed hash value and does not adjust as the network computing power increases.

##### Block found proof of work
- Successfully find the block receive 10% of the block reward.

![The twice of proof of work process](/static/twice.png)

[Note]
> During the proof-of-work process, once the basic hash requirement is reached, the node will immediately send the currently calculated nonce value to the memory pool (only once per block), and then continue to complete subsequent proof-of-work until Find the block. When a block is discovered, 90% of the reward will be distributed equally to all miners in the mempool, and the remaining 10% will be distributed to the block discoverer. If there is no data in the mempool, the block discoverer will receive all block rewards.

## Emission Scheme

!!!
Martiscoin has a fixed maximum supply of 21M MSC.Mining block starts at around 2 MSC.The reward is automatically halved after every 5,000,000 blocks mined - this happens approximately every 5 years based on the 30 second interval it typically takes to mine a block.
!!!

Every day approximately 60/30 * 60 * 24 * 2 = 2880 blocks and 5760 MSC

#### The emission for the next 10 years is summarized in the following table

Year   | Supply | Mined
:---   | :---: | ---:
2025 Q1 | 	2,102,400	| 10.01%
2026 Q1	| 4,204,800	| 20.02%
2027 Q1 | 	6,307,200	| 30.03%
2028 Q1	| 8,409,600	| 40.04%
2029 Q1 | 	10,512,000| 	50.05%
2030 Q1	| 11,563,200	| 55.06%
2031 Q1	| 12,614,400	| 60.06%
2032 Q1	| 13,665,600	| 65.07%
2033 Q1	| 14,716,800	| 70.08%
2034 Q1	| 15,768,000| 	75.08%
2035 Q1	| 16,293,600	| 77.58%
2037 Q1	| 16,819,200	| 80.09%
_	| _	| _
2045 Q1	| 19,841,400| 	94.46%
_	| _	| _
2059 Q1	| 20,859,750	| 99.33%

![Emission Scheme 1](/static/supply.png)

![Emission Scheme 2](/static/supply2.png)

> The official launch date is Q1 2025

## I want to work with the team. How can I apply?

Currently, we don't have any open positions. We will announce job openings and create a dedicated page in the documentation when they become available. However, if you want to stand out and improve your chances, you can contribute by submitting valuable PRs, actively engage with the community and developers, and more. We always appreciate proactive involvement and contributions. This is an initiative that carries significant weight if you want to work more closely with the team.
