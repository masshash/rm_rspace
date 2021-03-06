# rm_rspace #
rm_rspace はテキストファイルから末尾空白を取り除きます。

![example](https://user-images.githubusercontent.com/42906988/49338917-94506e00-f66c-11e8-85d1-b67351bd3e96.png)

## 対応バージョン ##
以下のバージョンで動作を確認しました。
- Python2.7
- Python3.2+

## インストール ##
```
pip install rm_space
```

## 使い方 ##
```
rm_rspace [-d] [-c] [-e ENCODING] FILE [NEWFILE]
```
FILE に末尾空白を取り除きたいテキストファイルを指定します。元のファイルを変更したくない場合は、NEWFILE に新しい保存先を指定してください。

### オプション ###
|オプション|説明|
|---------|----|
| -h, --help                            |ヘルプメッセージを表示して終了|
| -d, --display                         |末尾空白があった行とその行番号を表示|
| -c, --count                           |末尾空白を取り除いた行の数を表示|
| -e ENCODING, <br> --encoding ENCODING |指定したエンコーディングでファイルを開く <br> 省略した場合は UTF-8 を使用| 

### 使用例 ###
```
$ rm_rspace -dc import.py
1 import os**
3 import random*
5 ***

3 行の末尾空白を取り除きました
```

## ライセンス ##
コードは MIT ライセンスのもとに公開しています。詳細は LICENSE.txt を参照してください。
