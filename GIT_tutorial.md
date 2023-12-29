# GIT
- 版本控制系統
- 遊戲存檔功能
- 共同開發

遊戲存檔功能：可以存很多次檔，死掉後可以回到過去的存檔

# github
- 遠端的hosting
- 類似google drive
- 建立git repository
- 使用者可以下載或更新repository
- 非唯一，還有gitlen, gitlab等等，就像dropbox, onedrive等等雲端硬碟

# 如何使用git 基礎
https://www.youtube.com/watch?v=Zd5jSDRjWfA&list=PLz-S_Wd1N3svV8XnuDM6CPaTCtQkk5SY4&index=1&ab_channel=%E8%B5%B0%E6%AD%AA%E7%9A%84%E5%B7%A5%E7%A8%8B%E5%B8%ABJames

## git init
建立git repository
初始化repo

## git status
查看git repo狀態，哪些檔案是tracked，哪些檔案是untracked
只會顯示跟上一次commit不同的部分。

## git add filename
將filename檔案加入追蹤清單
類似遊戲存檔功能
把追蹤的檔案作存檔

## git add .
將當前資料夾內所有檔案加入追蹤清單
類似遊戲存檔功能
把追蹤的檔案作存檔

## git commit
會打開文字編輯器，輸入存檔說明資訊。
git add .
git commit -m "inform text"
以上兩指令要連用

## git commit -m "Information Texts"
不用打開文字編輯器。
git commit -m "Create README.md"

## git log
查看所有git commit的訊息

## git remote add <自訂名稱> <網址>
在github上新建立的repository，會產生代碼教你如何作以下事情。
將github上新建立的repository連結到本地端，
git remote add read_gemsdat https://github.com/RedhouseChen/read_gemsdat.git

## git push <git remote add 自訂名稱> <branch名稱>
將本地端已經git的資料上傳到githut等
git push read_gemsdat master
git push -u read_gemsdat master
將master的branch推送到read_gemsdat的github repo
-u：把預設的remote設成read_gemsdat(自訂名稱)，未來push時如果不指定remote都會推到read_gemsdat
那麼下一次再執行git push到read_gemsdat時，只要打
git push
即可。

## git clone <github網址>
完整下載遠端的git repo，下載之後不需要重新git init。
git clone https://github.com/RedhouseChen/read_gemsdat.git
就可以將github的read_gemsdat下載到本地端

# git 進階1
https://www.youtube.com/watch?v=TjHslMeJ81k&ab_channel=%E8%B5%B0%E6%AD%AA%E7%9A%84%E5%B7%A5%E7%A8%8B%E5%B8%ABJames

## code .
用vscode打開資料夾

## git reset
變成unstage changes
git reset -- filename
將filename這個檔案unstaged，解除git add後的staged狀態

## git checkout
變成上一次commit版本的內容，discard changes
undo last commit

git reset -- filename
git checkout -- filename

## source controls > commit > undo last commit
使用時機：commit的訊息打錯了、加的檔案錯了、等等，使用git reset
git reset --soft HEAD~1
數字1代表回到上一個commit，2代表回到上兩個commit，以此類推


# git 進階2
## git branch

## git push



