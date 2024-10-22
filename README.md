# DOD Miners

## Configuration
in `.env.example`
1. `WIF=$WIF_private_key`, you can export from Wizz Wallet/DOD Wallet
2. `CYCLES_PRICE=$target_cycle_price`
    eg. `CYCLES_PRICE=2`
3. rename `.env.example` to `.env`


## Build
install rustup

https://www.rust-lang.org/tools/install

```bash
cargo build --release
```


## Run

### Bash run
```bash
./target/release/dod_miner miner --threads=$cpu_threads
```

eg.
```bash
./target/release/dod_miner miner --threads=12
```