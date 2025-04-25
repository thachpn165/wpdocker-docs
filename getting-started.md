---
order: 400
---
# Getting started

+++ Vietnamese 🇻🇳

## Chuẩn bị trước cài đặt

- Hệ điều hành:
  - Ubuntu 22 hoặc mới hơn
  - AlmaLinux 8 hoặc mới hơn
  - macOS.
  - Mặc dù WP Docker sẽ tự cài đặt Docker và Docker Compose, nhưng khuyến khích tự cài Docker & Docker Compose thủ công trước khi sử dụng WP Docker.

- Cấu hình tối thiểu:
  - RAM: 1 GB
  - CPU: 1 core

## Lệnh cài đặt

Tải về file installer và thực thi cài đặt với lệnh sau:

```bash
curl -fsSL https://raw.githubusercontent.com/thachpn165/wp-docker/refs/heads/main/src/install.sh -o install.sh && bash -i install.sh
```

Ở lần chạy đầu tiên, bạn sẽ cần chọn kênh phân phối phiên bản. WP Docker hỗ trợ những kênh phiên bản như sau:

- **Official**: Kênh phiên bản ổn định
- **Nightly**: Phiên bản cập nhật sớm và chỉ dùng để kiểm thử
- **Dev**: Chọn tùy chọn này sẽ clone source từ Github và không tự động cập nhật phiên bản, sử dụng `git pull` để cập nhật thủ công

Nếu bạn là người sử dụng thông thường, hãy luôn chọn kênh *Official* để đảm bảo dùng những phiên bản ổn định. Bạn cũng có thể đổi kênh phiên bản sau này trên chức năng menu hoặc lệnh `wpdocker core channel change`.

Sau khi cài đặt hoàn tất, bạn cần thoát ra khỏi terminal và truy cập vào lại để mở menu với lệnh `wpdocker menu` và bắt đầu sử dụng. Bạn có thể truy cập vào thư mục của WP Docker tại `/opt/wp-docker` nếu cần thao tác thêm.

Lần đầu tiên truy cập vào menu với lệnh `wpdocker` hệ thống sẽ hỏi bạn chọn ngôn ngữ sử dụng. Tùy chọn này cũng có thể thay đổi sau tại tính năng Công cụ hệ thống hoặc lệnh `wpdocker core lang change --lang=en`.

## Xóa cài đặt

Vì lý do nào đó bạn không muốn sử dụng WP Docker nữa thì có thể xóa nó đi với lệnh sau:

```bash
wpdocker core uninstall
```

Nó sẽ xóa toàn bộ các dữ liệu liên quan đến WP Docker, các container webserver (NGINX), MariaDB, Redis, PHP của các website. Hãy sao lưu dữ liệu quan trọng trước khi xóa.

+++ English 🇬🇧

## Pre-installation Requirements

- Operating System:
  - Ubuntu 22 or newer
  - AlmaLinux 8 or newer
  - macOS
  - Although WP Docker will automatically install Docker and Docker Compose, it's recommended to manually install Docker & Docker Compose before using WP Docker.

- Minimum System Requirements:
  - RAM: 1 GB
  - CPU: 1 core

## Installation Command

Download and run the installer with the following command:

```bash
curl -fsSL https://raw.githubusercontent.com/thachpn165/wp-docker/refs/heads/main/src/install.sh -o install.sh && bash -i install.sh
```

On first run, you'll need to select a version distribution channel. WP Docker supports the following channels:

- **Official**: Stable version channel
- **Nightly**: Early updates for testing only
- **Dev**: This option clones the source from Github and doesn't auto-update. Use `git pull` for manual updates

For regular users, always choose the *Official* channel to ensure stable versions. You can change the version channel later through the menu or using the command `wpdocker core channel change`.

After installation completes, you need to exit and reopen the terminal to access the menu with the `wpdocker menu` command and start using it. You can access the WP Docker directory at `/opt/wp-docker` for additional operations.

When you first access the menu with the `wpdocker` command, the system will ask you to select your preferred language. You can change this later in the System Tools feature or using the command `wpdocker core lang change --lang=en`.

## Uninstall

If you no longer want to use WP Docker for any reason, you can remove it with the following command:

```bash
wpdocker core uninstall
```

This will remove all WP Docker related data, including webserver (NGINX), MariaDB, Redis, and PHP containers for all websites. Make sure to backup important data before uninstalling.