# AdSpot Contract

A Solidity smart contract for managing advertisement spots using Superfluid Protocol. The ad spot is taken by the highest bidder who can showcase their NFT, while previous advertisers become members of a distribution pool and receive a share of the new advertiser's flow.

## Features

- Bidding system using Superfluid money streams
- NFT showcase functionality for the highest bidder
- Fair distribution pool for previous advertisers
- Built with Superfluid Protocol for real-time finance

## Prerequisites

- [Foundry](https://book.getfoundry.sh/getting-started/installation)
- [Git](https://git-scm.com/downloads)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/superfluid-finance/ad-auction-example
cd ad-auction-example
```

2. Install dependencies:
```bash
forge install
```

## Testing

Run all tests:
```bash
forge test
```

Run a specific test:
```bash
forge test --match-test testFlowCreation
```

Add verbosity levels for more detailed output:
```bash
forge test -vv  # Shows logs
forge test -vvv # Shows stack traces
```

## Contract Architecture

The AdSpot Contract consists of three main components:

1. **Bidding System**: Uses Superfluid's Constant Flow Agreement (CFA) to manage real-time money streams as bids.
2. **NFT Showcase**: Allows the highest bidder to display their NFT.
3. **Distribution Pool**: Manages the fair distribution of new bidder's streams to previous advertisers.

## Usage

1. Deploy the contract with a supported Super Token
2. Users can start bidding by creating Superfluid streams
3. Highest bidder can set their NFT to showcase
4. Previous bidders automatically receive their share of new streams

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

GPL-3.0

## Acknowledgments

- Built with [Superfluid Protocol](https://www.superfluid.finance/)
- Developed using [Foundry](https://book.getfoundry.sh/)
