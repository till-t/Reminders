# Best Practices for smart contracts in Solidity
- Monitor & upgrade package.json dependencies
- Use stable solidity versions 
    - 0.5.16 - 0.5.17 
    - 0.6.11 - 0.6.12 
    - 0.7.5 - 0.7.6 
    - 0.8.4
- Avoid floating pragma
- Use Checks-Effects-Interactions Pattern
    - Checks (require(s), modifier(s), ...)
    - Update storage variables
    - Call another contract(s)
- Take warnings seriously
- Keep things small and modular (KISS)
- Always protect withdrawal functions
- Avoid selfdestruct
- Modifiers should't update state
- Use safemath when using solc less than 0.8.0
- Use rentrancy guard
- Send ETH via *call*, avoid *transfer* and *send*
- Avoid pseudo randomess (use chainlink VRF)
- Avoid *tx.origin*, use *msg.sender*
- Divide before multiply
- Use *increaseAllowance* & *decreaseAllowance* instead of *approve*
- Check for address (0x0)
- Always test extreme case of external integrations 
    - Can Uniswap run out of liquidity? test that scenario
- Mainnet Forking --> Fork & Test on the real environment
- Don't make useless optimizations, security is the top priority
- CI/CD (block merging PRs)
- A dex is a decentralized exchange but a centralized price oracle 

