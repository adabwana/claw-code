## Inject .env
```bash
set -a
source .env
set +a
```

## Build 
```bash
cd rust
cargo build --release -p claw-cli
```

## Run CLI REPL
```
./target/release/claw
```