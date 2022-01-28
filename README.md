# Subnets

The source data is in _data/chains. Each chain has its own file with the filename being the [CAIP-2](https://github.com/ChainAgnostic/CAIPs/blob/master/CAIPs/caip-2.md) representation as name and `.json` ans extension.

## Example

```json
[
    {
        "name": "Avalanche Mainnet",
        "chain": "AVAX",
        "icon": {
            "url": "ipfs://QmRALA5qvQBRwWre8ofuhCbr3wxVmPS3kGetRR9uJqbqqe",
            "width": 1503,
            "height": 1504,
            "format": "png"
        },
        "rpc": [
            "https://api.avax.network/ext/bc/C/rpc"
        ],
        "faucets": [
            "https://free-online-app.com/faucet-for-eth-evm-chains/"
        ],
        "nativeCurrency": {
            "name": "Avalanche",
            "symbol": "AVAX",
            "decimals": 18
        },
        "infoURL": "https://www.avax.network/",
        "shortName": "Avalanche",
        "chainId": 43114,
        "networkId": 43114,
        "slip44": 9000,
        "explorers": [
            {
                "name": "snowtrace",
                "url": "https://snowtrace.io",
                "standard": "EIP3091"
            }
        ]
    },
    {
        "name": "Avalanche Fuji Testnet",
        "chain": "AVAX",
        "icon": {
            "url": "ipfs://QmRALA5qvQBRwWre8ofuhCbr3wxVmPS3kGetRR9uJqbqqe",
            "width": 1503,
            "height": 1504,
            "format": "png"
        },
        "rpc": [
            "https://api.avax-test.network/ext/bc/C/rpc"
        ],
        "faucets": [
            "https://faucet.avax-test.network/"
        ],
        "nativeCurrency": {
            "name": "Avalanche",
            "symbol": "AVAX",
            "decimals": 18
        },
        "infoURL": "https://cchain.explorer.avax-test.network",
        "shortName": "Fuji",
        "chainId": 43113,
        "networkId": 1,
        "explorers": [
            {
                "name": "snowtrace",
                "url": "https://testnet.snowtrace.io",
                "standard": "EIP3091"
            }
        ]
    }
]
```


icon should:
 * the URL must be a IPFS url that is publicly resolveable
 * width and height are optional - but when one is there then the other must be there also
 * format is either "png", "jpg" or "svg"

## Usages

 * [subnetlist.org](https://subnetlist.org)
