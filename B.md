## 手順5
開発者側のローカルブランチを最新化し、作業ブランチを作成
```
git pull
git switch -c sagyou3
```
stylesheet.cssを追加してAへプルリクエストを出す
```
echo "hello" >> stylesheet.css
git add stylesheet.css
git commit -m "手順5を実行"
git push -u origin sagyou3
```
