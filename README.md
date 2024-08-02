# Token on Solana

+ Install **Rust**: https://rustup.rs/
```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh```

+ Install **Solana Tool Suite**: https://docs.solana.com/cli/install-solana-cli-tools
```sh -c "$(curl -sSfL https://release.solana.com/v1.18.18/install)"```

+ confirm installation: ```cargo --version``` and ```solana --version```

+ Install **SPL-CLI**: ```cargo install spl-token-cli```

+ generate new wallet: ```solana-keygen new --no-outfile```

+ set devnet network configuration: ```solana config set --url https://api.devnet.solana.com```

+ check network configuration: ```solana config get```

+ get free SOL: ```solana airdrop 1```

+ check balance: ```solana balance```

+ create and deploy token: ```spl-token create-token```

+ COPY THE TOKEN ADDRESS

+ create an account to store token ```spl-token create-account <token-address>```

+ mint token to the created account: ```spl-token mint <token-address> <token-amount>```