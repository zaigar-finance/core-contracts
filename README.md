# Zaigar Finance Farm

This repo is home to the Farming contracts for Zaigar Finance. Liquidity pools are initialized and added as a staking token to the MasterZai contract. This MasterZai contract is also in control of the number of minted $ZAIF per block. As users stake LP and other tokens, the MasterZai distributes them according to the weight of rewards of a specific pool along with an accounts stake in that pool.

https://zaigar.finance. 

## Updates to MasterChef
As MasterZai is fork of Pancake's MasterChef, we want to be transparent about the updates that have been made: https://www.diffchecker.com/


- Documented platform fees: Some other farms take a mining fee on new minted tokens without inform to the community, and also on top of the documented inflation. We wanted to be very transparent on that part and has all fees commented and inside the planned inflation. There's no additional token flooding the market. 
- Migrator Function removed: This function has been used in rug pulls before and as we want to build trust in the community we have decided to remove this. We are not the first, but we agree with the decision. 
- Farm safety checks. When setting allocations for farms, if a pool is added twice it can cause inconsistencies.
- Helper view functions. View functions can only read data from the contract, but not alter anything which means these can not be used for attacks. 
- Only one admin. A recent project was exploited that used multiple forms of admins to control the project. An admin function that was not timelocked was used to make the exploit. We want the timelock to have full control over the contract so there are no surprises

## Updates BNBRewardZai
BNBRewardZai contract is a spin off of Pancake's SmartChef contract and BNBRewardApe, will provide a means to distribute BNB for staking tokens in place of a BEP20 token.

## BEP20RewardZai
BEP20RewardZai contract is similar to the BNBRewardZai contract, but it gives out a BEP20 token as the reward in place of BNB. 

## BEP20RewardZaiV2
BEP20RewardZaiV2 adds two admin functions which allow the pool rewards to be updated allowing the pool to be extended for a longer period of time.


### BSCMAINNET

#### Our Contracts has been audited since day 1
You can find the audit on this official link: 

#### Token Contracts
- ZaifToken: [0x280C3Fc949b1a1D7a470067cA6F7b48b3CB219c5](https://bscscan.com/token/0x280C3Fc949b1a1D7a470067cA6F7b48b3CB219c5)
- FarmToken: [](https://bscscan.com/token/)

#### Farm Contracts
- MasterZai: [](https://bscscan.com/address/)
- Timelock: [](https://bscscan.com/address/)