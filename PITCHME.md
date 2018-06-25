# GitHubTIPS
GitHubを便利に使うTIPS

---

### 自己紹介

★TODO: サクッと自己紹介

---

### 背景説明

- なんでこんなことしようとしたのか？前提踏まえて書く

★Confluenceに書いた記事からパクる

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

- ★TODO: 所感書く

---

## 裏技

---

### 【裏技1】 gist-it 既存のGitHubソースコードを埋め込み表示

[gist-it](http://gist-it.appspot.com/)

- repository上のソースコードを埋め込み表示することができる
- 外部ライブラリの調査結果とか書くときに便利

---

### 【裏技2】 issueを使って画像を楽々アップロード

通常画像をアップロードする場合、Gist or 任意のrepositoryをcloneして画像のアップロードが必要。。。めんどい

- Issues>New Issueで表示されるテキストボックスに画像をDrag&Drop  
  → サクッと画像がアップロードできる！
- 自動生成されるmarkdownタグだと画像サイズが大きい。。とかなりがち  
  → 所詮は画像URLなので、imgタグ使って埋め込んじゃえばサクッと任意のサイズにもできる

---

### おわり
