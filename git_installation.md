# gitのインストール

## Gitのダウンロード
### Macの場合
デフォルトで入っていると思うのでターミナルを開き`git -v`を実行してバージョンが表示された場合はダウンロードが完了しています。

### Windowsの場合
[GitのWebサイト](https://git-scm.com/)からダウンロードします。コマンドまたはPowerShellで`git -v`を実行してバージョンが表示された場合は成功です。  
https://www.curict.com/item/60/60bfe0e.html  
パスを通すのはインストーラでできます。


## Gitの設定
GitHubにコミットするときに記録される`名前`と`メールアドレス`を設定します。ここで設定した名前とメールアドレスの公開範囲はリポジトリの公開範囲と同じです。すなわち、少なくとも共同編集者にはメールアドレスが公開されます。個人のメールアドレスを非公開にする場合は(**推奨**)GitHubが提供するメールアドレス以下のように取得して使いましょう。  

コマンドまたはターミナルを開き、`git config user.name <name>`(`<name>`を設定したい名前に置換)を入力して実行してください。  
次に、[GitHubの設定からEmails(ここをクリック)](https://github.com/settings/emails)を開き`Primary email address`の下にある`数字+ ~~ @users.noreply.github.com`のメールアドレスを確認後、コマンドまたはターミナルに`git config user.email <email>`(`<email>`を確認したメールアドレスに置換)を入力、実行。(詳細は[GitHubのコミットメールアドレスを設定する](https://docs.github.com/ja/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)を参照)

これでGitのダウンロードと設定は終了です。

## リポジトリのクローン
リモート（Web）上のファイルを自分のコンピューターにコピーすることです。  
`F1`を押すか上部のバーの`表示`->`コマンドパレット`でコマンドパレットを表示させ`git clone`を入力し画面に従えばクローンできます。ターミナルでもできます。  


## ブランチの作成とコミット
ブランチを使用して、分岐して開発することで共同で編集することが可能になります。予期せぬエラーを防ぐためブランチ名は英語でスペースは使用せずかわりに`-`を使ってください。
コミットとは自分のコンピューターでの変更をリモートブランチ（Web）上に記録することです。  

![Alt text](/sources/images/git_branch.png)]  
※PRはプルリクエストの略です。  
  

VScodeの左下（枝のマーク）のところから新しいブランチを作成できます。  
新しいブランチを作成したあとVScodeの左のところから`ファイルの変更`（枝のマーク）をクリックして`変更をステージ`(+マーク)をクリックして`コミット`を押すとコミットできます。

- https://backlog.com/ja/git-tutorial/stepup/01/
- https://docs.github.com/ja/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches#working-with-branches

