# GitHub TIPS
GitHubを便利に使うTIPS

---

### 自己紹介

白井 誠  
(shirai makoto)

普段はiPhoneアプリの開発をしています。

- GitHub: [@shirai](https://github.com/shirai)
- Qiita: [@sirai](https://qiita.com/sirai)
- Twitter: [@shirai_makoto](https://twitter.com/shirai_makoto)

---

### 本日のお話

<font color="red">「GitHubを学習用ノートとして使う」</font>  
という話をする予定でしたが、

- 背景説明をするのに時間がかかる
- さほど面白い背景でもない

ということでそのへんの説明を省き、  
<font color="blue">「GitHubを便利に利用した話」</font>  
を中心にお話します。

---

### 目次

1. GitHub(Gist)とConfluenceを連携  
2. 小技集
  1. 既存ソースを埋め込みHTML化
  2. 画像を簡単にupload
  3. 発表用スライド作成

---

## GitHub(Gist)とConfluenceを連携

---

GitHub(Gist)とConfluenceを連携

### 目的

- 育成コンテンツ用のサンプルコードはGitHub
- 育成コンテンツの説明＆展開方法はConfluence

情報を一箇所にまとめたかった

---

GitHub(Gist)とConfluenceを連携

### 手順

1. Gistにwiki情報を書く
2. gist-embedで埋め込みHTMLを加工する

---

### Step1. [Gist](https://gist.github.com)にwikiを書く

- 埋め込みHTMLを自動生成してくれる
- privateなページが作れる  
  ※URLさえ知ってれば誰でもアクセスできちゃうけど

---

### Step2. [gist-embed](http://blairvanderhoof.com/gist-embed/)で埋め込みHTMLを加工する

- Gistが生成する埋め込み用jsを加工できる
- 行数指定やfooterを消したりできるようになる  
  ※見た目気にしないならSKIPしても良いです

---

### Step3. Confluenceに埋め込む

htmlマクロ機能を使って  
生成したjsを貼り付ける

![gist_to_confluence](https://user-images.githubusercontent.com/16277668/41912333-600e93b0-798a-11e8-90d2-853a8b9a42a8.png)

---

### 完成

![gist_to_confluence_2](https://user-images.githubusercontent.com/16277668/41912332-5fe91c48-798a-11e8-82dd-0181310ab774.png)

- wiki,ソースコードはGistにのみ存在
- Gist,Confluence両方から参照できる

<font color="blue">使い勝手を変えずに、情報の集約に成功</font>

---

## 小技集

---

### 【小技1】既存のソースコードからjs自動生成

[gist-it](http://gist-it.appspot.com/)を利用

- repository上のソースコードを埋め込み表示することができる  
  Gistへのコピペ不要！
- 外部ライブラリの調査結果とか書くときにも便利

---

### 【小技2】 issueを使って画像を楽々アップロード

- Issues>New Issueで表示されるテキストボックスに画像をDrag&Drop
  - サクッと画像がアップロードできる！
- Issue自体はSubmit不要

---

### 【小技3】 スライドを作成

1. repository作成
1. README.md を PITCHME.md にrename
1. PITCHME.md を編集
1. https://gitpitch.com/$userName/$repoName にアクセス  

ブラウザだけで簡単にスライドが作れちゃう！ 

今回のスライドもこれで作ってます  
[URL](https://gitpitch.com/shirai/GitHubTIPS) [ソース](https://github.com/shirai/GitHubTIPS/blob/master/PITCHME.md)

---

### おわり

アウトプットを楽に続けていくためにも、便利なものをより便利に使いたい

まだまだ便利な使い方模索しています！

---

おまけ: 参考サイト

- [【gist-it】githubのソースコードをサイトに埋め込む方法 - プログラミング雑記](https://algorithm.joho.info/programming/gist-it-github-soucecode-website/)
- [GitHub の Wiki に画像を貼り付ける一番簡単な方法（Wiki リポジトリを clone しないバージョン） - akiyoko blog](http://akiyoko.hatenablog.jp/entry/2016/08/30/051708)
- [GitHubだけで超高機能なスライド資料が作れる「GitPitch」の使い方を徹底解説！ - paiza開発日誌](https://paiza.hatenablog.com/entry/2017/06/22/GitHubだけで超高機能なスライド資料が作れる「GitPitch」の)
