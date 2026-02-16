# Disperse PC

Batch send PC tokens on Pentagon Chain.

## Live

**https://disperse.pentagon.games**

## Features

- Connect wallet (auto-adds Pentagon Chain if needed)
- Whitespace delimited input: `address amount` per line
- Real-time parsing and error checking
- Shows recipient count + total before sending
- Uses `dispersePCExactDecimal` for decimal precision

## Format

```
0x1234...abcd 10.5
0x5678...efgh 25
0xabcd...1234 7.25
```

One address per line, space or tab separated.

## Contract

**Disperse Contract:** [`0x210a72A04fAF219e3c0EEf34c1A8f85E87633de5`](https://explorer.pentagon.games/address/0x210a72A04fAF219e3c0EEf34c1A8f85E87633de5)

### Functions

| Function | Description | Payable |
|----------|-------------|---------|
| `dispersePCExactDecimal(address[], uint256[])` | Send PC with exact wei values | ✅ Yes |
| `dispersePCx18Decimal(address[], uint256[])` | Send PC with whole numbers (auto × 10¹⁸) | ✅ Yes |
| `disperseWPCExactDecimal(address[], uint256[])` | Send WPC (wrapped) exact values | No |
| `disperseWPCx18Decimal(address[], uint256[])` | Send WPC with whole numbers (auto × 10¹⁸) | No |
| `disperseTokenExactDecimal(IERC20, address[], uint256[])` | Send any ERC20 exact values | No |
| `disperseTokenx18Decimal(IERC20, address[], uint256[])` | Send any ERC20 with whole numbers | No |

## Links

- [Pentagon Games](https://pentagon.games)
- [Pentagon Chain Explorer](https://explorer.pentagon.games)
- [Twitter](https://x.com/PentagonGamesXP)
- [Discord](https://discord.gg/pentagongamesxp)
- [Telegram](https://t.me/pentagongames)

## License

MIT
