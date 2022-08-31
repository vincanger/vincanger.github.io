---
title: "Tippable Q&A Forum on Polygon"
date: 2022-08-31
tags: [ERC20, Solidity, Polygon, Web3, Blockchain]
excerpt: "A Tippable Q&A Forum with a native ERC20 token and swap capabilities"
---
## Description

The [Tippable Q&A Forum on Polygon](https://defi-on-polygon.vercel.app/) is a prototype dApp that allows users to:

- Post questions
- Answer questions
- Upvote answers using a native ERC20 Token
- Swap the native token

The entire state for the app is saved on-chain on Polygon Mumbai and transactions are paid for in Polygon's `MATIC` token. 

The novel feature of this app is that everytime a user upvotes an answer, a "tip" is sent. If the answerer has a native token balance of >= 10, they receive the tip, if not it goes to the address of the Forum's smart contract.

<div max-width="100%">
  <video width="100%" controls>
    <source src="https://i.imgur.com/WCTd97y.mp4" type="video/mp4">
  </video>
</div>


I chose this implementation to incentivize participation in the tipping scheme, without forcing users to have to pay a fee upfront when answering a question. This way, users can freely post questions and answers with minimal transaction fees thanks to Polygon. But, if they want be elligble to receive upvote tips from other uses, they have to acquire and hold the native ERC20 token. This also opens up other possibilities for the Forum to pay out "power users" or "super tippers" with the tips that the contract address receives. 

I also a built a simple swap tool/Automate Market Maker to transfer from a fake `MATIC` contract, to the native `GOFLOW` token.

<img src="https://i.imgur.com/dk4bxJS.gif">

### Live App & Code

The Tippable Q&A Forum on Polygon app is deployed live on Vercel, and on Polygon Mumbai:
- [Live dApp -- https://defi-on-polygon.vercel.app/](https://defi-on-polygon.vercel.app/)
- [Forum contract](https://mumbai.polygonscan.com/address/0xe872B752389AfA71aB213fF2f038404854cD7b80#code)
- [AMM contract](https://mumbai.polygonscan.com/address/0xC0011Aaa2d7b0C4AD65C83518bc0aA16Ac49E9a2#code)

Check out the code on GitHub for both the NextJS app, as well as the Hardhat Project files, Test files, and Solidity contracts >>

 - [https://github.com/vincanger/defi-on-polygon](https://github.com/vincanger/defi-on-polygon)

### More Info

<img src="https://i.imgur.com/agrZ564.gif">

This project was originally intended as a long-form tutorial for Pointer.gg before the company pivoted. I created a number of interactive explainer components to help explain the concepts of ERC20 tokens and Automated Market Makers (above). Here are the drafts:

- [DeFi on Polygon, Part 1](https://www.notion.so/DeFi-on-Polygon-Part-1-f266d0dc3c4c4295bb5ab0d9301537c3)
- [DeFi on Polygon, Part 2](https://www.notion.so/DeFi-on-Polygon-Part-2-2607411576b64395ac166b0be62b03d1)
