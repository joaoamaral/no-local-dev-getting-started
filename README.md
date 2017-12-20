# nocoding-getting-started

**Warning - under active development**

This is a simple application that can be used to sync (and then view) data from Salesforce using Heroku Connect.

It supports a Getting Started article on Heroku Dev Center that shows how to set up and manage an app without requiring you to install any development tools.

# Deploy

The easiest way to deploy this is to push the button:

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)


# Verified

If you are not yet a Heroku verified account holder, clicking the Heroku button will prompt you to sign up for Heroku first, and enter billing details.  These details are required for abuse prevention - running this app in the standard configuration won't incur any costs.

# Running

After you verify your Heroku account, clicking the Heroku button will create an app, a database, and a demo instance of Heroku Connect.  Following the resulting link will guide you through final configuration in the Heroku Connect UI.

Please make sure that you are in the intended Heroku app context, as you may not be defaulted to the new Heroku Connect app if you have multiple instances already running.

| Method | Endpoint                          | Functionality                                     | Screen                            | Done |
|--------|-----------------------------------|---------------------------------------------------|-----------------------------------|------|
| POST   | /kartes/search                    | searches and filters all medical records          | S016.健診結果に基づく検索         | 全   |
| GET    | /kartes/last_interviews           | get last interviews of the given kartes IDs       | S016.健診結果に基づく検索         | 全   |
| POST   | /attendances/search               | searches and filters all attendances              | S018. 残業情報 検索条件           | 全   |
| GET    | /attendances/last_interviews      | get last interviews of the given attendances IDs  | S018. 残業情報 検索条件           | 全   |
| POST   | /stresschecks/search              | searches and filters all stresschecks             | S017. ストレスチェク結果 検索条件 | 全   |
| GET    | /stresschecks/last_interviews     | get last interviews of the given stresschecks IDs | S017. ストレスチェク結果 検索条件 | 全   |
| PUT    | /interviews                       | upsert an interview                               | S016~S018. 面談登録モーダル       | 全   |
| POST   | /interviews/search                | searches and filters all interviews               | S019. 面談検索画面                | 全   |
| GET    | /employees/{sfid}/email_histories | get email transmitted history of contact id       | S025. メール送信履歴              | 全   |
| POST   | /interviews/notify                | send email from single interview or in bulk       | S019. 面談検索画面                | 全   |
| GET    | /email_settings                   | get all email settings                            | S015. メール設定                  | 全   |
| PUT    | /email_settings                   | creates email settings                            | S015. メール設定                  | 全   |
| PATCH  | /email_settings/{id}              | changes the email settings                        | S015. メール設定                  | 全   |
| POST   | /employees/{sfid}/reset_password  | reset user password                               | S014.一括ユーザアカウント設定     | 全   |
| POST   | /employees/{sfid}/invitation      | re-send invitation email                          | S008. データ一括取り込み画面      | 全   |
