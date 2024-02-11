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
Route your node, port 31244 & 31245
```bash
ufw allow 31244 && ufw allow 31245
```
edit the file massa-node/config/config.toml
```bash
nano massa-node/config/config.toml
copy and paste this config [https://github.com/massalabs/massa/blob/main/massa-node/base_config/config.toml] to your config.toml
```
config/set your node public IP Address
```bash
routable_ip = "YourNodePublicIPAddress"
```
save that .toml update configuration
```bash
(CTRL+X) then (CTRL+Y) then (ENTER)
```
Launch your node, Replace <PASSWORD> with a password that you will need to keep to restart your node
```bash
cd massa/massa-node/
./massa-node -p <PASSWORD> |& tee logs.txt
```
