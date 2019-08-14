## 準備
```bash
sudo gem install asciidoctor asciidoctor-diagram
npm install -g mermaid.cli
```

## エディタ
`VSCode`
- https://marketplace.visualstudio.com/items?itemName=joaompinto.asciidoctor-vscode


## 設定
~/Library/Application Support/Code/User/settings.json
```json
"asciidoc.use_asciidoctor_js": false,
"asciidoc.asciidoctor_command": "asciidoctor -a env-vscode -a outdir=.adoc -a imagesdir=.adoc -a imagesoutdir=.adoc -r asciidoctor-diagram -o-",
```

## ビルド
```bash
# 1ファイルのみ
# パスも適切ではない
asciidoctor -a env-html -a outdir=.adoc -a imagesdir=.adoc -a imagesoutdir=.adoc -r asciidoctor-diagram my_dif/my.adoc
```


<!-- https://qiita.com/gho4d76g/items/302e1ff91754b9b50f34 -->
