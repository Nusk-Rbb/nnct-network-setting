# 目次

### 1. [NetworkManagerをインストール](#networkmanagerをインストール)

### 2. [NetworkManagerを起動](#networkmanagerを起動)

### 3. [802.1x認証の設定](#8021x認証の設定)

### 4. [接続確認](#接続確認)

# ネットワーク設定

## NetworkManagerをインストール

```bash
sudo apt install networkmanager
```

## NetworkManagerを起動

```bash
sudo systemctl start NetworkManager
```

OSが起動と同時にNetworkManagerも起動する場合

```bash
sudo systemctl enable NetworkManager
```

## 802.1x認証の設定

以下のように設定を行ってください

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