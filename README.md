# ldex-configs
Repo which holds configs for existing LDEX markets.

These configs are intended to be used to allow community members to run DEX nodes in `passiveMode` but they can be adapted for use by active LDEX members by setting `passiveMode` to `true` and by filling out missing fields such as `sharedPassphrase`, `passphrase`, `memberAddress`...

Passive mode allows individuals to run their own DEX nodes for a specific market without having to be a member of that DEX federation.
Such DEX nodes can allow a user to independently monitor cross-chain trades and to verify the correctness of trades executed by a DEX federation - They can also be used to replay any segment of the on-chain trading history in a controlled environment.

Config objects for each module should be copied to the LDEM node operator's own `config.json` file (and placed inside their own `modules` object).
It's critical that the market-specific properties of a `lisk_dex_...` module match exactly with those of other nodes which participate in that same DEX market in order to achieve consensus.
