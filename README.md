# GitHub Quest - 冒険者のためのGit & GitHub入門 for VScode

## ようこそ！GitとGitHubの冒険の世界へ！

勇者よ、今日から君はGitHubの世界で冒険を始めるんだ！  
目的は「プルリクエスト」という最終ボスを倒して、みんなで仲良くプロジェクトを進めること！  
さあ、君の冒険が今始まる！

## 参考文献
突貫工事で作り始めました。
でも疲れました。
ありがとうございました。

多分情報不足です。
わからないところは以下のサイトを横断しながら調べてほしいです。
ごめんなさい。

- [VSCodeでGit・GitHubを使う方法を解説する【初心者向き】](https://miyashimo-studio.jp/blog/detail/vscode-github/)
- [vscode初回起動の時のgit使い方](https://zenn.dev/kd_gamegikenblg/articles/b220e23b0b7ef9#%E4%BD%BF%E3%81%84%E6%96%B9)
- [プル→コミット→プッシュの基本的な流れ](https://zenn.dev/ojk/books/github-vscode/viewer/pull-push)
- [編集&コミット](https://zenn.dev/ojk/books/github-vscode/viewer/vscode-git#%E7%B7%A8%E9%9B%86%EF%BC%86%E3%82%B3%E3%83%9F%E3%83%83%E3%83%88)
- [プッシュ（とアプリ連携）](https://zenn.dev/ojk/books/github-vscode/viewer/vscode-git#%E3%83%97%E3%83%83%E3%82%B7%E3%83%A5%EF%BC%88%E3%81%A8%E3%82%A2%E3%83%97%E3%83%AA%E9%80%A3%E6%90%BA%EF%BC%89)


## 冒険のマップ

0. **世界観** - コードの冒険が始まる
1. **冒険の準備** - Gitの初期設定をしよう
2. **VSCodeの世界へ** - リポジトリをクローンしてみよう
3. **分岐点の選択** - 新しいブランチを作って、自分だけの冒険を始めよう
4. **発見した宝物** - コードを編集して保存しよう
5. **報告の石版** - コミットして、変更内容を伝えよう
6. **勇者の掲示板** - プルリクエストで仲間に報告しよう

---


---

# 1章: 冒険の準備 〜GitとVSCodeのインストールと初期設定〜

君がコードの大陸を冒険するために、まずは2つの重要なアイテム「Git」と「VSCode」を手に入れる必要がある。この2つは、冒険をスムーズに進めるために欠かせない道具だ。さあ、準備を整えて冒険の第一歩を踏み出そう！

## すでにインストール済みの場合
もしすでにGitとVSCodeがインストールされているなら、初期設定（名前とメールアドレスの登録）だけを行っておこう。あとは、君の準備は万全だ！

## 1.1 Gitのインストール
Gitは、君のコードのバージョンを管理してくれる強力なツールだ。過去に戻ったり、仲間と一緒にコードを作るときにも大いに役立つぞ。もしまだインストールしていない場合は、以下の手順を参考にしてね。

### 手順
1. **Gitの公式サイトにアクセスする**  
   まず、Gitの公式ダウンロードページに行こう。以下のリンクからアクセスできるよ。  
   [Git公式ダウンロードページ](https://git-scm.com/downloads)

2. **自分のOSに合ったバージョンをダウンロード**  
   ページにアクセスしたら、自分のOS（Windows、Mac、Linux）に合ったバージョンをダウンロードしよう。

3. **インストーラーを実行してインストール**  
   ダウンロードが完了したら、インストーラーを開いて、画面の指示に従ってインストールを進めていこう。基本的にはデフォルト設定で問題ないよ。

### Windowsの注意点
インストール時に「Git Bash」も一緒にインストールされるけど、これを選んでおくことを忘れないでね。後で便利に使えるよ！

---

## 1.2 VSCodeのインストール
VSCode（Visual Studio Code）は、冒険に欠かせないもう一つの道具。これはコードを書くためのエディターで、Gitとの連携も非常にスムーズにできる魔法のツールだ。

### 手順
1. **VSCodeの公式サイトにアクセスする**  
   [VSCode公式ダウンロードページ](https://code.visualstudio.com/)に行こう。

2. **自分のOSに合ったバージョンをダウンロード**  
   自分のOSに合ったリンクが表示されるので、クリックしてダウンロードしよう。

3. **インストーラーを実行してインストール**  
   ダウンロードが完了したら、インストーラーを開いてインストールしよう。これもデフォルト設定で進めてOKだよ。

---

## 1.3 Gitの初期設定（名前とメールアドレスの設定）
道具が揃ったら、冒険者としての君の名前とメールアドレスを設定しよう。これで、君の冒険の記録がきちんと保存されるようになるんだ。

### ターミナルを使って設定
VSCodeには「ターミナル」という便利な機能があるから、そこから設定をしていくよ。

### 手順
1. **VSCodeを起動してターミナルを開く**  
   VSCodeを開いて、上のメニューから「View（表示）」→「Terminal」をクリックしよう。
   ![image](https://github.com/user-attachments/assets/c6ede61e-9b1e-43e2-bc5f-9ae1c87697dc)

3. **Windowsの場合：ターミナルをGit Bashに切り替える**  
   Windowsを使っている場合、デフォルトで「Powershell」が表示されるけど、これを「Git Bash」に切り替えるんだ。ターミナル内の「Powershell」と書かれた部分の右側の▼をクリックして、「Git Bash」を選ぼう。
   ![image](https://github.com/user-attachments/assets/b7680386-eb25-4497-936d-106721cf4c19)
   ![image](https://github.com/user-attachments/assets/2e847e64-9824-4f76-a741-7b7855e8dece)

   *MacのユーザーはそのままでOKだよ。*

5. **名前とメールアドレスの設定**  
   次に、以下の呪文（コマンド）をターミナルに打ち込んで、君の名前とメールアドレスをGitに登録しよう。

```bash
# 勇者の名前とメールアドレスを設定
git config --global user.name "君の名前"
git config --global user.email "君のメールアドレス"
```

例：
```bash
# 勇者の名前とメールアドレスを設定
git config --global user.name "Taro Yamada"
git config --global user.email "taro.yamada@example.com"
```

これで、君が行った変更がしっかり記録されるようになるよ。もう道具は揃った！これで準備は完了だ。さあ、次の章で実際の冒険（プロジェクト）を始めよう！

---

## 2. VSCodeの世界へ：リポジトリをクローンしよう

さあ、いよいよ冒険の地図（リポジトリ）を手に入れる時が来た！VSCodeを使って、みんなで冒険するための場所を準備しよう。

手順：
### 【初回起動の場合】VSCode管理画面上でのクローンの場所
VSCodeの画面で、ソース管理を選択します。左のリポジトリのクローンをクリックします。
![image](https://github.com/user-attachments/assets/6c7d2baa-3d3c-4f7f-b786-a4e0b5b2fd1d)
画面上部にURLを貼り付ける枠が出てくるので、先ほどコピーしたものを貼り付けて、EnterもしくはリポジトリのURL git@github.com:ユーザー名/RepositoryForVSCode.gitをクリックします。
![image](https://github.com/user-attachments/assets/3b730c19-7fd0-41ed-bdbc-6416361125e7)

---

### 【起動2回目以降】VSCode管理画面上でのクローンの場所　
クローンしたいリモートリポジトリのURLを入力する欄が表示されます。クローン先リモートリポジトリのURLをこの欄に張り付け、「Enter」を押して下さい。
- VSCodeを開く
- サイドバーにあるソース管理アイコンをクリック
- VSCode管理画面左上の「…」→「クローン」の順でクリックして、GitHubリポジトリのURLを入力しよう
  ```bash
  https://github.com/airu3/git-lecture.git
  ```
  
![image](https://github.com/user-attachments/assets/99c5f0d2-a218-4f3b-b928-00ed6197ba3e)

### 共通 クローン先のフォルダを選択して、冒険をスタート！
  そうすると、「リモートリポジトリの宛先」とするローカルのフォルダを選択するよう指示されます。
  任意のフォルダを選んで「リポジトリの宛先として選択」をクリックして下さい。
![image](https://github.com/user-attachments/assets/c7d66163-f1c1-4e07-920e-ead5e95a2e4a)

![image](https://github.com/user-attachments/assets/778296f0-47a4-4a2c-8d16-6fd2860e8432)
  **この記事を作った人は`I:\code\web`ディレクトリに保存しています。**
  
## 3. 分岐点の選択：新しいブランチを作ってみよう

冒険者は自分だけの道を進むべきだ！「ブランチ」という分かれ道を作って、他の勇者に迷惑をかけないようにしよう。
![image](https://github.com/user-attachments/assets/29545529-7200-416e-b57b-74edd0b995d9)

ブランチとは開発中のソースコードに影響を与えずに、新しく作成したブランチ側で開発作業を続けられる機能です。
新しいブランチ側の作業が完了した際には、メインのブランチへ修正内容を反映（マージ）させます。
ブランチは複数人で共同開発をする際に、よく使われる機能なので覚えておきましょう。

### 手順：
VSCodeでブランチを作成する場合、メインのブランチを開いた状態で画面左下のブランチアイコンをクリックして下さい。
そうすると画面右上にブランチの作成画面が表示されるので、任意のブランチ名を入力し「新しいブランチの作成」をクリックします。
（ここでは参考までにブランチ名を「test_branch」とします。）
![image](https://github.com/user-attachments/assets/8089cae2-d207-4a8d-96dc-50727bcd325f)

- VSCodeで、画面左下の「ブランチ」名をクリック
- 「新しいブランチを作成」ボタンを押して、新しいブランチを作成しよう  
  例: `feature/add-introduction`

### 出力:

```bash
ブランチ 'feature/add-introduction' を作成しました。
```

## 4. 発見した宝物：コードを編集して保存しよう

ここまで来た君は、何か新しい宝物（コード）を見つけるはずだ！勇気を出して、少しだけ手を加えてみよう。

### 手順：

- VSCodeでファイルを開いて、コードを編集
- エクスプローラーで新しいファイルを選択します。
![image](https://github.com/user-attachments/assets/ec393d26-8373-45a9-9a59-f0e71fe29e19)

- 編集が終わったら、保存（Ctrl+S）を忘れずに！
![image](https://github.com/user-attachments/assets/d5e53539-95ab-4644-8406-046d56bf672a)

---

## 5. 報告の石版：コミットしよう

発見した宝物をみんなに知らせるために、魔法の石版「コミット」を使う必要がある。この石版に自分の発見を書き込んで報告しよう。

### 手順：

- VSCodeのソース管理タブを開く
- 編集したファイルがリストアップされているはずだ。「+」ボタンで変更をステージする
- 下のメッセージ欄に、君の発見を簡単に説明しよう  
  例: `"イントロダクションを追加しました"`
- 「✓」ボタンを押してコミット完了！

- 編集が終わったら、ソース管理の項目に通知アイコンみたいなものが表示されています。これは変更があった場合のファイルの数を表しています。
![image](https://github.com/user-attachments/assets/31502f2c-035c-48e4-8969-8f1d72bf6a9f)

- 変更の下にあるファイルをクリックすると、前回との差分が表示されます。今回は新しく追加したので、赤い部分(前回の部分)には何も表示されていません。またファイルをマウスオーバーすると横に出てくるアイコンは、それぞれファイルを開く 変更を破棄 変更をステージとなっています。
![image](https://github.com/user-attachments/assets/27b38ea6-a02a-4c46-a692-0724c5ce86ac)

- ファイルをアップロードするためには、変更をステージをクリックします。そして、コメントを書き、コミットをクリックします。このコミットは、ローカルに保存しただけなので、最後にGitHubにアップロードする作業が必要です。
ソース管理の右にある三点リーダーをクリックし、プッシュを選択することでアップロードが完了となります。
![image](https://github.com/user-attachments/assets/cc8757ee-3224-49bd-90ce-8ef844288d3f)

- GitHubの方でも確認してみると、アップロードされているのが確認できると思います。
![image](https://github.com/user-attachments/assets/45586792-c177-4482-91c7-be9fd4f5a286)

## 6. 勇者の掲示板：プルリクエストを作成しよう
さあ、いよいよ君の冒険も終盤だ！最後に仲間に君の成果を伝える「プルリクエスト」を作成しよう。

### 手順：

- VSCodeからGitHubにプッシュしよう
- 画面下の通知から「リモートリポジトリにプッシュしますか？」をクリック
- 「はい」を選択してリモートに送る

次に、GitHubに戻って、「Pull Requests」タブから「New Pull Request」をクリックし、君の冒険の報告書を簡単に書いてプルリクエストを作成しよう！
