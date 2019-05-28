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

共同開発課題３　「「Hello World」アプリでブランチ作成・任意の変更を加える・コミット・プッシュ・プルリク」
内容：　Hello WorldアプリにGood Morning!の文言を追加し、githubに反映させる。
やったこと：
1. git checkout -b "add_good_morning"で新しいブランチを作成する
2. index.html.erbにGood Morning!を追加する
3. git add .
   git commit -m "add_good_morning"でローカルリポジトリにコミット（変更を記録）する
4. git push origin add_good_morningを実行
5. https://github.com/lallana38/helloworld　に新しいブランチが作られるので
　　「compare & pullrequest」を押下し、プルリクエストを作成
6. 「Good Morningを追加しました。」と入力し、「create pullrequest」ボタンを押下

学んだこと：
プルリクエストとは
自分のパソコンで開発したソースコードをリモートリポジトリにプッシュした後に
コードレビューを依頼すること・他の人にソースコードに変更があったことを通知すること
