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


## Cursorの詳細設定
右上の歯車マークから、settingsを開いて、Featuresタブを開く。すると、いくつか設定項目があると思うが、それぞれの意味は以下のような感じ。

**Chat**
- **Always search the web**: すべてのプロンプトに`@web`を含めるのと同じように、常にウェブ検索を行う設定。
- **Fade chat stream**: 有効にすると、チャットがフェード効果で表示される。
- **Default no context**: デフォルトでコンテキストなしでチャットを送信する設定。
- **@ symbol suggestions**: AIチャットで`@`シンボルの提案を行う設定。
- **Narrow scrollbar**: AIチャット用に狭いスクロールバーを使用する設定。

**Editor**
- **Show chat/edit tooltip**: エディタ内でハイライトされたコードの近くにチャット/編集ツールチップを表示する設定。
- **Auto parse inline edit links**: `^/⌘ + K`入力に貼り付けられたリンクを自動的に解析する設定。
- **Auto select for Ctrl/⌘ + K**: インラインコード編集のために自動的に領域を選択する設定。
- **Use themed diff backgrounds**: インライン差分のためにテーマ背景色を使用する設定。
- **@ symbol suggestions for Ctrl/⌘ + K**: `Ctrl/⌘ + K`で`@`シンボルの提案を行う設定。

**Terminal**
- **Terminal hint**: ターミナルの下部にヒントテキストを表示する設定。
- **Show terminal hover hint**: ターミナル内で「Add to chat」などのヒントを表示する設定。

私の設定は以下のようにした。

![](images/2024-07-24-11-12-05.png)