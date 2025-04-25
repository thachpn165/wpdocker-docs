---
order: 90
label: Install Let's Encrypt
---
# Install free SSL with Let's Encrypt

+++ Vietnamese 🇻🇳
[![video cài đặt Let's Encrypt cho website](https://asciinema.org/a/zY9xZJCVNDIWfxNifXpE83Xxj.svg)](https://asciinema.org/a/zY9xZJCVNDIWfxNifXpE83Xxj)
Để cài đặt chứng chỉ SSL miễn phí từ Let's Encrypt, bạn phải thực hiện trỏ tên miền về địa chỉ IP của VPS/Máy chủ đang cài đặt WP Docker.

## Cài đặt Let's Encrypt qua menu

Bạn truy cập vào menu với lệnh `wpdocker menu` và chọn chức năng Quản lý Chứng chỉ SSL, sau đó chọn chức năng Cài chứng chỉ miễn phí từ Let's Encrypt và chọn website trên hệ thống cần cài đặt để quá trình cài đặt diễn ra tự động.

## Cài đặt Let's Encrypt qua lệnh wpdocker

Sử dụng lệnh sau để cài Let's Encrypt cho website.

```bash
wpdocker ssl install letsencrypt DOMAIN
```

Thay `DOMAIN` thành tên miền website của bạn.

+++ English 🇬🇧
[![Let's Encrypt installation video for website](https://asciinema.org/a/zY9xZJCVNDIWfxNifXpE83Xxj.svg)](https://asciinema.org/a/zY9xZJCVNDIWfxNifXpE83Xxj)

To install a free SSL certificate from Let's Encrypt, you need to point your domain to the IP address of the VPS/Server where WP Docker is installed.

## Installing Let's Encrypt via Menu

Access the menu using the `wpdocker menu` command, select the SSL Certificate Management function, choose the Install Free Certificate from Let's Encrypt option, and select the website on the system that needs the certificate. The installation process will run automatically.

## Installing Let's Encrypt via wpdocker Command

Use the following command to install Let's Encrypt for your website:

```bash
wpdocker ssl install letsencrypt DOMAIN
```

Replace `DOMAIN` with your website's domain name.