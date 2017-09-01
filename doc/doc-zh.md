## Meta Description

如果你想設置頁面的meta description 信息，請在每篇markdown 文件的頭部添加`desc` 字段信息——更實用的方式是在scaffolds 文件夾中，將`desc` 配置到常用模板中去，示例如下：

```md
title: Lorem ipsum dolor
date: 2015-12-31 14:49:13
desc: Lorem ipsum dolor sit amet, consectetur.
---

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, non numquam saepe ex ut. Deleniti culpa inventore consectetur nam saepe!
```

生成結果:

```html
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur.">
```

如果沒有配置該信息，Hexo-theme-apollo 會使用 `page.title` 和 `page.author` 來配置該標籤。

## 標題

實際上，Hexo-theme-apollo 只支持兩種標題：`h1~h3` 大標題，`h4~h6` 小標題，也就是說，`#` 和 `###` 的樣式是一樣的。之所以這麼處理，是因為就個人感覺而言，我們不應該為文章設置過多的層級消耗讀者的閱讀精力。這相當於強制使用 Hexo-theme-apollo 的用戶在寫文章時注意文章結構，最多只能使用兩層結構。

另一個潛在的原因是因為我還沒有發現好的樣式來處理不同層級的標題，單純以大小和顏色很容易讓頁面變得混亂和冗雜。如果你有好的建議，請告訴我:)!

## 文章摘要

如果你想創建文章摘要用於向讀者展示文章的核心內容，那麼需要在文章摘要之後其他內容之前添加 HTML 註釋標籤 `<!--more-->`，使用方法如下圖所示：

![https://cloud.githubusercontent.com/assets/9530963/14064341/0fa3c754-f432-11e5-8ad7-5d063d4a0886.png](https://cloud.githubusercontent.com/assets/9530963/14064341/0fa3c754-f432-11e5-8ad7-5d063d4a0886.png)

## 評論插件

Hexo-theme-apollo 支持兩種評論插件：Disqus 和 Duoshuo. 請在 `theme/_config.yml` 文件中做如下配置:

```yaml
disqus: seansun
```

## 警告塊

使用警告塊需要 `div` 標籤和 `tip` 類名：

```html
<div class="tip">
    預處理器很強大，但它只是編寫 CSS 的輔助工具。出於對擴展和維護等方面的考慮，在大型項目中有必要使用預處理器構建 CSS；但是對於小型項目，原生的 CSS 可能是一種更好的選擇。不要肆意使用預處理器！
</div>
```

![danger](https://cloud.githubusercontent.com/assets/9530963/11359678/489a510c-92b9-11e5-9256-341cef6999b6.png)

## 圖例

也許你已經在我的博客中看到了很多圖例：流程圖、草圖……也許你想問它們是怎么生成的……實際上，它們是用Microsoft Powerpoint 製作的，可能這個答案讓你有點小失望，但是你還是應該嘗試用它製作一下圖例，你會發現它真的很適合！

## Last but not Least

專注文章內容的創作勝過博客樣式的美觀，祝各位玩的開心:) !
