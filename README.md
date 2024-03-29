# MinaFolio

Investment portfolio DEFI
Sometimes you just want to invest in crypto without using dex, which are complicated to use and can lead you to make mistakes.
Our product aims to create investment portfolios simply by choosing which crypto you want to invest in and what percentage of your portfolio it should complete.

You can also copy existing portfolios with a single click, to replicate the performance of the platform's top traders.

We can even offer anonymized investments.

Proposal Overview / Summary
Describe the problem that your zkApp is solving
The aim of our platform is to simplify investment in a crypto portfolio, and to offer the simplest possible interface so that any novice can invest in just a few clicks.
Describe your proposed solution
Once the user has created a wallet or replicated an existing one, our platform will exchange all the tokens needed on the dex platforms currently deployed for the user's Mina.
Architecture
Go-to-market strategy
Share your go-to-market strategy, which includes:
The MVP can be created in 3 months, and will focus on the platform's ease of use, so that users can easily create their own portfolios.
The platform's ease of use and sleek interface must be attractive to the user in order to achieve a good conversion rate.
The aim is to attract users via different communication channels such as telegram/discord/twitter, which are the main crypto communication channels.
Partnerships can be formed with various dex, since our platform will use them, and it will be a win-win partnership.
A reward may be distributed to the creators of the replicated portfolios, based on a tax on that portfolio.
An airdrop could also be distributed to different users on a model close to that of blur.
What does success look like in terms of user adoption in 6 months from now? Please be as specific as possible.
A dozen different portfolios would have to be created and a hundred different investors would have to use our platform.

The aim would be for these users to become ambassadors for our platform.

Commercial vision
Share your thoughts on generating revenue over a longer time horizon (greater than 6 months)
The main method of financing will be a tax on the creation of a portfolio, a bit like the dex tax on swaps.

A governance token can also be issued and offered to different users to give them a choice about future decisions.

What is your long-term vision for this project if your proposal is funded? What is your dream scenario for how this project could evolve?
The creation of portfolios that evolve according to market conditions, or that reflect the investments of one or more users.

The bridge between Mina and ethereum will also enable wallets on Ethereum and its L2s to be created anonymously and directly from Mina.

The possibilities are endless.

Budget and milestones
Standard Budget Proposal
(Required) The standard scope is the minimum budget, scope, and milestones which can be delivered in the proposed three month development sprint.

Standard Budget in MINA
57000

Standard Scope
UI/UX 10000 MINA 

The interface will be the key element in attracting the user and making it as easy as possible to use, thus improving conversion. it should be created by one or more professional graphic designers.

Website Frontend/Backend 25000 MINA

The website will be what the user sees and uses on a daily basis, it will have to integrate ui/ux perfectly and be quick to use, it will be made up of several pages including a landing page to present our services, different pages to manage the portfolios and follow their evolution in terms of price, backend service to store information and get real price data.
 

SmartContract 20000 MINA

Smartcontracts are at the heart of the application, and will enable you to create portfolios and interact with other smartcontracts to swap with tokens.

Hosting 2000 MINA
The site will have to be fast to load and the smartcontracts will have to be cached on cloud solutions to be available to users as quickly as possible, which requires high-performance hosting.

Standard Scope Milestones
Midpoint milestone
The user will be able to create their first portfolio on a fairly simple website, invest in it and withdraw their money.

Final milestone
The website will be finalized, it will allow us to see the different portfolios, replicate them, create our own, see their course in real time.
Advanced Budget Proposal
(Optional) The advanced scope section allow you to propose a larger scope and effort for the same development timeline. The advanced scope will replace the standard scope if the funding target is met. As a replacement to the standard scope, you would still document the original budget, scope and milestones AND add the additional budget, scope, and milestones to present a TOTAL proposal which could be delivered in the proposed three month development sprint.

Propose Advanced Scope?
Yes

Advanced Budget in MINA
82000

Advanced Scope
Incorporate privacy, with the help of protokit, we'll be able to allow users to invest anonymously in our various products, allowing them to withdraw their winnings progressively from different accounts in order to offend their actions as much as possible.

Website 5000 MINA
The website must take these different types of investment into account

Smartcontract 20000 MINA
This will be the most complicated part and will require a lot of testing to make sure we respect our users' privacy and that they are as secure as possible. 

Advanced Scope Milestones
Midpoint milestone
Users can create their first portfolio on a simple website, invest in it and withdraw their money. They can also invest anonymously using different accounts with no direct link.

Final milestone
The website will be finalized, it will allow us to see the different portfolios, replicate them, create our own, see their course in real time. Implement anonymous portfolio money creation and withdrawal
Risks & Dependencies
What risks or dependencies do you foresee with building and launching this application?
This application requires the presence of other assets on Mina to invest in it, a lack of choice in terms of assets could make this application unattractive at first
Team Info
This section provides details about the proposal team.

Proposer Github
https://github.com/youtpout
Proposer Experience
I have been a developer for 13 years, for 3 years in cryptocurrency, I have a first experience on EVM compatible blockchains and for a few months I have integrated the mina navigator program and created ZkApp, I even created a library allowing to reproduce the signatures and their verification of mina signing in C#.
I will act as tech lead on this project, I will work mainly on the smartcontract part, my long experience as a developer has allowed me to meet trusted people who can help me in the creation of this project
Cohort 2 Participation
Please note that if you were funded as part of Cohort 2, your proposed milestones for Cohort 3 must be a progression from the proposed milestones for Cohort 2. See ‘Builder FAQ’ for more details.

Cohort 2 Participation
No

Team Members, Allow Team Application, and Attach Files
Team Members: This section is used to add team members. They must have an active zkIgnite account.

Allow Team Application: This section is used to enable zkIgnite community members to submit a request to join this proposal team. If a team is looking for additional team members, then checking the "allow team member" box will enable the proposer to accept team applications. In the text field, the proposer should provide some information to potential team members regarding the skills and experience they are seeking. For example: experienced programmer who knows Python or Javascript; project manager; frontend UX designer.

Attach Files: File attachments should be used to present diagrams, presentations, and other supporting documents. An image can be attached as a teaser image for the proposal in the summary view. Attachments do not replace the submission form and should only be used to support and enhance the submission.

Provide technical detail for your zkApp design
We'll create a smartcontract for each investment contract, with the list of assets stored as a mekle root in the corresponding smartcontract.

When a user invests in a portfolio, the portfolio will exchange the various assets for the user's mina, using the existing dex.
The goal is to use Luminadex :
https://luminadex.com/
Kaupang can be a good alternative too :
https://sandbox.kaupang.xyz/
If no dex is deployed at the time of development, we will use the example of MINA.

https://github.com/o1-labs/o1js/blob/main/src/examples/zkapps/dex/dex.ts


If a user wants to make investments anonymously, a deposit smartcontract will be created, from another account thanks to his proof of deposit he will be able to choose in which portfolio to invest and in which proportions.
This part will be based on protokit and the Zkeeper example.
https://github.com/0x471/zkeeper/blob/main/packages/chain/src/mixer.ts