# Sollidity-first-260207


Search for "Solidity" by Juan Blanco

compile,

forge build
  forge test          # Run tests
  forge fmt           # Format Solidity code
  forge clean         # Clean build artifacts


 1. Write Tests                                                                  
                                                                                
  forge test                                                                      
  Run your tests in test/Counter.t.sol to make sure your contract works.

  2. Run Tests with Verbosity                                                   
                                                                                
  forge test -vvvv
  See detailed output including traces and gas usage.

  3. Deploy Locally (for testing)

  # Start a local blockchain
  anvil

  # In another terminal, deploy
  forge script script/Counter.s.sol --fork-url http://localhost:8545 --broadcast

  4. Deploy to Testnet

  # Deploy to Sepolia testnet (needs RPC URL and private key)
  forge script script/Counter.s.sol --rpc-url <SEPOLIA_RPC_URL> --private-key
  <YOUR_KEY> --broadcast

  5. Other Useful Commands

  forge fmt           # Format your code
  forge snapshot      # Gas snapshots
  forge coverage      # Test coverage report

  Typical flow: Write code → Build → Test → Deploy locally → Deploy to testnet →
  Deploy to mainnet
