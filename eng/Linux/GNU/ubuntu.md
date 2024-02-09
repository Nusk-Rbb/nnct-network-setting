# Contents

### 1. [802.1x authentication settings](#1-8021x-authentication-settings)

### 2. [Connection Confirmation](#2-connection-confirmation)

# Network setting

### 802.1x authenticaton settings

Please configure as follows

| Setting items | |
| ---- | ---- |
| Authentication | Protected EAP (PEAP) |
| Anonymous Identity | Student ID |
| No CA | check☑ |
| Inner Atuthentication | MSCHAPv2 |
| Username | Student ID |
| Password | Microsoft Initial password |

![](./img/Networkmanager.conf.png)

### Connection Confirmation

```bash
ping -c8 google.com
```