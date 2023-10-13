# Image-Analysis for Plant Biologists with Python

## Table of Contents
- [はじめに](columns/0_introduction.md)

- プログラミング基礎
  - Python（とColaboratory）の基礎
  - 植物画像解析でよく使われるPythonコードの紹介
- 植物画像解析基礎
  - [ぶどう花粉活性度評価](notebooks/pollencounter.ipynb)
    - scikit-imageのregionpropsとWatershedを利用したオブジェクトの計数
  - [イネ種子計数形状解析（１）](notebooks/rice_seed_shape_analysis.ipynb)  *後半のmaskrcnnを分離する*
    - scikit-imageのregionpropsとWatershedを利用したオブジェクトの計数と形状解析
  - [リンゴの葉形状と遺伝的多様性の解析](notebooks/apple_leaf.ipynb)  *GWAS解析の検証とGSの追加が必要*
    - 楕円フーリエ記述子と輪郭形状解析
    - SNPを利用したPCA/GWAS/GS 解析
- 機械学習を活用した植物画像解析
  - シンプルなCNNの事例をなにか考える
  - マルバツユクサの気孔開度定量
    - HOG特徴量を利用した気孔検出
    - CNNによる気孔開閉判定
    - scikit-imageのregionpropsを利用した気孔開度定量
  - [イネ収量予測](notebooks/riceyieldcnn.ipynb)  
    - 学習済CNNモデルを利用したイネ収量推論
  - [植物病害識別診断](notebooks/plantvilllage.ipynb)
    - tensorflow.kerasを活用したCNNの学習と活用
  - [ドローン画像からの小麦穂検出モデル作成](notebooks/globalwheat2021.ipynb)
    - YOLOv8物体検出モデルの学習と推論
  - イネの種子計数形状解析（２）
    - Mask-RCNNを利用した種子インスタンス・セグメンテーション
  - 雑草検出モデルの作成
    - object detection
    - semantic segmenatation
    - instance segmenatation
  - シロイヌナズナのepidermal peel気孔開度定量
    - detectron2によるinstance segmenatation + keypoint detection
  - シロイヌナズナのleaf disc気孔開度定量
    - YOLOXによる気孔検出
    - Segmentation Modelsによる気孔開度検出
  - 機械学習モデルの解釈
  - [3D共焦点画像からの細胞壁検出と細胞インスタンス・セグメンテーション](notebooks/plantseg.ipynb)
    - PlantSegの活用
  - [U<sup>2</sup>-Net (U-Square Net)を利用した葉領域抽出](notebooks/u2netp.ipynb)
  - 葉脈解析

  

-----
  - Grad-CAM、guided backpropagationによる可視化
 
  - Segmentation
    - Weed Segmenatation (pytorch segmentationあたりを使いたい)
    - Instance Segmenatation
- 応用編2
  - [PlantSegによる細胞壁検出と細胞インスタンス・セグメンテーション3D共焦点画像解析](notebooks/plantseg.ipynb)
  


- おまけ？
  - Segment Anything
  - Grounding DINO
- 参考資料集
  - オンラインで便利なpython講座・資料まとめ
    - リンク集にするか解説をつけるかは後で考える。
    - http://mdsc.kyushu-u.ac.jp/lectures
    - https://amorphous.tf.chiba-u.jp/lecture.files/chem_computer/index.html
    - https://repository.kulib.kyoto-u.ac.jp/dspace/handle/2433/245698
    - https://utokyo-ipp.github.io/course/
    - https://cs50.jp/web/2020/python/ （動画）
      - https://cs50.jp/web/2020/python/notes/　（ノート）

### Plant Phenotyping Themesアイディア
- U-Net
- きゅうりの形状解析
  - cc by
    - https://github.com/workpiles/CUCUMBER-9
    - ![img_3.png](assets/img_3.png)
- イネ種子の割れ米分類
  - classical, svm, cnn
- 葉や果実の形状解析
  - 楕円フーリエ記述子を使ったクラスタリング、潜在空間へのマッピング
  - 
  - 
- 植物病害クラス分類 (PlantVillage)
  - CNN学習
    - keras sequential API?を使ってcnnを自分で書いてみる
    - 特徴量の可視化
- Arabidopsis leaf segmentation
  - https://zenodo.org/record/168158
  - cc by attribution
  - ![img_2.png](assets/img_2.png)
- 植物病斑物体検出（PlantDoc）
  - yolo-x
  - yolov8
- 領域分割（Arabidopsis Leaf Dataset）
  - unet
- 顕微鏡画像解析がなにか１つほしい
  - ためしげさん　気孔
    - detectron2?
- ドローンの物体検出植物
  - https://www.mdpi.com/2072-4292/12/8/1246
  - ccby4.0
  - ![img.png](assets/img.png)
- 小麦穂検出（global wheat dataset challenge）
  - ![img_1.png](assets/img_1.png)
  - LICENSEを確認
    - yolov8? 
    - kaggleの使い方
- VegAnn
  - https://www.nature.com/articles/s41597-023-02098-y
  - ccby4.0
### 応用
- 葉脈パターンのグラフ変換と種分類
  - https://www.jstage.jst.go.jp/article/jsbbs/72/1/72_21078/_article/-char/ja/

### Common Dataset Format
- COCO Format
- PASCAL VOC Format
- TFDataset

### おまけ
- u2netによる背景除去
- Foundation modelを活用したゼロショット推論
- colab以外の実装形態
  - .pyファイル
  - ウェブ形式
    - streamlit, gradio ....


    メモ
    - 