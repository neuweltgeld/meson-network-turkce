Meson Network Türkçe kurulum adımları

Kullandığım sistem
1 vCPU
1GB RAM
25GB Disk


Öncelikle https://dashboard.meson.network adresinden kayıt olup, oturum açtıktan sonra Nodes sekmesine geliyoruz.

# Sunucumuzda gerekli ayarlamayı yapıyoruz
```
sudo apt-get update -y && sudo apt-get install wget -y
```

# Node sekmesine geldiğinde göreceğiniz 1 Nolu 1. download & install kodu çalıştırıp kurulumu yapıyoruz.

![alt text](https://dashboard.meson.network/img/cmd_pic.2565de46.png)

# tokenadresi yazan yere node sayfasında gördüğünüz token adresini yapıştırıyorsunuz. 
# cahce.size kısmı sunucunuzdan ne kadar yer ayıracağınızı belirler.
# Direkt olarak sayfada bulunan 2. set token and config nolu kodu da kopyalayabilirsiniz.
```
sudo ./meson_cdn config set --token=tokenadresi --https_port=443 --cache.size=20
```

# Port açmak için aşağıdaki kodları giriyoruz.
```
sudo ufw enable
```
```
sudo ufw allow 443
```

# Son olarak sistemi başlatıyoruz. 
```
sudo ./service start meson_cdn
```

Node sayfanızı 1dk sonra yenilediğinizde sunucunuza ait bilgileri görebilirsiniz.

Meson Network Linkleri
admin@meson.network
https://t.me/mesonnetwork
https://discord.gg/Qu7archn
