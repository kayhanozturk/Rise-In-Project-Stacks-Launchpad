# Simple Launchpad on Stacks

 ## Project Description
Simple Launchpad on Stacks is a blockchain-based application for crowdfunding on the STX blockchain. When new campaign is created, fundraiser sets a goal in STX and a duration in blocks. In order to finish succesfull campaign, the campaign need to be fully invested or exceeding the funding goal before the target block-height is reached. After succesfull campaign, the fundraiser can then collect the funds. Investor can request a refund at any point while the campaign still active.This ensures that the investors stay in control of their STX until the funding goal is reached. If the goal of the campaign is not met after it reached setted block-height, the investors can request a refund.

## Repository URL 
https://github.com/kayhanozturk/Rise-In-Project-Stacks-Launchpad


## Technologies Used
 - Stacks Blockchain
 - Clarity Smart Contracts
 - Stacks.js libraries

## Key Features
- Users can start campaigns and add a name, short description, a link, funding goal, and duration.
- The campaign owner can update the short description and link.
- The campaign owner creates tiers, each having a name, short description, and cost.
- Investors choose one or more tiers to invest. They are required to pay at least the tier cost in order for the investment to be successful.
- Investors can take their investment out as long as the campaign has not reached its funding goal.
- The campaign owner can collect the funds once the campaign is successfully funded.

## Getting Started
### Prerequisites
- Node.js (v14 or later)
- npm or yarn
- Stacks wallet (Hiro Wallet, Xverse, Leather Wallet)


### Read-only functions
 - `get-campaign-id-nonce`
    - Returns the current campaign ID nonce of the smart contract.
 - `get-total-campaigns-funded` 
    - Returns the total number of campaigns that have been funded.
 - `get-total-investments`
    - Returns the total amount of investments. This number may go up and down a bit depending on refunds.
 - `get-total-investment-value`
    - Returns the total amount of STX invested. 
- `get-campaign-status(campaign-id uint)`
    - Returns the current campaign status (whether the goal was reached, the block height it was reached if successful, and whether the campaign owner has collected the funds).
 - `get-is-active-campaign(campaign-id uint)`
    - Returns whether the campaign is currently active (not expired and the funding goal has not yet been reached).

### Public functions
- `create-campaign (name buff, description buff, link buff, goal uint, duration uint)`
    - Creates a new campaign with the provided information. Returns the campaign ID if successful.
- `update-campaign-information(campaign-id uint, description buff, link buff)`
    - Updates campaign information for the specified campaign. Only the owner can do this. Returns u1 if successful.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Contact/Support
For support, please open an issue in the GitHub repository.

## Acknowledgments
Thanks to the Stacks ecosystem for providing the tools and resources to build this project.
