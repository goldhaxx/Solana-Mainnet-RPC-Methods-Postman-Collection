# Solana Mainnet RPC Methods Postman Collection

## Overview
The Solana RPC method Postman collection enables you to rapidly test Solana RPC methods. It utilizes the Solana Foundation's public mainnet beta RPC endpoint. When executing the methods available in this collection, they are sent to the Solana Foundation's provided public mainnet beta RPC endpoint. If the proper information is submitted within these methods, the RPC node will reply accordingly.

## How the Collection Works
- Each request in the collection corresponds to a specific RPC method available on the Solana network.
- The collection is designed to allow users to interact with the Solana blockchain by sending JSON-RPC requests.
- The responses from the RPC methods are processed and can be logged or stored in Postman variables for further use.

## Variables
The collection uses several variables that can be modified to customize the requests:

- **`_solRpcEndpoint`**: The URL of the Solana RPC endpoint. Default is `https://api.mainnet-beta.solana.com`.
- **`solAccountPubkey`**: The public key of the Solana account you want to interact with. Default is `7cVfgArCheMR6Cs4t6vz5rfnqd56vZq4ndaBrY5xkxXy`.
- **`solWalletBalanceLamports`**: Stores the wallet balance in lamports.
- **`solWalletBalance`**: Stores the wallet balance in SOL.
- **`sol_LAMPORTS_PER_SOL`**: Conversion rate from lamports to SOL. Default is `1000000000`.
- **`solVoteAccount`**: The public key of the vote account. Default is `FQwewNXahV7MiZcLpY6p1xhUs2acVGQ3U5Xxc7FzV571`.
- **`solCurrentBlockHeight`**: Stores the current block height.
- **`solCurrentSlot`**: Stores the current slot.
- **`solTokenProgram`**: The program ID for the token program. Default is `TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA`.

## Useful Information
- **Rate Limiting**: The default endpoint is rate-limited, and some methods may be blacklisted due to abuse potential. You can update the `_solRpcEndpoint` variable to use another provider's URL if needed.
- **Pre-request Scripts**: Some requests include pre-request scripts that fetch necessary data (like the current block height) before executing the main request.
- **Testing and Logging**: Each request can log responses and set environment or collection variables for further use, making it easier to manage data across multiple requests.

## Contact
For any questions or issues, feel free to reach out: [Contact](https://x.com/goldhaxx)

## Additional Resources
- [What is an RPC?](https://chatgpt.com/share/c9c14141-665c-4aee-8866-ca8ed8483b4c)
- [Solana JSON API Reference](https://docs.solana.com/developing/clients/jsonrpc-api#json-rpc-api-reference)
- [Clusters & Endpoints](https://solana.com/docs/core/clusters)
