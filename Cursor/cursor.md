# インストール
[公式サイト](https://www.cursor.com/)からインストールする

# 起動のための設定
インストールすると、こんな画面になるので、設定を行う。

![](images/2024-07-20-17-15-12.png)

- Language for AI: AIに入力する言語を書いておく
- Codebase-wide: コードベース全体をエンべディング(埋め込み)するかどうか。これを有効にすると、プロジェクトのコード全体に対してAI検索が適用されるようになる。(コード全体を読み取られたくない場合は無効にする)
- Add Terminal Command: ターミナルにコマンドを追加する。これを有効にすると、ターミナルに`cursor`と入力するだけで、cursorが起動するようになる。vscodeの`code.`のようなもの。(私はVSCodeと使い分けたいため、cursorのみをインストール。)

Continueをクリックすると、VSCodeの拡張機能をインポートするかの選択がある。User Extensionsをクリックすると、自動的にVSCodeの拡張機能がインストールされる。
![](images/2024-07-20-17-24-44.png)

VSCodeでGithub Copilotを使用している場合は、以下のような画面がでる。CursorのCopilot++っていうCopilotよりもイケイケのものでoverrideするけどええか？って聞いている。今回はそれでokなので、Continue with Defaultをクリック。

![](images/2024-07-20-17-27-38.png)


**1番重要なところ**データをOpenAIに送信するかどうかの設定に移る。デフォルトでは送信されるようになっているので要注意。今回は送信したくないので、Privacy ModeにしてContinueをクリック。

![](images/2024-07-20-17-35-44.png)

すると、ログインやサインアップを求められるので、サインアップを行う。

![](images/2024-07-20-17-36-03.png)

ログインすると、VSCodeとほぼ同じ画面がでてくる。これにて起動の設定は終了！
![](images/2024-07-20-17-40-23.png)

# Cursorの設定
macであれば、左上のCursor -> Preferences -> Cursor Settingsをクリックする。

![](images/2024-07-20-18-46-43.png)

## ツールバーを縦方向にする
VSCodeと同様に、ツールバーを縦方向にする。
Cursroの任意の場所で`cmd+,`をして、設定ファイルを開く。設定ファイルで、orientationをverticalに変更する。

![](images/2024-07-23-17-53-27.png)