# Japanese
## 概要
本書の目的はDolibarrをベースとした生産管理アプリの開発に用いる資料場所およびソースコード箇所を示す。

## ディレクトリ構造
  DOLIBARR-PROJECT：プロジェクト全体フォルダ（Git管理）
    /docs: 開発用資料格納場所
        -FunctionList.md: 当資料
        -function_{機能名}.md: 機能別仕様書

    /html: ソースコード格納場所
        /core: Dolibarrのコア機能
            /modules: モジュール別の機能

    /themes: テーマ別のレイアウト


## 機能一覧
1. [OAuth認証](function_OAuthVerification.md):OAuth認証: 外部サービスとの認証連携を管理
   - Microsoft, GitHub, Stripe等との認証フロー
   - トークン管理
   - コールバック処理

2. [バーコード管理](function_BarcodeManagement.md): バーコードの生成と管理
   - バーコード生成
   - 印刷機能
   - データ管理

3. [通知管理](function_Notification.md): システム通知の制御
   - 通知設定
   - イベントトリガー
   - 配信チャネル

4. [ラベル管理](function_LabelManagement.md): ラベル印刷と管理
   - ラベルテンプレート
   - 印刷フォーマット
   - バッチ処理

5. [採用管理](function_Recruitment.md): 採用プロセスの管理
   - 求人情報管理
   - 応募者追跡
   - 面接スケジュール
　 - レポート機能

6. [支払い管理](function_Payment.md): 支払い処理と管理
   - 支払い処理
   - ステータス管理
   - レポート生成

7. [POS管理](function_PosManagement.md): POSシステムの管理
   - 販売管理
   - レシート印刷
   - 在庫連携

8. [汎用モジュール管理](function_ModulesManagement.md): モジュールの有効化と設定
  - モジュール管理
  - 設定管理
  - 依存関係チェック

## 機能別ソースコード箇所

### 会計/財務機能
core/accountancy.php
core/finance.php

### 顧客管理機能
core/customer.php

### 在庫管理機能
core/stock.php

### 仕入/発注機能
core/purchase.php

------------------------

# English
## Summary
The purpose of this document is to provide the locations of reference materials and source code for developing a production management application based on Dolibarr.

## Directory Structure
DOLIBARR-PROJECT: Main project folder (managed by Git)
    /docs: Repository for development materials
        - FunctionList.md: This document
        - function_{function_name}.md: Function detail 
    
    /html: Repository for source code
        /core: Core functionality of Dolibarr
            /modules: Module-specific functionalities
    /themes: Layouts for each theme

