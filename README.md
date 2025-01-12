# network3-node-setup
![image](https://github.com/user-attachments/assets/0369dbfb-4dd4-4380-9b7c-256108744216)

---

### Minimum Donanım Gereksinimleri  
▫️ **CPU:** 1vCPU  
▫️ **RAM:** 2GB  
▫️ **Depolama:** 60GB SSD  

### Network3 Üzerine Hesap Kaydı:  
[https://account.network3.ai/register_page?rc=fffda9d8](https://account.network3.ai/register_page?rc=fffda9d8)  

1. E-posta adresinizi ve şifrenizi girin.  
2. Gerekirse yönlendirme kodunu girin: **fffda9d8**  
3. **Solana Wallet (Phantom)** bağlayın.  

✅ **Tamamlandı!**  

---

### Kurulum  

**1. Bağımlılıkları Yükleyin:**  
Terminale aşağıdaki komutları girin:  

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install net-tools -y
```

**2. Ubuntu Node'u İndirin:**  

```bash
cd $HOME
wget https://network3.io/ubuntu-node-v2.1.1.tar.gz
```

**3. Dosyayı Çıkartın:**  

```bash
tar -xzf ubuntu-node-v2.1.1.tar.gz
```

**4. 8080 Portunu Açın:**  

```bash
sudo ufw allow 8080
sudo ufw reload
```

**5. Node’u Çalıştırın:**  

```bash
cd ubuntu-node
sudo bash manager.sh up
```

*) Terminalde "node is ready" mesajını görene kadar bekleyin, bu mesaj node'un başarıyla çalıştığını gösterir.  
![image](https://github.com/user-attachments/assets/81c6227b-2130-435b-bf23-5aa26e678765)

---

**6. Node Hesabınıza Özel Anahtar Üretin:**  

```bash
sudo bash manager.sh key
```

*) Çıktıdan özel anahtarı kopyalayın ve güvenli bir şekilde saklayın.  
![image](https://github.com/user-attachments/assets/c9ea3dd3-4083-4b57-878b-41c54d1184ed)

---

### Node’un Çalışıp Çalışmadığını Doğrulama  

1. Tarayıcıyı açın ve şu adresi ziyaret edin:  
   **https://account.network3.ai/main?o=xx.xx.xx.xx:8080**  
   *) "xx.xx.xx.xx" kısmını kendi VPS IP adresinizle değiştirin.  

2. Daha önce kaydolduğunuz hesap bilgileriyle giriş yapın.  

3. Özel node anahtarını kopyalayın.  
   a. Dashboard üzerindeki mevcut node panelinin sağ üst köşesindeki '+' düğmesine tıklayın.
   ![image](https://github.com/user-attachments/assets/cf11eb9e-7ba1-4c5d-b43a-40f712a27bd2)
   
   b. Özel anahtarı yapıştırın ve "Tamam" butonuna basın.
   
   ![image](https://github.com/user-attachments/assets/b3fd5573-59e0-4733-99e1-7355338b626f)




✅ **Tamamlandı!**  

---

### Hızlı Çözümler  

Eğer "+" düğmesini bulamazsanız, node’u durdurup yeniden başlatabilirsiniz:  

```bash
sudo bash manager.sh down  # Node'u durdurmak için  
sudo bash manager.sh up    # Node'u başlatmak için  
```  

--- 

# Destek için repoyu yıldızlamayı ve beni takip etmeyi unutmayın.
# Sevgiler.
# CemS
