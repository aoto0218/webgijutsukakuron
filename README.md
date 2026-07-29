# 手順書


まず'Docker Compose'と'git'が使える環境を構築します。


このリポジトリをクローンします。
```bash
git clone https://github.com/aoto0218/webgijutsukakuron.gi
```


docker compose upします。
```bash
docker compose up
```


mysqlに入ります。
```bash
docker compose exec mysql mysql example_db
```


テーブルを作成します。
```bash
CREATE TABLE `bbs_entries` (`id` INT UNSIGNED NOT NULL AUTO_INCREMENT PRIMARY KEY,`body` TEXT NOT NULL,`created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,`image_filename` TEXT DEFAULT NULL);
```


ブラウザでアクセスします。
```bash
ec2のパブリックIP/bbsimagetest.php
```
