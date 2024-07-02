# Super-resolution
機械学習による超解像化に関する知見や技術を保管するレポジトリ

# SRCNN
超解像にDLとしてCNNを活用したもの。<br/>
### コード
[SRCNN.ipynb](https://github.com/cielcs/Super-resolution/blob/main/SRCNN.ipynb "SRCNN.ipynb")<br/>
<br/>
### 手順
1. 低解像度の画像を画像補完アルゴリズムにより拡大する
2. モデルの構造は入力層、畳み込み層、残差ブロック、アップサンプリング
3. 損失関数は平均二乗誤差を採用

### モデルの構造
go to [SRCNN.ipynb](https://github.com/cielcs/Super-resolution/blob/main/SRCNN.ipynb "SRCNN.ipynb")

### 補足
最初に画像を拡大する際の補完方法に有名なアルゴリズムとして以下のものがある。<br/>
今回はbilinearを採用した。
- 最近傍補完（Nearest neighbor)
- 双一次補完（Bilinear)
- 双三次補完（Bicubic)
### 参考
- https://arxiv.org/pdf/1501.00092
- https://qiita.com/PingpongChopper/items/cca7d95a16c522746130
- https://qiita.com/ratorato/items/7c2ee6c87d7707a733c1

# メモ
NVIDIAのRTX VSがすごそう。https://blogs.nvidia.co.jp/2023/03/10/rtx-video-super-resolution/
