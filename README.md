# Secure File Transfer System

**Bilgisayar Ağları Dönem Projesi**  
**Geliştiren: Hasan Umut Kocatepe** 

Bu proje, hem **UDP hem de TCP** üzerinden şifreli ve güvenli dosya transferini destekleyen bir hibrit sistemdir.  
AES-256 şifreleme, IP spoofing saldırı simülasyonu ve sniffer tabanlı anomali tespiti gibi güvenlik önlemlerini içerir.

---

## Proje Amacı

✔ Dosya transferini şifreli ve güvenli hale getirmek.  
✔ IP spoofing ve flood saldırılarını algılayarak kara listeye almak.  
✔ Kullanıcı dostu GUI arayüzüyle farklı protokolleri desteklemek.

---

## Özellikler

- **AES-256 Şifreleme:** Dosyalar client tarafında şifrelenir, server tarafında çözülür.
- **UDP ve TCP Destekli:** Kullanıcı, GUI üzerinden UDP veya TCP seçimi yapabilir.
- **Sniffer:** Sunucu, ağ trafiğini dinler ve anomali tespiti yapar.
- **IP Kara Liste:** 100 tekrar eden flood saldırılarını tespit eder ve IP’yi kara listeye alır.
- **IP Spoofing Simülasyonu:** Sanal makine üzerinden saldırı testi gerçekleştirilmiştir.
- **GUI (Tkinter):** Kullanıcı dostu bir arayüz sunar.

---

## Klasör Yapısı
	Secure-File-Transfer-System/
	├── .gitignore
	├── Bilgisayar-Aglari-Dönem-Projesi-Final-Raporu_21360859077.pdf
	├── README.md
	├── client.ipynb
	├── config.py
	├── ip-spoof-simulation.ipynb
	├── requirements.txt
	└── server.ipynb

---

## Kurulum
1 - Gerekli Kütüphaneleri yükleyin:
```bash
pip install -r requirements.txt
```

2 - Server'ı başlatın:
```bash
python server/server.ipynb
```

3- Client'ı başlatın:
```bash
python client/client.ipynb
```

4- IP Spoofing Simulasyonunu Çalıştırın(Ayrı bir cihaz veya sanal makine aracılığıyla):
```bash 
sudo python3 attack_simulation/ip_spoofing_simulation.py
```

## Youtube Tanıtım
- https://youtu.be/0f_NkozS7wQ

>Bu proje Bursa Teknik Üniversitesi 2024-2025 Bahar Dönemi Bilgisayar Ağları Dersi için gönderilmiştir.
