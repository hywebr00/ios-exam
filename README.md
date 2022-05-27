# 凌網科技有限公司研究發事業處：資深 iOS 工程師徵才考題 🚀

我們是台灣圖書館電子書第一品牌HyRead的研發團隊，歡迎有自信、對軟體開發充滿熱情的夥伴加入，一同發掘數位閱讀的無限可能。

## 1. 流程

1. 請自行一個建立 **XCode** 專案
2. 這裡有一個基礎 [Figma](https://www.figma.com/file/4aAUNkjFEd8q5RF1zbzCrI/HyRead?node-id=0%3A1) 設計稿 👋
3. 請您盡可能的建立一個**好的架構**、**乾淨的代碼** ✨
4. **實作服務請求**👇拿到『所有書籍』的資料 📕
5. 必須要有**離線顯示**的功能 ✔️
6. 必須要有可以**收藏**與**取消收藏**的功能 ❤️
7. 將您完成好的專案上傳至您個人的 **Github**
8. **郵件**您的**存儲庫 (Repository)** 至 HR: *wendy@hyweb.com.tw*
9. 符合標準將會同知您來進行**面試**
10. 其他問題可詢問公司 **HR 李小姐: (02)2395-6966 #3128**

<br>

> **額外加分**
> 1. 如果您有比基礎設計稿更好的**創意**來呈現**視覺**或者**使用者體驗** 加分 👍
> 2. **響應式程式設計** 加分 👍
> 3. 使用者**資料安全保護** 加分 👍
> 4. 盡可能地將**您會的技術展實作出來** 加分 👍

<br>

## 2. 服務串接

- **URL:**
    **`GET`**  https://mservice.ebook.hyread.com.tw/exam/user-list

- **Request:**
    | header|  value|
    |:--:|:--:|
    |Content-type| application/json|

- **Response:**
    | 欄位|  說明|
    |:-----:|:-----:|
    |uuid |  唯一碼 |
    |coverUrl |  書封圖片 |
    |publishDate |  出版日期 |
    |publisher |  出版社 |
    |author |  作者 |

```json
[
  {
    "uuid": 0,
    "title": "藍色時期. 7",
    "coverUrl": "https://webcdn2.ebook.hyread.com.tw/bookcover/270374978957267916620215022111051.jpg",
    "publishDate": "2021[民110]",
    "publisher": "東立出版社",
    "author": "山口飛翔 著"
  },
  {
    "uuid": 1,
    "title": "[試讀本] 熾熱之夢",
    "coverUrl": "https://webcdn2.ebook.hyread.com.tw/bookcover/278194978986319625920223411010153.jpg",
    "publishDate": "2022[民111]",
    "publisher": "蓋亞文化",
    "author": "喬治.馬汀著;章澤儀譯"
  },
  /// 省略
]
```