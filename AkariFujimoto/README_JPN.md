# \藤本茜李\の成果

[🇺🇸 English](./README.md) | 🇯🇵 日本語  
このディレクトリは，2026年度医学研究実習（徳島大学 医学部 医学科 3年次科目）における\[学生\]が作成した公開可能な研究成果（Jupyter Notebook，解析スクリプト，ワークフロープログラムなど）をまとめています．  

## 日本人における血液バイオローム由来生物学的年齢モデルの構築と評価
本研究では東北メディカル・メガバンク計画のデータを用いて、日本人集団における血液メタボローム由来の生物学的年齢モデルを構築した。
メタボローム、特定健診、臨床検査の３つのプラットフォームから7種類の年齢予測モデルをLASSO回帰により作成した。
さらに、予測年齢と実年齢の差をΔageとして算出し、臨床検査項目や既往歴との関連を評価した。

## Notebookおよびその他の成果物
# 前処理
1. 1_25117_TMM-BAge_Precheck-ver1.ipynb
- 元データの読み込み
- データ構造の確認
2. 2_260916_TMM_preprocess-ffq.ipynb
- 品質管理
3. 3_260924_TMM-BAge_Preproceess_Metabolome.ipynb
- 解析対象データの抽出
- 品質管理
- 欠損値処理
4. 4_261008_TMM-BAge_lifestyle-preprocess.ipynb
- 解析対象データの抽出
5. 5_260930_TMM-BAge_specific-panel.ipynb
- 解析対象データの抽出
- 前処理
6. 6_261005_TMM-BAge_laboratory-panel.ipynb
- 解析対象データの抽出
- 前処理
7. 7_261002_TMM-BAge_MetAge-preprocess.ipynb
- 前処理
8. 8_261016_TMM-BAge_MetAge-LASOO-regressionSHAP.ipynb
- メタボローム由来モデルの作成
- SHAP値の算出
9. 9_261019_TMM-BAge_SpeAge-LASSO.ipynb
- 特定健診由来モデルの作成
10. 10_261019_TMM-BAge_LaboAge-LASSO.ipynb
- 臨床検査由来モデルの作成
11. 11_261019_TMM-BAge_model-comparision.ipynb
- カテゴリモデル間の比較
12. 12_261019_TMM-BAge_pheno-panel-regression.ipynb
- 表現型回帰分析

## 必要要件
- python
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- statsmodels

## ライセンス
解析データは公開しない 

## 謝辞
東北メディカル・メガバンク計画のデータを利用した。 

## ログ
- ディレクトリ作成：2026年10月21日（渡邊謙吾）
- 成果物の追加：2026年10月22日（藤本茜李）
