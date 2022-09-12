# product_master_sql

product_master_sql は、主にエッジアプリケーションにおいて、データ連携基盤 と連携された品目マスタデータを保存する SQL テーブルを作成するためのレポジトリです。  
product_master_sql は、そのままクラウド環境におけるアプリケーションにも、適用可能です。

## 前提条件

product_master_sql は、SQL の データ連携基盤 との データ連携にあたり、API を利用し、本レポジトリ の sql 設定ファイルの内容は、下記 URL の API 仕様を前提としています。
https://api.XXXXXXXX.com/api/OP_API_XXXXXXX_XXX/overview  

## sql の設定ファイル

product_master_sql には、sql の設定ファイルとして以下の sql ファイルが含まれています。

* product_master_sql_general_data.sql（データ連携基盤 品目マスタ - 基本データ）
* product_master_sql_plant_data.sql（データ連携基盤 品目マスタ - プラントデータ）
* product_master_sql_mrp_area_data.sql （データ連携基盤 品目マスタ - MRP エリアデータ）
* product_master_sql_procurement_data.sql（データ連携基盤 品目マスタ - 購買データ）
* product_master_sql_sales_plant_data.sql（データ連携基盤 品目マスタ - 販売プラントデータ）
* product_master_sql_sales_organization_data.sql（データ連携基盤 品目マスタ - 販売組織データ）
* product_master_sql_work_scheduling_data.sql（データ連携基盤 品目マスタ - 作業計画データ）
* product_master_sql_quality_data.sql（データ連携基盤 品目マスタ - 品質管理データ）
* product_master_sql_accounting_data.sql （データ連携基盤 品目マスタ - 会計データ）
* product_master_sql_product_description_data.sql（データ連携基盤 品目マスタ - 品目テキストデータ）
* product_master_sql_sales_tax_data.sql（データ連携基盤 品目マスタ - 販売税データ）

## MySQL のセットアップ / Kubernetes の設定 / SQL テーブルの作成方法

MySQL のセットアップ / Kubernetes の設定 / 具体的な SQL テーブルの作成方法、については、[mysql_kube](https://github.com/latonaio/mysql_kube)を参照ください。
