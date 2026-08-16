# Day 01 — Networking ve HTTP

## Kavramlar
- IP adresi:
- Port:
- DNS:
- TCP:
- HTTP:
- HTTPS/TLS:

## Uyguladığım komutlar
- `nslookup example.com`
- `curl.exe -I https://example.com`
- `Test-NetConnection example.com -Port 443`

## Gözlemlerim
- DNS sonucu:
- HTTP durum kodu:
- Dikkatimi çeken response header'ları:
- 443 portunun anlamı:

## Bugün öğrendiklerim

## Anlamadığım konular

## Yarın
Linux komut satırı ve dosya izinleri

## Karşılaştığım sorun

OpenCode bağlantısında `certificate is not yet valid` hatası aldım.

- Neden: Windows sistem saati gerideydi.
- Çözüm: Tarih ve saat ayarlarını otomatik eşitledim.
- Öğrendiğim: TLS sertifikaları yerel sistem saatine göre geçerlilik kontrolünden geçer.
- ## DNS Sorunu ve Çözümü

Varsayılan DNS sorguları zaman aşımına uğruyordu.

- Neden: Modemin dağıttığı IPv6 link-local DNS sunucusu cevap vermiyordu.
- Test: IPv4 ve IPv6 Cloudflare DNS sunucularına yapılan doğrudan sorgular başarılıydı.
- Çözüm: Ethernet DNS ayarlarını Cloudflare IPv4 ve IPv6 adresleriyle değiştirdim.
- Doğrulama: `nslookup google.com` zaman aşımı olmadan A ve AAAA kayıtlarını döndürdü.
