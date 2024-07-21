# vue js 基礎編

## 学習動画
 - https://www.youtube.com/watch?v=Oyr0sr6l3SQ

 ## コース内容あ
 - course.png 参照

 ## 学習整理
 - 全体像
    コンポーネントをもとに一つのアプリを作っている
        コンポーネントはファイルという形式で成り立ってる => .vue(単一ファイルコンポーネント)
 - 今回使用するもの
    - vite
        インストール方法：https://zenn.dev/zakimaz/articles/94f5b67fc7b585
        コマンド: ```npm create vue@latest```
        ※上記のコマンドはnode.jsが入ってないと実行できない
    - node.js
        インストール方法：https://zenn.dev/tmasuyama1114/books/vue-rails-chat/viewer/node-js-installation
        ヴァージョン確認：```node -v ```|| ```node --version```
    - VSCode
        インストール方法：https://zenn.dev/karaage0703/books/80b6999d429abc8051bb/viewer/5b814b
 - ファイル内容整理
    【week1/vue-lesson/package.json】
        dependencies => 本番環境で使われるもの
        devDependencies => テスト環境で使われるもの
        script
            dev: テスト環境実行のためのコマンドで用いる。実行すると右側の内容が実行される様になっている。
            build: 本番環境にアップするためのファイル群を作るためのコマンド => distフォルダが作られる
            preview: 正しく動作するかどうか確認するためのコマンド
            lint: コードが正しく書けているかチェックしてくれるコマンド
            format: フォーマットを整えてくれるコマンド => 今回はprettierがそれをやってくれる