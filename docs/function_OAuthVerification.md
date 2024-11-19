# 機能名: OAuth認証

## 概要
外部サービス（Microsoft, GitHub, Stripe等）との認証連携を管理するモジュール。
ユーザー認証とトークン管理を行います。

##機能概要
- **認証フロー**: OAuth 2.0の認証フローを実装し、ユーザーが外部サービスにログインする際の認証をサポートしている。
- **トークン管理**: トークンの取得、更新、保存を行い、セッション管理をサポートしている。
- **セキュリティ**: トークンの安全な保存とアクセス制御を実装している。

## 関連ソースコード
### 主要クラス
- modOauth (html/core/modules/modOauth.class.php)
- DoliStorage (OAuth\Common\Storage\DoliStorage)

### コールバックハンドラー
- microsoft_oauthcallback.php
- github_oauthcallback.php
- stripelive_oauthcallback.php
- generic_oauthcallback.php

## 入出力仕様
### 入力
- クライアントID
- クライアントシークレット
- リダイレクトURI
- 認証コード

### 出力
- アクセストークン
- リフレッシュトークン
- トークン有効期限

## 依存関係
- OAuth\Common\Storage
- OAuth\Common\Consumer

