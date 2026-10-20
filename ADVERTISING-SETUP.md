# 広告配信は未開始

2026-10-21：広告アカウント未登録のため、広告SDK・広告コード・実在しない広告IDは組み込んでいません。ad-config.jsonは状態を記録する設定で、自動的に広告コードを読み込むものではありません。

1. 所有者本人がGoogle AdSense等に登録し、本人情報・支払情報・利用規約を確認する。
2. サイトの登録可否と独自ドメインの必要性を広告事業者に確認し、所有権確認とサイト審査を進める。公開URLがあるだけでは配信承認にはならない。
3. 承認済みの広告コードと必要な同意管理を実装し、プライバシー説明を更新する。
4. 広告はカタログ等の説明ページで検討。ゲームページには現在広告を設置していない。AdSenseのゲーム画面から150px以上離す配置条件等を確認する。
5. 広告テストとiPhone/Androidの操作確認後に有効化する。H5 Games Adsは別途条件・申請を確認する。

公式参考：
- https://support.google.com/adsense/answer/7584263?hl=ja
- https://support.google.com/adsense/answer/2768340?hl=ja
- https://support.google.com/adsense/answer/9959170?hl=ja

## Webアプリ

Android Chromeのホーム画面追加・インストールに向けたmanifest、PNGアイコン、ネットワーク専用Service Workerを同梱。オフラインプレイ非対応。Google Playストア向けAPK/AABは今回の対象外。iPhone Safariもホーム画面追加に対応。

既存10作品から別ディレクトリへコピーし、Web版だけYouTube SDK読み込みを削除。元の公開サイトとPlayables向けソースは変更していない。新サイトの各ゲームの保存キーに専用接頭辞を付けた。
