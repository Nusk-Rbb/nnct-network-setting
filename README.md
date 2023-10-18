# NNCT Networking Setting

## Windows

## 1. 流れ

1\. Wired AutoConfigをONにする

2\. 802.1x認証設定を行う

3\. ログインフォームに自分のIDとパスワードを入力

## 2. 具体的な方法

### 1. Wired AutoConfigを起動する

まず、**タスクマネージャー**を起動する

Windowsボタンを右クリックしタスクマネージャーをクリック

![StartTaskManaget](img/Screenshot%202023-10-19%20000938.png)

Serviceを選択し、Wired AutoConfigを右クリックし起動をクリック

![RunTaskManager](img/Screenshot%202023-10-19%20011526.png)


### 2. 802.1x認証設定

まず、コントロールパネルを起動する

Win keyを押して`control panel`と入力

![StartControlPanel](img/Screenshot%202023-10-19%20012127.png)


`ネットワークとインターネット`を選択

![SelectNetwork](img/Screenshot%202023-10-19%20012429.png)

`インターネットと共有センター`を選択

![SelectInternet](img/Screenshot%202023-10-19%20012607.png)

`アダプターの詳細設定`を選択

![SelectAdapter](img/Screenshot%202023-10-19%20012627.png)

`Ethernet`を右クリックしてプロパティをクリック

![EthernetPropaty](img/Screenshot%202023-10-19%20012644.png)

まず、IEEE802.1X認証にチェックを入れます

次にその下にある設定をクリックします

![Ethernet8021x](img/Screenshot%202023-10-19%20012719.png)

***一番上のチェックを外してください***

※これを外さないと寮ネットに接続できなくなります

次に下のほうにある認証方法を`EAP-MSCHAPv2`にします

`OK`をクリックします

![EthernetSetting](img/Screenshot%202023-10-19%20012742.png)

次に`追加設定`をクリックします

認証モードを`ユーザー認証`にしてください

そしてその右にあるボタンをクリックしてIDと
パスワードを設定します

![EthernetUserSetting](img/Screenshot%202023-10-19%20012759.png)

## 3.IDとパスワードの入力

ここに**演習室で使用するMicrosoftのIDとパスワード**を入力してください

※パスワードは初期に使ったパスワードです

![IDandPasswordSetting](img/Screenshot%202023-10-19%20012844.png)

最後にOKをすべてクリックして、接続できたか確認してください

## 終わりに

ここまでお疲れ様です。良いインターネットライフを。