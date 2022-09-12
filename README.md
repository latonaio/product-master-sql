# product-master-sql

product-master-sql は、主にエッジアプリケーションにおいて、データ連携基盤 と連携された品目マスタデータを保存する SQL テーブルを作成するためのレポジトリです。  
product-master-sql は、そのままクラウド環境におけるアプリケーションにも、適用可能です。

## 前提条件

product-master-sql は、SQL の データ連携基盤 との データ連携にあたり、API を利用し、本レポジトリ の sql 設定ファイルの内容は、下記 URL の API 仕様を前提としています。
https://api.XXXXXXXX.com/api/OP_API_XXXXXXX_XXX/overview  

## sql の設定ファイル

product-master-sql には、sql の設定ファイルとして以下の sql ファイルが含まれています。

* product-master-sql-general-data.sql（データ連携基盤 品目マスタ - 基本データ）
* product-master-sql-plant-data.sql（データ連携基盤 品目マスタ - プラントデータ）
* product-master-sql-mrp-area-data.sql （データ連携基盤 品目マスタ - MRP エリアデータ）
* product-master-sql-procurement-data.sql（データ連携基盤 品目マスタ - 購買データ）
* product-master-sql-sales-plant-data.sql（データ連携基盤 品目マスタ - 販売プラントデータ）
* product-master-sql-sales-organization-data.sql（データ連携基盤 品目マスタ - 販売組織データ）
* product-master-sql-work-scheduling-data.sql（データ連携基盤 品目マスタ - 作業計画データ）
* product-master-sql-quality-data.sql（データ連携基盤 品目マスタ - 品質管理データ）
* product-master-sql-accounting-data.sql （データ連携基盤 品目マスタ - 会計データ）
* product-master-sql-product-description-data.sql（データ連携基盤 品目マスタ - 品目テキストデータ）
* product-master-sql-sales-tax-data.sql（データ連携基盤 品目マスタ - 販売税データ）

## MySQL のセットアップ / Kubernetes の設定 / SQL テーブルの作成方法

MySQL のセットアップ / Kubernetes の設定 / 具体的な SQL テーブルの作成方法、については、[mysql-kube](https://github.com/latonaio/mysql-kube)を参照ください。
