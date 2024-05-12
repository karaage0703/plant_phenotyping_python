# Plant Phenotyping for Biologists with Python

Python言語で学ぶ植物画像解析（生物学者向け）

![title_image](assets/_30b8ab64-b43d-455a-8a6f-ee7b8263def7.jpeg)

## [はじめに](columns/introduction.md)

## Column

### [なんでもかんでもAIっていうんじゃない](columns/using_the_term_AI.md)

### [エラーは怖くない：自分で解決できるようになろう](columns/error.md)

### [ファイルとフォルダの命名方法](columns/file_name.md)

### [Pythonの命名規則](columns/styleguide.md)

### [座標系と表記順序：xyなのかyxなのか、nhwcなのかnchwなのか。](columns/xyyxrc.md)

### [「レナ」を超えて](columns/lenna.md)

### [機械学習におけるデータセットのフォーマット](columns/dataset_format.md)

### [データリーク](columns/dataleak.md)

### [巨人の肩での研究: ソフトウェアライセンスについて](columns/license_rules.md)

---

## Part 1: Image Analysis Basics for Plant Phenotyping

### [割米判定アルゴリズムの作成](notebooks/rice_proper_broken.ipynb)

* 画像解析基礎とコメ面積定量
* 最適な閾値の定義

### [シロイヌナズナの葉面積定量と生育モデル作成](notebooks/time_series_growth.ipynb)

* HSV閾値による葉面積定量
* 時系列データの作図
* 生育モデルの作成

### [キュウリの茎径と環境データ分析](notebooks/env_data_analysis.ipynb)

* pandasやplotlyを用いた表データ操作・分析・可視化

---

## Part 2: Conventional Image Analysis Aproach for Plant Phenotyping

### [イネ種子計数・形状解析](notebooks/rice_seed_shape_analysis.ipynb)

* scikit-imageのregionpropsとwatershedを利用したオブジェクトの計数と形状解析

### [リンゴ葉形状解析](notebooks/apple_leaf_shape_analysis.ipynb)

* 手動特徴量・regionrops・楕円フーリエ記述子を用いた葉形状解析

### [WEIPS：ドローン画像からの雑草除去およびキクイモ表現型定量](notebooks/WEIPS.ipynb)

* MATLABコードのPython再実装
* RGBとDepth情報を用いた領域抽出
* オルソモザイク画像とデジタルサーフィスモデル画像からの表現型抽出

### [ドローン画像からのテンサイ個体認識](notebooks/plant_cataloging.ipynb)（未完

* Vegetation Indicesを使った作物領域のセグメンテーション
* 時系列間での作物の位置合わせ

### [Aravib: シロイヌナズナの茎振動の定量](notebooks/aravib.ipynb)

* Color Thresholdによる特徴点抽出とトラッキング
* scipyのfftを活用した振動解析

---

## Part 3: Training Deep Learning Models for Plant Phenotyping

### [植物病害識別診断モデルの作成](notebooks/plantvilllage.ipynb)

* plantvillageデータセットの活用
* tensorflow.kerasを活用したCNNモデルの構築と訓練

### [大麦種子品種識別モデルの作成](notebooks/barley_seed_classification.ipynb)

* tensorflow.kerasを活用したCNNモデルの構築と訓練
* 現場データ収集における問題（データ不足、データ不均衡）に対応する
  * class weights
  * 転移学習
  * データ拡張

### [甜菜セグメンテーションモデルの作成](notebooks/phenobench.ipynb)

* phenobenchデータセットの活用
* segmentation_models_pytorchを用いた領域分割モデルの作成
  * Binary Semantic Segmenatation
  * MultiClass Semantic Segmentation

### [小麦穂検出モデルの作成](notebooks/globalwheat2021.ipynb)

* Global Wheat Head Dataset 2021の活用
* YOLOv8物体検出モデルの学習と推論

### [カリフラワーインスタンスセグメンテーションモデルの作成](notebooks/growliflower.ipynb)

* GrowliFlowerデータセットの活用
* detectron2ライブラリの活用
* 注意：データセット非商用ライセンス。本への収録は未定。

### [SLEAPを利用したキーポイント検出とトラッキングによる植物の動態解析](notebooks/SLEAP_plant_tracking.ipynb)

* キーポイント検出

---

## Part 4: Utilizing Trained Deep Learning Models for Plant Phenotying

### [大麦種子計数形状解析](notebooks/barley_seed_shape_analysis.ipynb)

### [DeepStomata: マルバツユクサの気孔開度定量](notebooks/dayflower_stomata_quantification.ipynb)

### [イネ収量予測](notebooks/riceyieldcnn.ipynb)

### [植物の根のセグメンテーション](notebooks/plantroots.ipynb)

### [StomaAI:シロイヌナズナの表皮断片顕微鏡画像からの気孔開度定量](notebooks/sai.ipynb)

### [シロイヌナズナのリーフディスク顕微鏡画像を利用した気孔開度定量](notebooks/arabidopsis_stomata_leafdisk.ipynb)

### [力学試験におけるヒノキ断面の構造的変化の定量的解析](notebooks/cell_wall_deformation.ipynb)

### [葉脈抽出とグラフネットワーク解析](notebooks/leaf_venation.ipynb)

### [PlantSeg:3D共焦点画像からの細胞壁検出と細胞インスタンス・セグメンテーション](notebooks/plantseg_240112.ipynb)

## Part 5: Miscellaneous Topics for Plant Phenotyping

### [アノテーションサービスを活用した酵母細胞検出モデルの訓練](notebooks/yeast_object_detection.ipynb)

### [U2-Net (U-Square Net)を利用した葉領域抽出](notebooks/u2netp.ipynb)

### [Depth Anything：深度推定基盤モデル](notebooks/depth_anything.ipynb)

### [MobileSAM:軽量な基盤モデルによるセグメンテーション](notebooks/MobileSAM.ipynb)

### [GroundingDINO:言語ベースの物体検出](notebooks/GroundingDINO.ipynb)

### [LLMによる植物ドメイン画像の視覚的質問応答](notebooks/LLM_rinna.ipynb)

----
