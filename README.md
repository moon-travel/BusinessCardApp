# BusinessCardApp

BusinessCardApp は **iPhone向けのデジタル名刺管理アプリ**です。

受け取った名刺の登録・管理と、自分のデジタル名刺の作成・共有を、ひとつのアプリで行えます。

> **対応OS:** iOS 17以降

---

# 主な機能

## 📇 名刺の登録

- 手入力で名刺を登録
- OCR（カメラ・フォトライブラリ）による自動読み取り
- 以下の情報を管理
  - 氏名
  - 会社名
  - 部署・役職
  - 電話番号
  - メールアドレス
  - メモ
  - 登録日
  - タグ

---

## 📚 名刺一覧

- 名前・会社名で並び替え
- キーワード検索
- タグによる絞り込み
- 連絡先登録状況でのフィルタリング
- 複数選択して一括削除
- CSVエクスポート

---

## 💳 マイ名刺

自分のデジタル名刺を作成できます。

### デザイン名刺

- レイアウトを選択
- 背景写真を設定

### 写真名刺

- 紙の名刺（表・裏）をそのまま登録

---

## 📤 名刺の共有

- AirDrop
- QRコード

で自分の名刺を送信できます。

受け取った相手は **.nametag** ファイルとしてそのままBusinessCardAppへ取り込めます。

---

## 📁 エクスポート

- vCard（連絡先アプリ）
- CSV

へ書き出しできます。

---

## 🏠 ホーム画面ウィジェット

Widgetを追加すると、

**自分の名刺のQRコード**

をホーム画面へ表示できます。

---

# 技術スタック

- SwiftUI
- WidgetKit
- VisionKit（OCR・ライブスキャン）
- CoreData
- App Groups

---

# インストール方法

BusinessCardAppは **SideStore** を利用して無料でインストールできます。

Apple Developer Programへの加入は不要です。


---


# 注意

このアプリのインストールはデベロッパーモードの有効化を前提としています。
Apple公式はデベロッパーモードの有効化により、セキュリティの低下が発生する可能性があるとしています。
そのため、十分注意して使用してください。また、アプリ作成者はインストールにより起きた損害に対して一切の責任を負いません。
必ず自己責任で行ってください。

---


## 必要なもの

- iPhone（iOS 17以上）
- Apple ID（無料で可）
- Mac または Windows（初回セットアップのみ）
- Wi-Fi環境

---

## 1. SideStoreをインストール

SideStore公式サイトから **iLoader** をダウンロードします。

https://sidestore.io

iLoaderを起動し、iPhoneをUSB接続して **SideStore (Stable)** をインストールしてください。

---

## 2. iPhoneを設定

**設定**

→ **一般**

→ **VPNとデバイス管理**

→ Apple ID

→ **信頼**

を選択します。

続いて

**設定**

→ **プライバシーとセキュリティ**

→ **Developer Mode**

をオンにしてください。

---

## 3. LocalDevVPNをインストール

App Storeから

**LocalDevVPN**

をインストールしてください。

起動後、

**Connect**

を押してVPNを有効にします。

BusinessCardAppのインストール・更新時は、LocalDevVPNを接続してください。

---

## 4. Sourceを追加

SideStoreを開き、

**Sources**

→ **＋**

を押して以下を追加します。

```
https://moon-travel.github.io/BusinessCardApp/apps.json
```

---

## 5. インストール

Sourceに表示された

**BusinessCardApp**

を選び、

**Install**

を押してください。

---

# アップデート

新しいバージョンが公開されたら

1. LocalDevVPNを接続
2. SideStoreを開く
3. My Apps
4. Refresh または Update

で最新版へ更新できます。

---

# よくある質問

## 「Cannot register more than 10 App IDs」と表示される

Apple無料アカウントでは、

**7日間で10個まで**

という制限があります。

BusinessCardAppはWidgetを使用するため、

**2個のApp ID**

を利用します。

表示された時間が経過してから再度インストールしてください。

---

## SideStoreの署名期限が切れた

SideStoreで

**Refresh All**

を実行してください。

---

## BusinessCardAppがインストールできない

以下を確認してください。

- LocalDevVPNが接続されている
- SideStoreが最新
- Apple IDのApp ID上限に達していない

---

# ライセンス

MIT License
