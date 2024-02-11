# massa
Massa Labs Mainnet Validator
#Instalation
Install Ubuntu libs
```bash
sudo apt install pkg-config curl git build-essential libssl-dev libclang-dev cmake
```
Install Rustup
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
configure path
```bash
source $HOME/.cargo/env
```
install rust stable version
```bash
rustup toolchain install 1.74.1
```
set it as default
```bash
rustup default 1.74.1
```
check rust version
```bash
rustc --version
```
clone repo
```bash
git clone https://github.com/massalabs/massa.git
```
go to the cloned repository
```bash
cd massa
```
checkout the latest tag
```bash
git checkout MAIN.2.1
```
