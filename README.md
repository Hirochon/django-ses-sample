# django-ses-sample

## 詳しくはコチラ
[Django-SESとAmazon SESでメール運用しようとした時に詰みまくった話(最速の運用手順も紹介)](https://qiita.com/Hirochon/items/44893feee1b6eb8178a1)

## 使い方！
1. AWSにサインイン後に、SES(Simple Email Service)でメールアドレスを登録する！
2. IAMユーザーでプログラム専用のユーザを作成して、アクセスキーIDとシークレットアクセスキーをGETする。
3. 最後にconfig/settings.pyの一番下を自分のアクセスキーIDとシークレットアクセスキーに書き換える。

```python:settings.py
# AWS settings 
AWS_ACCESS_KEY_ID = '自分のアクセスキーID'       # アクセスキーID
AWS_SECRET_ACCESS_KEY = '自分のシークレットアクセスキー'     # シークレットアクセスキー
```