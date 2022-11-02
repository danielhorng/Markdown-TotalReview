## 簡介

Markdown 是 **約翰·格魯伯(John Gruber)** 在2004年所創建的一種輕量級標記式語法。它允許人們使用 **純文字格式** 加上 **簡單的標記符號** 來編寫文件，然後透過 **轉譯器** 來轉換成有效的 **HTML** 文件。

{% hint style="info" %}
請參考維基百科中關於 [Markdown](<https://zh.wikipedia.org/wiki/Markdown>) 的說明。
{% endhint %}


## 簡易的範例
我們先來看一個簡單的 Markdown 語法範例：

```
+ 水果
  + 蘋果
  + 香蕉
+ 蔬菜
  + 空心菜
  + 高麗菜
```

上面的 Markdown 語法經過轉譯後的 HTML 語法為

```
<ul>
  <li>
    水果
    <ul>
      <li>
        蘋果
      </li>
      <li>
        香蕉
      </li>
    </ul>
  </li>
  <li>
    蔬菜
    <ul>
      <li>
        空心菜
      </li>
      <li>
        高麗菜
      </li>
    </ul>
  </li>
</ul>
```

顯示的結果如下：

+ 水果
  + 蘋果
  + 香蕉
+ 蔬菜
  + 空心菜
  + 高麗菜

<font color="orange">顯而易見地，Markdown 的語法比 HTML 語法要容易閱讀及撰寫。</font>

由於 Markdown 的易讀易寫特性，並且對於圖片，清單、表格都有支援，目前許多網站及各種開源系統都廣泛使用 Markdown 來撰寫說明文件或是用於論壇上發表訊息。例如： GitHub、GitBook、SourceForge...。

我們通常使用 .md 的副檔名來表示 Markdown 語法所撰寫的文件，例如：README.md。

## 標準化

由於 Markdown 語法從一開始就沒有正式的規範或標準，所以隨著時間的演進，人們為了滿足本身特定的需求，在 Markdown 的基本語法之外，各自增添一些額外的語法，也各自實作了 Markdown 語法的轉譯器。

你可以在 [babelMark III](<https://babelmark.github.io/>) 的網站上，輸入 Markdown 的語法，然後查看不同轉譯器所產生的 HTML 語法。

## 與 HTML 共存

Markdown 允許我們在文件中插入 HTML 的語法，這樣讓我們增加了許多的彈性，減少了許多 Markdown 的語法定義。例如：Markdown 並沒有關於文字顏色的語法，所以我們可以直接使用 HTML 的語法。

```
+ <font color="red">水果</font>
  + 蘋果
  + 香蕉
+ <font color="red">蔬菜</font>
  + 空心菜
  + 高麗菜
```

顯示的結果如下：

+ <font color="red">水果</font>
  + 蘋果
  + 香蕉
+ <font color="red">蔬菜</font>
  + 空心菜
  + 高麗菜

