# Simple Launchpad on Stacks

 ## Project Description
Simple Launchpad on Stacks is a blockchain-based application for crowdfunding on the STX blockchain. When new campaign is created, fundraiser sets a goal in STX and a duration in blocks. In order to finish succesfull campaign, the campaign need to be fully invested or exceeding the funding goal before the target block-height is reached. After succesfull campaign, the fundraiser can then collect the funds. Investor can request a refund at any point while the campaign still active.This ensures that the investors stay in control of their STX until the funding goal is reached. If the goal of the campaign is not met after it reached setted block-height, the investors can request a refund.

## Repository URL 
https://github.com/kayhanozturk/Rise-In-Project-Stacks-Launchpad


## Technologies Used
 - Stacks Blockchain
 - Clarity Smart Contracts
 - Next.js/React
 - Stacks.js libraries
 - Tailwind CSS

## Key Features
- Users can start campaigns and add a name, short description, a link, funding goal, and duration.
- The campaign owner can update the short description and link.
- The campaign owner creates tiers, each having a name, short description, and cost.
- Investors choose one or more tiers to invest. They are required to pay at least the tier cost in order for the investment to be successful.
- Investors can take their investment out as long as the campaign has not reached its funding goal.
- The campaign owner can collect the funds once the campaign is successfully funded.

## Getting Started
* Prerequisites
* Node.js (v14 or later)
* npm or yarn
* Stacks wallet (Hiro Wallet, Xverse)



Parameters:
amount: The amount of STX to donate.
sender: The address of the sender.


Returns: A list of all donations.
get-donation: Retrieves a specific donation by ID.

Parameters:

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Contact/Support
For support, please open an issue in the GitHub repository.

## Acknowledgments
Thanks to the Stacks ecosystem for providing the tools and resources to build this project.
