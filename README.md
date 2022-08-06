# gitTest

### 查看 git 版本
```bash
git --version
```

### 初始化數據庫
資料夾裡面會有一個隱藏的 `.git` 資料夾 (前往資料夾的終端機指令：`cd 資料夾路徑`)
```bash
git init
```

### 設定個人資料
做版本控制時，可以知道更新版本的人是誰

-   設定作者：`git config --global user.name "your name"`
-   設定作者 email：`git config --global user.email "your email"`
-   查詢 git 設定內容：`git config --list`

---
### 查看 git 的狀態
如果有新增檔案、更改檔案，git 狀態就會改變，可以用下面的指令查看 git 目前的狀態是怎樣。

```shell
git status
```

### 加入索引

`git add` 將檔案從加入索引(暫存區)。

#### 加入全部有改變的檔案到索引
```shell
git add .
```

or

#### 加入指定檔案到索引
```shell
git add <file>
```


### 加入本地數據庫 (local repository)
`git commit` 指令把暫存區的內容移至儲存庫。

```shell
git commit -m "新增/更改狀態描述"
```


### 加入遠端數據庫 (remote repository)
```shell
git remote add origin https://github.com/kkkaychen/gitTest0806.git
git branch -M main
git push -u origin main
```
