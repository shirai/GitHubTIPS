# GitHub TIPS
GitHubを便利に使うTIPS

---

### 自己紹介

![icon](https://user-images.githubusercontent.com/16277668/41948274-ebbee344-79f6-11e8-8f2a-57fe6e2bf4ee.jpg)  
白井 誠 (shirai makoto)

普段はiPhoneアプリの開発をしています。

- GitHub: [@shirai](https://github.com/shirai)
- Qiita: [@sirai](https://qiita.com/sirai)
- Twitter: [@shirai_makoto](https://twitter.com/shirai_makoto)

---

### 本日のお話

<font color="red">「GitHubを学習用ノートとして使う」</font>  

- プログラミング学習記録を残す上でGitHubは便利
- ただし学習成果の発表には不便な面が多い

そこで、  
<font color="yellow">「GitHubを使ってoutput出す」</font>  
という話をさせていただきます。

---

### 目次

1. GitHub(Gist)とConfluenceを連携  
2. 小技集
  1. 既存ソースを埋め込みjs化
  2. 画像を簡単にupload
  3. 発表用スライド作成

---

## GitHub(Gist)とConfluenceを連携

---

GitHub(Gist)とConfluenceを連携

### 目的

- Confluenceを見ればすべての情報に辿り着ける状態にしたい
- でもGitHubに上げた情報をコピペするのは嫌だ

→ Confluence上でGitのページを表示したい

---

### 手順

1. Gistにwiki情報を書く
2. gist-embedで埋め込みjsを加工する
3. ConfluenceのHTMLマクロで埋め込む

---

### Step1. [Gist](https://gist.github.com)にwikiを書く

![gist](https://user-images.githubusercontent.com/16277668/41947753-5c08d75c-79f4-11e8-8b1b-84049ca04db8.png)

- md PreviewはもちろんSyntax Highlightも効く
- 埋め込みjsを自動生成してくれる

---

### Step2. [gist-embed](http://blairvanderhoof.com/gist-embed/)でjsを加工

- Gistが生成する埋め込み用jsを加工できる
- 行数指定やfooterを消したりできるようになる  
  ※見た目気にしないならSkipしても良いです

---

### Step3. Confluenceに埋め込む

htmlマクロを使いjsを貼り付ける

![gist_to_confluence](https://user-images.githubusercontent.com/16277668/41912333-600e93b0-798a-11e8-90d2-853a8b9a42a8.png)

---

### 完成

![gist_to_confluence_2](https://user-images.githubusercontent.com/16277668/41912332-5fe91c48-798a-11e8-82dd-0181310ab774.png)

- wiki,ソースコードはGitHubにのみ存在
- Gist,Confluence両方から参照できる

GitHubへの<font color="yellow">情報の集約に成功</font>

---

## 小技集

---

### 1. [gist-it](http://gist-it.appspot.com/)で既存ソース埋め込み

![gist-it](https://user-images.githubusercontent.com/16277668/41949490-932756fc-79fc-11e8-9083-539ab41f82a6.png)

- repository上のソースコードを埋め込み可能
- 外部ライブラリの調査結果とか書くときにも便利

---

### 2. issueで画像を楽々アップロード

![issue_image_upload](https://user-images.githubusercontent.com/16277668/41948128-40502f2c-79f6-11e8-9930-ff9f2887276c.png)

- Issues>New Issueで画像をDrag&Drop  
  → サクッと画像がアップロードできる！
- Issue自体はSubmit不要

---

### 3. [PITCHME](https://gitpitch.com)でプレゼン資料を作成

1. repository作成
1. README.md を PITCHME.md にrename
1. PITCHME.md を編集
1. https://gitpitch.com/$userName/$repoName  

ブラウザだけで簡単にスライドが作れちゃう！ 

今回のスライドもこれで作ってます  
[URL](https://gitpitch.com/shirai/GitHubTIPS)　　　[ソース](https://raw.githubusercontent.com/shirai/GitHubTIPS/master/PITCHME.md)

---

### おわり

アウトプットを楽に続けていくためにも、  
便利なものをより便利に使いたい

まだまだ便利な使い方模索しています！

---

おまけ: 参考サイト

- [【gist-it】githubのソースコードをサイトに埋め込む方法 - プログラミング雑記](https://algorithm.joho.info/programming/gist-it-github-soucecode-website/)
- [GitHub の Wiki に画像を貼り付ける一番簡単な方法（Wiki リポジトリを clone しないバージョン） - akiyoko blog](http://akiyoko.hatenablog.jp/entry/2016/08/30/051708)
- [GitHubだけで超高機能なスライド資料が作れる「GitPitch」の使い方を徹底解説！ - paiza開発日誌](https://paiza.hatenablog.com/entry/2017/06/22/GitHubだけで超高機能なスライド資料が作れる「GitPitch」の)
- [GitPitch Embed Provider | Embedly](https://embed.ly/provider/gitpitch)
