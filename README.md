# SPL Token Interest-Bearing Extension Test

This repository contains a test implementation of the interest-bearing token extension for Solana using the Token2022 program.

## Overview

The SPL Token program on Solana has been extended with Token2022, which introduces new features including the ability to create interest-bearing tokens. This repo demonstrates and tests the implementation of such tokens.

## Features

- Create interest-bearing tokens
- Set and adjust interest rates
- Accrue interest over time
- Transfer tokens with interest calculations

## Prerequisites

- Rust 1.68 or later
- Solana CLI tools
- Node.js and npm (for client-side testing)

## Setup

1. Clone the repository:
`git clone https://github.com/yourusername/spl-token.git
cd spl-token`

2. Install dependencies:
`cargo build
npm install`

3. Configure your Solana cluster:
`solana config set --url https://api.devnet.solana.com`

## Usage

1. Deploy the program:
`solana program deploy target/deploy/spl_token.so`

2. Testing:
`cargo test
npm run test`

## Key Components

- `src/lib.rs`: Main program logic
- `src/state.rs`: State management for tokens and accounts
- `src/instruction.rs`: Instruction definitions
- `tests/`: Unit and integration tests

## Disclaimer

This is a test implementation and should not be used in production environments without thorough auditing and testing.

## Resources

- [Solana Documentation](https://docs.solana.com)
- [SPL Token Documentation](https://spl.solana.com/token)
- [Token2022 Program](https://spl.solana.com/token-2022)
