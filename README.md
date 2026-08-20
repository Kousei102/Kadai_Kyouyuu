# 手順

## 手順1
GitHubのGUIからリモートリポジトリを作成してローカルにclone
```
git clone https://github.com/Kousei102/Kadai_Kyouyuu.git
```
index.htmlにHelloと記述して作成
```
echo "Hello" >> index.html
```
addとcommitをしてmainブランチへpush
```
git add index.html
git commit -m "make index.html"
git push
```

## 手順2
開発者側でリポジトリをclone
```
git clone https://github.com/Kousei102/Kadai_Kyouyuu
```
作業ブランチを作成し、index.htmlを編集
```
cd Kadai_Kyouyuu/
git switch -c sagyou
echo "Add new line" >> index.html
```
編集内容をpush
```
git add index.html
git commit -m "手順2を実行"
git push -u origin sagyou
```
GitHubのGUI上でプルリクエストをだす
## 手順3
GitHubでプルリクエストをレビューし、mainブランチにマージ

## 手順4
ローカルのmainブランチを最新化
```
git pull
```
作業ブランチを作成
```
git switch -c sagyou2
```
index.htmlを編集
```
echo "Add new line 2" >> index.html
```
ブランチをリモートに作成
```
git push -u origin sagyou2
```
コミットを作成しプルリクエストを出す
```
git add index.html
git commit -m "手順４を実行"

gh pr create
Creating pull request for sagyou2 into main in Kousei102/Kadai_Kyouyuu

? Title (required) Add new line 2
? Body <Received>
? What's next? Submit
```
GitHubでマージ

## 手順5
開発者側のローカルブランチを最新化し、作業ブランチを作成
```
git pull
git switch -c sagyou3
```
stylesheet.cssを追加し、push
```
echo "hello" >> stylesheet.css
git add stylesheet.css
git commit -m "手順5を実行"
git push -u origin sagyou3
```
GitHubのGUI上でプルリクエストをだす

## 手順6
GitHubでプルリクエストをレビューしmainブランチにマージ
