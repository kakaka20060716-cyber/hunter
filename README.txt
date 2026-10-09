LIFE HUNTER PWA（Android用）

内容:
- index.html: アプリ本体
- manifest.webmanifest: ホーム画面追加用設定
- sw.js: オフラインキャッシュ
- icon.svg: アプリアイコン

Androidでホーム画面に追加するには、HTTPSで公開する必要があります。
ローカルのHTMLファイルを直接開いただけでは、PWAとして正常にインストールできません。

簡単な公開方法（GitHub Pages）:
1. GitHubにログインし、新しいPublic repositoryを作成（例: life-hunter）。
2. このZIPを解凍し、4ファイルをリポジトリの最上位にアップロードしてCommit。
3. Repositoryの Settings > Pages > Build and deployment で「Deploy from a branch」を選択。
4. Branchを main、フォルダを /(root) にして Save。
5. 公開された https://ユーザー名.github.io/life-hunter/ をAndroidのChromeで開く。
6. Chromeの ⋮ メニューから「アプリをインストール」または「ホーム画面に追加」を選ぶ。
7. 追加したアイコンからLIFE HUNTERを起動。

記録:
- XP、達成クエスト、週間記録はブラウザのlocalStorageに保存され、外部サーバーには送信しません。
- ブラウザデータを消去したり、アプリデータを削除すると記録が消える可能性があります。
- アプリ内の「記録をバックアップ」でJSONを保存し、機種変更や消去前にバックアップしてください。
- 復元は「バックアップを復元」から行えます。

注意:
- この版は単一端末のローカル保存です。複数端末同期はありません。
- 週間クエストの進捗は、このアプリ内で記録されたデイリー達成に基づきます。
