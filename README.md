# Git-it

![ss](https://raw2.github.com/jlord/git-it/master/git-it-ss.png)

これはGitとGithubを学ぶための [workshopper](https://github.com/rvagg/workshopper) のモジュールです。

ターミナル上に問題形式で設問が表示されます。
その問題を解き進めていくことでGitとGithubについて学習することができます。

詳細は[nodeschool.io](http://nodeschool.io)をご覧ください。

---

**For developer documentation, see [CONTRIBUTING.md](https://github.com/jlord/git-it/blob/master/CONTRIBUTING.md).**

**Mentoring at an event with Git-it? Run through Git-it yourself and review [TROUBLESHOOT.md](https://github.com/jlord/git-it/blob/master/TROUBLESHOOT.md) for common things users run into**.

---

## ようこそ、未来のForker, Brancher, そしてPull Requesterの皆様方。

これはGitとGithubを問題をとくことで学習できるアプリです。  
MacのターミナルまたはWindowsのBash上で学習を進めていきます。ホンモノのターミナルを使うことで便利なコマンドラインを覚えて、ホンモノのGitとGithubを使って学んでいきましょう。
ひととおり学習を終えたあかつきには、あなた自身のGitHubアカウントにリポジトリを作成し終えて、そして[contribution chart](https://github.com/blog/1360-introducing-contributions) に緑の四角い印がついた状態になることでしょう。

![contributions](https://raw2.github.com/jlord/git-it/master/ghcc.png)

学習していく内容を確認したい場合は、Git-itガイド内の [challenge table of contents](http://jlord.github.io/git-it) をご覧くださいませ。

---

#### Git-itをはじめるまえに…

`Git-it`を動かすためには事前準備が必要です。  
ですが、必要なものは**すべて**がタダもしくはタダだけでなくオープンソースで提供されています。

- **Git**：これであなたの作業内容を記録（track）していきます。
 - Windowsをお使いの場合は、[GitHub for Windows](http://windows.github.com)をダウンロードしましょう。  
   Gitと、ターミナルである**Git Shell**をインストールできます。
 - Macをお使いの場合は、[GitHub for Mac](http://mac.github.com)をダウンロードして下さい。  
   その後、Preferences > Advanced > Install Command Line Toolsを選択して、Gitをインストールしましょう。
- **Node.js**：`Git-it`はNode.jsで作成されているので必須です。  
  これはJavascriptをサーバで動かすためのエンジンで、バックグラウンドで動作します。あなたのコンピュータがここではその"サーバ"になるわけです。
  [ここ](http://nodejs.org/download/)からNode.jsをダウンロードして下さい。Windowsの場合は`.msi`、Macの場合は`.pkg`を選択してください。
 - すでにNodeとnpmをインストールしている場合は、バージョンが1.4.3以上であることを確認して下さい。```npm -v```のコマンドで確認できます。
- **テキストエディタ**：コードを編集するためにとても便利です。いくつか種類があるのでお好きなものを選んでください。
  [Atom](http://www.atom.io), [Sublime Text](http://www.sublimetext.com/2), [Textmate](http://macromates.com/download), [Brackets](http://brackets.io/)などがあります。
 - 実際にはGit-itを進める上で"コーディング"は行いません。なのでMac/PCにデフォルトでインストールされている「メモ帳」や「テキストエディット」でもぶっちゃけ問題ありません。

#### Git-itをインストールする

さて、上記の準備を整えたらGit-itをインストールしましょう。

- ターミナルウィンドウを開き、Git-itを"グローバルにインストール"します。グローバルにインストールすることで、どこのディレクトリにいてもGit-itを使えるようになります。  
  Node.jsに付属している[NPM](http://www.npmjs.org)を用いて、Node.jsのモジュールである`Git-it`を下記コマンドでインストールしましょう。

```bash
$ npm install -g git-it
```

- 権限不足によるエラーが出た場合は`sudo`をコマンドの先頭に追加してください：`sudo npm install -g git-it`
- `Git-it`のインストールが完了したら下記コマンドで実行できるようになっています。

```bash
$ git-it
```
- さぁ、これで準備は完了です！最初の課題を選んで、エンターキーを押してはじめましょう！

#### 学習のすすめかた

- `git-it`
- git-itが起動し、メニューが表示されたら、矢印キー（↑↓）を使って最初の問題をエンターキーで選択しましょう。
- 問題が表示されたら、画面下に表示される指示に従ってガイドを開きましょう。  
ウェブ版のガイドは[ここ](http://jlord.github.io/git-it)を参照してください。
![img](https://raw.githubusercontent.com/jlord/git-it/master/guide-ss.png)

- ガイドにある指示に従って問題を解き進めていきましょう。
- 問題が終了したら`git-it verify`とコマンドを入力・実行しましょう。
- もし問題が正しく回答されていない場合は、Git-itがどこが間違っているかを指摘し、解説してくれます。
- 問題が終わったら、`git-it`をもう一度実行して次の問題に進みましょう！

**もし何か質問がある場合は[issue](https://github.com/jlord/git-it/issues/new)を作成するか、[troubleshooting doc](https://github.com/jlord/git-it/blob/master/TROUBLESHOOT.md)をご覧ください。

---

#### 始めるためのヒント

コマンド解説では、`$ some code-stuff --here`のように、表記されています。  
先頭のドルマーク_($)_は"ユーザが入力するコマンド"という目印の意味で使用されています。  
実際にコマンドを実行する際は、`some code-stuff --here`のように、先頭にドルマークは入力しません。

コマンド解説での表記内にある、`<VARIABLENAME>`は変数を表しています。  
実際にコマンドを実行する場合は`<>`も含めて、まるごと適切な値に置き換えてください。例えば、新しいディレクトリを作成する  
`mkdir <FOLDERNAME>`というコマンドがあります。'octocat'というディレクトリを作成したい場合は  
`mkdir octocat`と入力します。

**コマンドライン**、**ターミナル**、**bash**...これらは全てMS-DOSや、ｽｰﾊﾟｰﾊｶｰが使っているような  
黒い画面に白い文字だけが表示されている画面のことです。コンピュータの操作をコマンドだけでできるとても強力なツールです。

スクリプトの実行、GitHub.comなどへのサーバ間の通信など、いろいろなことができます。
