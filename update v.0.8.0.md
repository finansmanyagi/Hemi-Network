## Hemi Network Nedir
Hemi, Bitcoin ve Ethereum tarafından desteklenen ölçeklendirme, güvenlik ve birlikte çalışabilirlik için modüler bir Katman-2 protokolüdür. 

# Faucet işlemleri için discord kanalları
https://discord.gg/hemixyz

### Gereksinimler:
-------------------
### RAM : 2 GB
### Storage : 50 GB
### CPU : 2 Core
### Sunucumuzu güncelliyoruz
```
sudo apt upgrade -y && sudo apt update -y
```
## Screen açalım
```
screen -S hemi 
```
## Güncellemeleri İndirelim: 
```
cd
```
```
curl -L -O https://github.com/hemilabs/heminetwork/releases/download/v0.8.0/heminetwork_v0.8.0_linux_amd64.tar.gz
```
```
tar xvf heminetwork_v0.8.0_linux_amd64.tar.gz
```
```
cd heminetwork_v0.8.0_linux_amd64
```
### Doğru Yüklendiğinden Emin Olmak İçin Help Komutunu Deniyelim :
```
./popmd --help
```
### Bilgilerimizi Ayarlayalım:
* private_key kısmında node etkinliği için olan cüzdan keyinizi yazın.
* Fee'yi biz 3000 ayarlardık - dilerseniz istediğiniz miktarla değiştirebilirsiniz.
```
export POPM_BTC_PRIVKEY=private_key
export POPM_STATIC_FEE=3000
export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public
```
### Başlatalım :
```
./popmd
```
### CTRL A + D ile screen'den çıkabilirsiniz - arkada çalışmaya devam edecektir.
* İstatistiklerinize Bakmak İçin : https://testnet.popstats.hemi.network/
