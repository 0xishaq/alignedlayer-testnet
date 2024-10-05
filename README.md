# alignedlayer testnet
![aligned](https://github.com/user-attachments/assets/6a884b40-4db3-448a-ac58-e62e6a61e4d0)

# Aligned Testnet tutorial
Kalian bisa mengerjakan tutorial ini di vps yang kalian pakai untuk run node

- Install Rust
```bash
source <(wget -O - https://raw.githubusercontent.com/0xishaq/installation/main/rust.sh)
```
- Install Foundry
```bash
source <(wget -O - https://raw.githubusercontent.com/zunxbt/installation/main/foundry.sh)
```
- Install OpenSSL and pkg-config
```bash
sudo apt update && sudo apt install pkg-config libssl-dev
```
- Import burner wallet terus kalian isi sama Holesky ETH 0,1 eth sudah cukup.
```bash
[ -d ~/.aligned_keystore ] && rm -rf ~/.aligned_keystore && echo "Deleted existing directory ~/.aligned_keystore." ; mkdir -p ~/.aligned_keystore && cast wallet import ~/.aligned_keystore/keystore0 --interactive
```
- Clone Repo dari Aligned Layer
```bash
[ -d aligned_layer ] && rm -rf aligned_layer && echo "Deleted existing aligned_layer directory." ; git clone https://github.com/yetanotherco/aligned_layer.git && cd aligned_layer/examples/zkquiz
```
- Terakhir jalankan command berikut
```bash
make answer_quiz KEYSTORE_PATH=~/.aligned_keystore/keystore0
```
- Jika sudah kalian harus menjawab pertanyaan, dan berikut jawabannya :

`y`,`c`,`c`,`a`,`y`
