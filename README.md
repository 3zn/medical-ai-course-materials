# メディカルAIコース オンライン講義資料

## 本講義資料について
本ページは 日本メディカルAI学会公認資格：メディカルAI専門コースのオンライン講義資料（以下本資料） です． 本講義資料を読むことで，医療で人工知能技術を使う際に最低限必要な知識や実践方法を学ぶことができます．

本資料を利用される方はこちらのサイトから利用してください．

https://japan-medical-ai.github.io/medical-ai-course-materials/

## 想定受講者
受講想定者として大学生，大学院生，医療従事者を想定しています．

## 内容について
* 線形代数，統計，確率の基礎，機械学習，DeepLearning（深層学習）の基礎や実践を学んでいきます．
* 実践では，Google Colaboratory上で動くJupyter Notebookを使って，ブラウザ上で実際にプログラムを書き，実行結果を確認しながら進めていきます．
* 本資料は全部で8章からなり，各章を終えるのにそれぞれ2〜3時間程度を想定しています．すでに知っている部分がある方は本資料を確認程度でスキップして進めていくこともできます．
* 各章の最後に問題が２つずつ設定されています．この問題に正解した人が合格となります（合格基準は非公開です）．

## 利用
本資料はコースの受講者以外も誰でも自由に無料で使うことができます．

## 資料もくじ
1. 機械学習に必要な数学の基礎
2. 機械学習ライブラリの基礎
3. ニューラルネットワークの基礎
4. Deep Learningフレームワークの基礎
5. 実践編: MRI画像のセグメンテーション
6. 実践編: 血液の顕微鏡画像からの細胞検出
7. 実践編: ディープラーニングを使った配列解析
8. 実践編: ディープラーニングを使ったモニタリングデータの時系列解析

## 推奨ブラウザ環境
主要なブラウザはサポートしています．特に内部で使用しているGoogle Colaboratory はPC 版のChromeとFirefoxでは完全に動作するよう検証されています．

## 本資料の作成者
本資料は株式会社Preferred Networksの岡野原 大輔，齋藤 俊太，菅原 洋平，その他多くの有志，そして株式会社キカガクの吉崎 亮介が中心となって作成しました．

## ビルド方法

```bash
docker pull mitmul/medical-ai-course-materials:build
docker run -v $PWD/build.sh:/build.sh -v $PWD:/medical-ai-course-materials --rm -t mitmul/medical-ai-course-materials:build bash build.sh
```

## ローカルで確認

```bash
cd docs
python -m http.server
```

Then open http://0.0.0.0:8000/

## デプロイ

```bash
GH_TOKEN=<YOUR_GITHUB_TOKEN> bash deploy.sh
```
