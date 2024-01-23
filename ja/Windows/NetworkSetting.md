## 目次

1. [インターネット接続の手順](#接続の手順)

    1. [Wired AutoConfigをONにする](#1-wired-autoconfigを起動する)

    2. [802.1x認証設定を行う](#2-8021x認証設定)

    3. [ログインフォームに自分のIDとパスワードを入力](#3idとパスワードの入力)

2. [トラブルシュート](#トラブルシュート)

## 接続の手順

### 1. Wired AutoConfigを起動する

まず、**タスクマネージャー**を起動する

Windowsボタンを右クリックしタスクマネージャーをクリック

![StartTaskManaget](img/startTaskManager.png)

Serviceを選択し、Wired AutoConfigを右クリックし起動をクリック

![RunTaskManager](img/runningAutoConfig.png)


### 2. 802.1x認証設定

まず、コントロールパネルを起動する

Win keyを押して`control panel`と入力

![StartControlPanel](img/searchControllPanel.png)


`ネットワークとインターネット`を選択

![SelectNetwork](img/openControllPanel.png)

`インターネットと共有センター`を選択

![SelectInternet](img/openNetwork.png)

`アダプターの詳細設定`を選択

![SelectAdapter](img/openNetworkConfigure.png)

`Ethernet`を右クリックしてプロパティをクリック

![EthernetProperty](img/openNetConnections.png)

まず、IEEE802.1X認証にチェックを入れます

次にその下にある設定をクリックします

![Ethernet8021x](img/settingIEEE8021x.png)

***一番上のチェックを外してください***

※これを外さないと寮ネットに接続できなくなります

次に下のほうにある認証方法を`EAP-MSCHAPv2`にします

`OK`をクリックします

![EthernetSetting](img/settingEAP.png)

次に`追加設定`をクリックします

認証モードを`ユーザー認証`にしてください

そしてその右にあるボタンをクリックしてIDと
パスワードを設定します

![EthernetUserSetting](img/settingUserCredential.png)

## 3.IDとパスワードの入力

ここに**演習室で使用するMicrosoftのIDとパスワード**を入力してください

※パスワードは初期に使ったパスワードです

![IDandPasswordSetting](img/settingUserPassword.png)

最後にOKをすべてクリックして、接続できたか確認してください

# トラブルシュート

- ここまで設定できたのにインターネットにつながりません

    IPv4の設定で自動設定になっていないかもしれません

    まず、コントロールパネルを立ち上げましょう。

    立ち上げる方法は[ここ](#2-8021x認証設定)に記載してあります

    そしてここまで来たらEthernetのプロパティを開いてください。

    ![](img/openNetConnections.png)

    つぎにIPv4を選択してプロパティを開いてください

    ![](img/ethernetProperties.png)

    もし、ここで両方とも手動設定になっていたら下の画像のように自動設定にしてください

    ![](img/IPv4Properties.png)

    自動設定にしたら、OKをすべて押して接続を確認してください

## 終わりに

ここまでお疲れ様です。良いインターネットライフを。