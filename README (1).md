# 左右反転画像 生成プログラム flip.py

## 1.概要
引数で指定した画像の左右反転画像を作成するpython3で動作するプログラムです。

## 2.ソースコード
```python
#　このプログラムは python3用です。
#　あらかじめ pip install pillow で pillow をインストールしておきます。
from PIL import Image
import sys

#コマンドライン引数から入力画像と出力画像のファイル名を取得
input_image = sys.argv[1]
output_image = sys.argv[2]

# 画像の読み込み
ing = Image.open(Image.FLIP_LEFT_RIGHT)

# 画像の保存
img_flip.save(output_image)
#左右反転画像 生成プログラム flip.py
```

## 3.使い方
### 3.1.実行例
- コマンドラインフォーマット

```
python3 flip.py <imput_image_path><output_image_path>
```
- 利用例

```
python3 flip.py input.jpg output.jpg
```

### 3.2.出力結果
- 以下のように入力画像の左右反転画像が表示されます。

| 入力画像(input.jpg) | 出力画像(output.jpg) |
| --- | --- |
| <img width="640" height="468" alt="input" src="https://github.com/user-attachments/assets/fae86e31-3620-4317-996e-fe71098dd9f4" /> | <img width="640" height="468" alt="output" src="https://github.com/user-attachments/assets/3b246859-bbf0-4e53-a894-3f7e0b61103a" /> |

以上
