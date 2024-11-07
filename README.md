# Merkle Tree Proof Generation

This script generates a Merkle Tree and provides a proof for an Ethereum address. It leverages the `merkletreejs` library and `keccak256` hashing to process addresses listed in `tokens.json`.

## Files

- **index.js**: Main script to create a Merkle Tree from Ethereum addresses and output the root and proof.
- **tokens.json**: A JSON file containing an array of Ethereum addresses to be included in the Merkle Tree.

## Usage

### Prerequisites

- Node.js installed on your machine
- `merkletreejs` and `keccak256` libraries (install them using npm if not present)

```bash
npm install merkletreejs keccak256
```

### Running the Script

Execute the script to generate a Merkle Tree root and proof:

```bash
node index.js
```

### Output

The script will log:

- **Root**: The Merkle Root generated from the provided addresses.
- **Proof**: A proof for an empty leaf.

## Example Structure of tokens.json

```json
[
  {
    "address": "0xc0ffee254729296a45a3885639AC7E10F9d54979"
  },
  {
    "address": "0x999999cf1046e68e36E1aA2E0E07105eDDD1f08E"
  }
]
```

---
