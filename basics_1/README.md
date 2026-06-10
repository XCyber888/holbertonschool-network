# 0-change_your_home_IP

Bu Bash skripti Ubuntu serverində **/etc/hosts** faylını dəyişərək:
- `localhost` → `127.0.0.2`
- `facebook.com` → `8.8.8.8`

## İstifadə

```bash
sudo ./0-change_your_home_IP
```

## Nümunə

Skriptdən əvvəl:
```
ping localhost       → 127.0.0.1
ping facebook.com    → 157.240.11.35
```

Skriptdən sonra:
```
ping localhost       → 127.0.0.2
ping facebook.com    → 8.8.8.8
```

## Qeyd

- Skript **root** icazəsi tələb edir (`sudo`).
- Dəyişiklikləri geri qaytarmaq üçün `/etc/hosts` faylından əlavə edilmiş sətirləri silin.
