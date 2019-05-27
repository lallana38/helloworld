Rubyのバージョン 2.5.1
Railsのバージョン　5.2.3
MySQL

共同開発課題１　「「Hello World」を表示したアプリをGithubにあげる」
内容:　'/users'にアクセスされると、「Hello World!!!」と表示されます。

やったこと:
1. ルーティングを決める
   デフォルトのURLの後ろが'/users'でアクセスされると、usersコントローラーのindexアクションに処理を渡す
2. app/controllersにusers_controller.rbを作成
   コントローラーの機能を使えるようになるため、ApplicationControllerを継承する
3. indexアクションを定義する
4. ビューにusersフォルダを作りindex.html.erbファイルを作成する

学んだこと:
indexアクションに書いた処理をビューに表示させるには、インスタンス変数が必要。
rails g controllerというコマンドを使わずに実装できるようになることが大事。

共同開発課題２　「Githubにアップした「Hello World」アプリをローカルにクローンして動作確認」
やったこと：
1. https://github.com/lallana38/helloworldのcloneordownloadボタンを押下して
　　urlをコピーする
2. ターミナルからデスクトップにgit clone https://github.com/lallana38/helloworld.gitを
　　入力する
3. デスクトップにできたhello worldアプリをrails sで立ち上げて確認する。

学んだこと:
クローンとは
「リモートリポジトリにプッシュされて登録されているソースコードを自分のパソコンにコピーしてくること。
他の人が書いたソースコードを自分のパソコンに持ってくることによって共同開発ができる。」
