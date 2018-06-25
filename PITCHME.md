# GitHub TIPS
GitHubを便利に使うTIPS

---

### 自己紹介

白井 誠  
(shirai makoto)

普段はiPhoneアプリを作成しています。

- GitHub: @shirai
- Qiita: @sirai
- Twitter: @shirai_makoto

---

### 背景説明

- なんでこんなことしようとしたのか？ | 

- iPhoneアプリエンジニアの育成カリキュラムも作成してます | 

- アウトプットの場は基本的にConfluence(社内限定公開)
- 成果物自体はpublicな情報で一般にも公開している(GitHub public repo) |

ConfluenceにもGitHubにも書かないといけない、というのが  
<font color="red">非常にめんどくさい</font>

---

### やりたいこと

全ての情報をGitHubで一元管理

---

## 実践

---

### Step1. Gistにwikiを書く

- 埋め込みHTMLを自動生成してくれる
- privateなページが作れる  
  ※URLさえ知ってれば誰でもアクセスできちゃうけど

---

### Step2. gist-embed で表示方法を加工する

[gist-embed](http://blairvanderhoof.com/gist-embed/)

- Gistが生成する埋め込みHTMLだと見た目を自由に変えられない
- 行数指定やfooterを消したりできるようになる

---

### Step3. Confluenceに埋め込む

htmlマクロを使って生成したjsスクリプトを貼り付ける

★TODO: image貼る

---

## 裏技

---

### 【裏技1】 gist-it 既存のGitHubソースコードを埋め込み表示

[gist-it](http://gist-it.appspot.com/)

- repository上のソースコードを埋め込み表示することができる
- 外部ライブラリの調査結果とか書くときに便利

---

### 【裏技2】 issueを使って画像を楽々アップロード

- Issues>New Issueで表示されるテキストボックスに画像をDrag&Drop
  - サクッと画像がアップロードできる！

※所詮は画像URLなので、imgタグ使って埋め込んじゃえばサクッと任意のサイズにもできる

---

### 【裏技3】 スライドを作成

1. repository作成
2. README.md を PITCHME.mdにリネーム
3. https://gitpitch.com/{ユーザー名}/{リポジトリ名} にアクセス

これだけでスライドが作れちゃう！使うのはブラウザとGitHubアカウントのみ！  
あとはよしなに [PITCHME.md](https://github.com/shirai/GitHubTIPS/blob/master/PITCHME.md) を編集すればOK

今回のスライドもこれで作ってます  
https://gitpitch.com/shirai/GitHubTIPS

---

### おわり

アウトプットを楽に続けていくためにも、便利なものをより便利に使いたい

まだまだ便利な使い方模索しています！


---

おまけ: 参考サイト

- [【gist-it】githubのソースコードをサイトに埋め込む方法 - プログラミング雑記](https://algorithm.joho.info/programming/gist-it-github-soucecode-website/)
- [GitHub の Wiki に画像を貼り付ける一番簡単な方法（Wiki リポジトリを clone しないバージョン） - akiyoko blog](http://akiyoko.hatenablog.jp/entry/2016/08/30/051708)
- [GitHubだけで超高機能なスライド資料が作れる「GitPitch」の使い方を徹底解説！ - paiza開発日誌](https://paiza.hatenablog.com/entry/2017/06/22/GitHubだけで超高機能なスライド資料が作れる「GitPitch」の)
