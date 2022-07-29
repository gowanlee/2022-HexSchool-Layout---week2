# 2022-HexSchool-Layout---week2
2022 六角切版直播班 - 第二週

本週學習重點：

<b>1. dislpay:flex 要放在上一層才有效果</b>

  - 決定軸線：flex-direction (互動詢問)
    - row (預設)
    - row-reverse
    - column
    - column-reverse
  
  - 主軸對齊：justify-content (開始代入範例)
    - flex-start (預設)
    - center
    - flex-end
    - space-between
    - space-around
    - space-evenly
  
  - 換行屬性：flex-wrap
    - nowrap(預設)
    - wrap
  
  - 交錯軸單行對齊：align-item
    - flex-start
    - center
    - flex-end
    - stretch(預設)
    - baseline

  - 交錯軸多行對齊屬性：align-content

<b>2. 在區塊元素載入圖片可以用 background</b>
 
  - background-image    //背景圖片 
  - background-color    //背景顏色
  - background-repeat   //背景重複顯示 repeat-x repeat-y no-repeat
  - background-size     //背景覆蓋 cover contain 
  - background-position //背景位置 左右 上下

<b>3. 圖片取代文字</b>
  
  - text-indent: 101%;
  - overflow: hidden;
  - white-space: nowrap;
  
<b>4. 利用偽元素在ul>li畫出圓點</b>
<img width="444" alt="截圖 2022-07-28 下午9 45 47" src="https://user-images.githubusercontent.com/106324011/181520865-d103b64e-fb78-4531-8575-0131e74380e1.png">


---------------------------------------------------


下方提供關於作業細節的建議：

1. scss 檔案拆分的部分，_layout.scss 中這部分可以拉出來命名為 _variables.scss，且符合 layout 會是每一頁都會有的樣式（例如：header、footer）因此建議這邊的樣式可以合併回去 _main.scss。（可以參考這篇文章）

2. scss 可以善用 & 連接符號來減少巢狀階層層數。

<!-- .my-brand{
  ＆-pic {}
} -->

<!-- // 編譯後
.my-brand{}
.my-brand-pic{} -->

3. .header 有使用 flex 排版就不需要再設置 container 了。

4.「About」、「Contact」也不需要再設置 container，且不需要 section 中的 flex 排版，皆可改用 text-align: center 即可。

5.「Other Works」區塊的作品名稱可以改為 h3 標籤，善用標題標籤設置重點內容，能有效提升 SEO。
