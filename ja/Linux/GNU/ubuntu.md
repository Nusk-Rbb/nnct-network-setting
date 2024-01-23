# 目次

### 1. [802.1x認証の設定](#8021x認証の設定)

### 2. [接続確認](#接続確認)

# ネットワーク設定

## 802.1x認証の設定

NetworkManagerを起動して以下のように設定を行ってください

| 設定項目 | |
| ---- | ---- |
| Authentication | Protected EAP (PEAP) |
| Anonymous Identity | 学籍番号 |
| No CA | check☑ |
| Inner Atuthentication | MSCHAPv2 |
| Username | 学籍番号 |
| Password | マイクロソフトの初期パスワード |

![](/Linux/GNU/img/NetworkManager.png)

## 接続確認

```bash
ping -c8 google.com
```