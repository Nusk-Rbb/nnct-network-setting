# Contents

### 1. [Install NetworkManger](#install-networkmanger)

### 2. [Launch NetworkManger](#launch-networkmanger)

### 3. [802.1x authentication](#8021x-authentication-settings)

### 4. [Connection Confirmation](#connection-confirmation)

# Configuration Network

## Install NetworkManger 

```bash
sudo pacman -S networkmanager
```

## Launch NetworkManger

```bash
sudo systemctl start NetworkManager
```

When NetworkManager starts at the same time the OS starts

```bash
sudo systemctl enable NetworkManager
```

## 802.1x authentication settings

```bash
nmtui
```

Please configure as follows

| Setting items | |
| ---- | ---- |
| Authentication | Protected EAP (PEAP) |
| Anonymous Identity | Student ID |
| No CA | check☑ |
| Inner Atuthentication | MSCHAPv2 |
| Username | Student ID |
| Password | Microsoft Initial password |

![](/Linux/GNU/img/NetworkManager.png)

## Connection Confirmation

```bash
ping -c8 google.com
```