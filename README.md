# GitHub Quest - 冒険者のためのGit & GitHub入門

## ようこそ！GitとGitHubの冒険の世界へ！

勇者よ、今日から君はGitHubの世界で冒険を始めるんだ！  
目的は「プルリクエスト」という最終ボスを倒して、みんなで仲良くプロジェクトを進めること！  
さあ、君の冒険が今始まる！

## 冒険のマップ

1. **冒険の準備** - Gitの初期設定をしよう
2. **VSCodeの世界へ** - リポジトリをクローンしてみよう
3. **分岐点の選択** - 新しいブランチを作って、自分だけの冒険を始めよう
4. **発見した宝物** - コードを編集して保存しよう
5. **報告の石版** - コミットして、変更内容を伝えよう
6. **勇者の掲示板** - プルリクエストで仲間に報告しよう

---

## 1. 冒険の準備：Gitの初期設定

冒険に出る前に、君の名前と魔法（メールアドレス）を設定しよう。これは君の行動が記録されるために必要な儀式だ。

### 呪文（コマンド）：

```bash
# 勇者の名前とメールアドレスを設定
git config --global user.name "your-name"
git config --global user.email "your-email@example.com"
```

---

## 2. VSCodeの世界へ：リポジトリをクローンしよう

さあ、いよいよ冒険の地図（リポジトリ）を手に入れる時が来た！VSCodeを使って、みんなで冒険するための場所を準備しよう。

手順：

- VSCodeを開く
- サイドバーにあるソース管理アイコンをクリック
- 「リポジトリをクローン」ボタンを押して、君のGitHubリポジトリのURLを入力しよう  
  URL: `https://github.com/airu3/git-lecture.git`
- クローン先のフォルダを選択して、冒険をスタート！

### 呪文（コマンド）：

```bash
https://github.com/airu3/git-lecture.git
```

出力:

```bash
リポジトリ 'https://github.com/airu3/git-lecture.git' をクローンしています...
完了しました。
```

## 3. 分岐点の選択：新しいブランチを作ってみよう

冒険者は自分だけの道を進むべきだ！「ブランチ」という分かれ道を作って、他の勇者に迷惑をかけないようにしよう。

### 手順：

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
- 編集が終わったら、保存（Ctrl+S）を忘れずに！

---

## 5. 報告の石版：コミットしよう

発見した宝物をみんなに知らせるために、魔法の石版「コミット」を使う必要がある。この石版に自分の発見を書き込んで報告しよう。

### 手順：

- VSCodeのソース管理タブを開く
- 編集したファイルがリストアップされているはずだ。「+」ボタンで変更をステージする
- 下のメッセージ欄に、君の発見を簡単に説明しよう  
  例: `"イントロダクションを追加しました"`
- 「✓」ボタンを押してコミット完了！

### 出力:

```bash
変更がステージされました。
コミットメッセージ: "イントロダクションを追加しました"
```

## 6. 勇者の掲示板：プルリクエストを作成しよう

さあ、いよいよ君の冒険も終盤だ！最後に仲間に君の成果を伝える「プルリクエスト」を作成しよう。

### 手順：

- VSCodeからGitHubにプッシュしよう
- 画面下の通知から「リモートリポジトリにプッシュしますか？」をクリック
- 「はい」を選択してリモートに送る

### 出力:

```bash
変更を 'origin' にプッシュしました。
```

次に、GitHubに戻って、「Pull Requests」タブから「New Pull Request」をクリックし、君の冒険の報告書を簡単に書いてプルリクエストを作成しよう！
