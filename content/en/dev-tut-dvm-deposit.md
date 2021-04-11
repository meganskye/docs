---
id: dev-tut-dvm-deposit
title: Deposit to a DVM address
sidebar_label: Deposit to a DVM address
---

> All tutorials are only used in Pangolin testnet.

## Pangolin Testnet

The Pangolin TestNet is a network for smart contract developers maintained by the Darwinia team with native token `PRING.` This network integrates the Darwinia Virtual Machine (DVM) which supports Ethereum smart contracts on the current Darwinia network. On Pangolin, you can use the most common Ethereum tools such as Metamask, Remix, etc. and unlike Crab Network cRING tokens, Pangolin tokens are freely issued to those who apply.

Developers who would like to deploy smart contracts and test their functionality for use on Darwinia network can apply for free pRING tokens in [Darwinia Element](https://app.element.io/?pk_vid=6961ca0f7c45f8bf16052310122d2437#/room/#darwinia:matrix.org).

## Add Pangolin to MetaMask 

We first need to query the balance of EVM account, so will need to add a new network in Metamask.

![add testnet](assets/wiki-tut-dvm-recharge-01.png)

![set testnet](assets/wiki-tut-dvm-recharge-02.png)

Setting Configuration:

- Network Name：`Pangolin`
- RPC URL: `https://pangolin-rpc.darwinia.network`
- Chain ID： `43`
- Currency Symbol： `PRING`

Click Save, and Pangolin network will be added; and then you will be ready to transfer tokens or deploy smart contracts using Metamask.

## Add Pangolin to Apps

Apps is a collection of toolkits provided by Darwinia Team. You can switch to Pangolin network as follows, click https://apps.darwinia.network/,
add custom ternal configuration ws://t1.hkg.itering.com:9944/, save and reload again.

![support apps](assets/wiki-tut-dvm-recharge-03.png)

> Note: if it prompts websocket unsecurity warn, please change chrome safe configuration to allow access to unsafe content.

## Deposit a EVM address

### Preparations

- An EVM address (Use Metamask to generate an account)
- A Darwinia address (This should have a proper balance, apply in the Darwinia Element channel)

### Deposit

1. Generate EVM address from Darwinia address

`Apps` - `ToolBox` - `DVM address`, enter the EVM address, the corresponding Darwinia address will be generated, which represent this EVM address to send or receive PRING.


![create substrate address](assets/wiki-tut-dvm-recharge-04.png)
The corresponding Darwinia address of `0xAa01a1bEF0557fa9625581a293F3AA7770192632` is `5ELRpquT7C3mWtjerXnTxDmKnvVxJjCCstXcN8yG34o4365H`.


2. Transfer use Apps

Transfer using [Apps](https://apps.darwinia.network/#/account), the target address is `5ELRpquT7C3mWtjerXnTxDmKnvVxJjCCstXcN8yG34o4365H`.

![transfer pring](assets/wiki-tut-dvm-recharge-05.png)

`Make Transfer` and wait until the extrinsic been finalized in block.


3. Comfirm balance in MetaMask

![confirm balance in mataMask](assets/wiki-tut-dvm-recharge-06.png)

The balance of EVM address `0xAa01a1bEF0557fa9625581a293F3AA7770192632` is 100, a successfully recharge completely.
