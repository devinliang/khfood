# 頁面 Page

## 實例
    <body>
    <div data-role="page">

        <div data-role="header">
            <h1>歡迎來到我的主頁</h1>
        </div>

        <div data-role="main" class="ui-content">
            <p>我現在是一個移動端開發者!!</p>
        </div>

        <div data-role="footer">
            <h1>底部文本</h1>
        </div>

    </div>
    </body>

## 實例說明：
- data-role="page" 是在瀏覽器中顯示的頁面。
- data-role="header" 是在頁面頂部創建的頁首工具列 (通常用於標題或者搜索按鈕)
- data-role="main" 定義了頁面的內容，比如文字， 圖片，表單，按鈕等。
- class="ui-content" 類用於在頁面添加內邊距和外邊距。
- data-role="footer" 用於創建頁面頁尾工具列

在這些容器中可以添加任何 HTML 元素 - 段落, 圖片, 標題, 列表等。

## 多頁面的使用

使用 jQuery Mobile, 可以在單個 HTML 文件中建立多個不同的頁面。

使用不同的href屬性來區分使用同一個唯一id的頁面：

### 實例

    <div data-role="page" id="pageone">
        <div data-role="main" class="ui-content">
            <a href="#pagetwo">跳轉到第二個頁面</a>
        </div>
    </div>

    <div data-role="page" id="pagetwo">
        <div data-role="main" class="ui-content">
            <a href="#pageone">跳轉到第一個頁面</a>
        </div>
    </div>

## 其他設定

- href="externalfile.html" 連結外部文件

## 頁面作為對話框使用

對話框是用於顯示頁面信息顯示或者表單信息的輸入。

方法一：在目的頁面中加上　data-dialog="true"　讓用戶點擊連結時彈出對話框

### 實例

    <div data-role="page" id="pageone">
        <div data-role="main" class="ui-content">
            <a href="#pagetwo">跳轉到第二個頁面</a>
        </div>
    </div>

    <div data-role="page" data-dialog="true" id="pagetwo">
        <div data-role="main" class="ui-content">
            <a href="#pageone">跳轉到第一個頁面</a>
        </div>
    </div>

方法二:在連結中加上　data-rel="dialog"　讓用戶點擊連結時彈出對話框:

### 實例

    <div data-role="page" id="pageone">
        <div data-role="main" class="ui-content">
            <a href="#pagetwo" data-rel="dialog">跳轉到第二個頁面</a>
        </div>
    </div>

    <div data-role="page" id="pagetwo">
        <div data-role="main" class="ui-content">
            <a href="#pageone">跳轉到第一個頁面</a>
        </div>
    </div>
