---
label: Website data migration
order: 80
---

# Migrate existing website to WP Docker

+++ Vietnamese 🇻🇳

Nếu bạn có một website WordPress đang có sẵn cần chuyển về để sử dụng trên WP Docker, bạn có thể dễ dàng làm quá trình này vì chúng tôi có thiết kế sẵn một công cụ giúp bạn thao tác mọi thứ dễ dàng hơn.

Trước khi thực hiện chuyển dữ liệu về, bạn cần chuẩn bị sẵn 2 tập tin sau và đảm bảo dữ liệu đầy đủ:

- Tập tin .zip hoặc .tar.gz chứa mã nguồn WordPress của website
- Tập tin .sql chứa dữ liệu database của website

Sau đó bạn tạo thư mục `/opt/wp-docker/archives/{domain.ltd}`, thay `{domain.ltd}` thành tên miền website của bạn cần chuyển về. Ví dụ mình có website *wpdocker.vn* thì sẽ tạo thư mục với lệnh `mkdir` như sau:

```bash
mkdir -p /opt/wp-docker/archives/wpdocker.vn
```

Sau đó bạn upload hai tập tin đã chuẩn bị vào thư mục này, tên tập tin có thể đặt bất kỳ nhưng đuôi mở rộng phải là `.zip` hoặc `.tar.gz` cho mã nguồn, và `.sql` cho database. Lưu ý, bạn phải đảm bảo chỉ có duy nhất hai (2) tập tin này trong thư mục.

!!!warning Sử dụng sFTP/SSH
Vì lý do bảo mật, WP Docker không tích hợp công cụ File Manager vào bộ cài. Nếu bạn cần upload tập tin nào lên máy chủ, hãy sử dụng sFTP/SSH.
!!!

Sau khi đã chuẩn bị tập tin đầy đủ, bạn truy cập vào menu với lệnh `wpdocker`, chọn chức năng Quản lý website và chọn chức năng Chuyển dữ liệu WordPress về WP Docker.  Sau đó nhập `y` để xác nhận đã chuẩn bị đầy đủ dữ liệu, và nhập tên miền website cần chuyển dữ liệu về. Hệ thống sẽ kiểm tra nếu website đó chưa tồn tại trên WP Docker thì sẽ tiến hành tạo ra, nếu website đã tồn tại trên WP Docker thì sẽ hỏi sao lưu trước khi ghi đè để bạn có thể khôi phục lại trong trường hợp quá trình chuyển dữ liệu bị lỗi.

[![asciicast](https://asciinema.org/a/ORgOpqNtDDLhdXUjlFsMwmkTL.svg)](https://asciinema.org/a/ORgOpqNtDDLhdXUjlFsMwmkTL)
+++ English 🇬🇧

If you have an existing WordPress website that you want to migrate to WP Docker, you can easily do this as we have designed a tool to help you with the process.

Before starting the migration, you need to prepare two files and ensure they contain complete data:

- A .zip or .tar.gz file containing the WordPress source code
- A .sql file containing the website's database

Then create a directory at `/opt/wp-docker/archives/{domain.ltd}`, replacing `{domain.ltd}` with your website's domain name. For example, if you have a website *wpdocker.vn*, create the directory using the `mkdir` command like this:

```bash
mkdir -p /opt/wp-docker/archives/wpdocker.vn
```

Next, upload the two prepared files to this directory. The filenames can be anything, but the extensions must be `.zip` or `.tar.gz` for the source code, and `.sql` for the database. Note that you must ensure there are only these two (2) files in the directory.

!!!warning Using sFTP/SSH
For security reasons, WP Docker does not include a File Manager in the installation package. If you need to upload files to the server, please use sFTP/SSH.
!!!

After preparing the files, access the menu using the `wpdocker` command, select the Website Management function, and choose the Migrate WordPress Data to WP Docker option. Then enter `y` to confirm that you have prepared all the data, and enter the domain name of the website you want to migrate. The system will check if the website doesn't exist on WP Docker, it will create it. If the website already exists on WP Docker, it will ask to create a backup before overwriting, so you can restore it in case the migration process fails.

[![asciicast](https://asciinema.org/a/ORgOpqNtDDLhdXUjlFsMwmkTL.svg)](https://asciinema.org/a/ORgOpqNtDDLhdXUjlFsMwmkTL)