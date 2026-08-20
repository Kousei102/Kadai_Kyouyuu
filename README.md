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
編集内容をpushし、プルリクエストをだす
```
git add index.html
git commit -m "手順2を実行"
git push -u origin sagyou
```
## 手順3

## 手順4

## 手順5

## 手順6
