# MarkdownとTypora

YDS 2020/11/14

## 自己紹介

名前: 大沼恭輔  @saamonumai

所属: 東京のセキュリティ会社

職種: プログラマー（Python, JavaScript）



<img src="D:\sources\yds202011\markdowns\sqGI3O1v_400x400.jpg" alt="sqGI3O1v_400x400" style="zoom: 50%;" />



## 今日話すこと

* Markdownについて
* Typoraについて
* Markdownの活用について



## Markdownとは

> Markdown（マークダウン）は、文書を記述するための軽量マークアップ言語のひとつである。本来はプレーンテキスト形式で手軽に書いた文書からHTMLを生成するために開発されたものである。
>
> -- [Markdown - Wikipedia](https://ja.wikipedia.org/wiki/Markdown)

つまり、

HTMLの様な**装飾された文章**を、**テキストデータ**で書ける言語です。



<img src="D:\sources\yds202011\markdowns\1200px-Markdown-mark.svg.png" alt="1200px-Markdown-mark.svg" style="zoom: 15%;" />





## Markdownでできる装飾、できない装飾

### 出来る 

* 見出し
* リスト、チェックボックス
* 表
* コードブロック
* 太字、斜体、横棒
* 画像埋め込み

### 出来ない

* 文字の色付け
* 多段組
* ワードアート

* マクロ



## Typoraとは

> Typora gives you a seamless experience as both a reader and a writer. It removes the preview window, mode switcher, syntax symbols of markdown source code, and all other unnecessary distractions. Instead, it provides a real live preview feature to help you concentrate on the content itself.
>
> -- https://typora.io/

↓翻訳↓

> Typoraは、リーダーとライターの両方としてシームレスなエクスペリエンスを提供します。 プレビューウィンドウ、モードスイッチャー、マークダウンソースコードの構文記号、およびその他すべての不要な注意散漫を削除します。 代わりに、コンテンツ自体に集中するのに役立つ実際のライブプレビュー機能を提供します。

つまり、



**ライブプレビューがメッチャ便利なMarkdownエディタです。**

<img src="D:\sources\yds202011\markdowns\Typora-256-logo-icon.jpg" alt="Typora-256-logo-icon" style="zoom:50%;" />

## Markdown記法: 見出し

# 見出し１

## 見出し２

### 見出し３

#### 見出し４

##### 見出し５

###### 見出し６



Markdownコード:

```mar
# 見出し１
## 見出し２
### 見出し３
#### 見出し４
##### 見出し５
###### 見出し６
```







## Markdown記法: リスト、チェックボックス

### リスト

* アイテムA
* アイテムB
* アイテムC

Markdownコード:

```mar
* アイテムA
* アイテムB
* アイテムC
```

### 番号付きリスト

1. アイテム１
2. アイテム２
3. アイテム３

Markdownコード:

```mar
1. アイテム１
2. アイテム２
3. アイテム３
```

### チェックボックス

* [x] TODO1
* [x] TODO2
* [ ] TODO3

Markdownコード:

```mar
* [x] TODO1
* [x] TODO2
* [ ] TODO3
```









## Markdown記法: 表

|  No. | Name   | Address                                 |
| -: | :-: | - |
|    1 | 天童   | 山形県天童市芳賀タウン北４丁目１−１     |
|    2 | 山形北 | 山形県山形市馬見ケ崎２丁目１２−１９     |
|    3 | 東根   | 山形県東根市さくらんぼ駅前３丁目７−１５ |



Markdownコード:

```markdown
|  ID | Name   | Address |
| -: | :-: | - |
|    1 | 天童   | 山形県天童市芳賀タウン北４丁目１−１     |
|    2 | 山形北 | 山形県山形市馬見ケ崎２丁目１２−１９     |
|    3 | 東根   | 山形県東根市さくらんぼ駅前３丁目７−１５ |
```





## Markdown記法: コードブロック

### 例1: JSON

```json
{
    "ID": 1,
    "name": "天童",
    "Address": "山形県天童市芳賀タウン北４丁目１−１"
}
```



Markdownコード:

```markdown
​```json
{
    "ID": 1,
    "name": "天童",
    "Address": "山形県天童市芳賀タウン北４丁目１−１"
}
​```
```

複数行の場合、```で囲む



### 例2: 

例: ここでコマンド`vagrant init`を実行します。



Markdownコード:

```markdown
ここでコマンド`vagrant init`を実行します。
```

改行を含まない場合、`で囲む



## Markdown記法: 太字、斜体、水平線

* **太字の例のテキスト**

* *斜体の例のテキスト / This is example of Italic text.*

* 水平線 ↓

------

Markdownコード:

```markdown
* **太字の例のテキスト**
* *斜体の例のテキスト / This is example of Italic text.*
* 水平線 ↓
------
```















## Markdown記法: 画像埋め込み

### 1. Typora上で張り付ける

（実際に操作します。）





Markdownコード:

```markdown

```



※ ローカル環境で編集時のみ反映されます。



### 2. 相対パスで参照する

<img src=".\1200px-Markdown-mark.svg.png" alt="1200px-Markdown-mark.svg" style="zoom:10%;" />



Markdownコード:

```markdown
<img src=".\1200px-Markdown-mark.svg.png" alt="1200px-Markdown-mark.svg" style="zoom:10%;" />
```



### 3. URLで参照

![1200px-Markdown-mark svg](https://user-images.githubusercontent.com/1874934/97949985-bd3d8880-1dd8-11eb-8c39-8012bea68f4e.png)

Markdownコード:

```markdown
![1200px-Markdown-mark svg](https://user-images.githubusercontent.com/1874934/97949985-bd3d8880-1dd8-11eb-8c39-8012bea68f4e.png)
```





### 4. (Github限定) PlantUML埋め込み

https://github.com/saamonumai/yds202011/issues/1#issue-734968583

※コードブロックとChrome拡張「PlantUML Viewer」の組み合わせで、Diagramを直接表示可能。



## Markdown活用例1: 資料作成

https://github.com/saamonumai/yds202011/issues/1#issue-734968583



## Markdown活用例2: API設計 

https://github.com/saamonumai/yds202011/issues/1#issuecomment-720906639

