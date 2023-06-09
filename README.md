# Coding Partner
## 目次
- [目次](#目次)
- [設定](#設定)
  - [APIキーの設定](#apiキーの設定)
  - [ユーザー名設定](#ユーザー名設定)
  - [ボット名の設定](#ボット名の設定)
- [チャット機能](#チャット機能)
- [サンプルコード生成機能](#サンプルコード生成機能)
  - [自由記述の場合](#自由記述の場合)
  - [テンプレートを利用する場合](#テンプレートを利用する場合)
- [リファクタリング機能](#リファクタリング機能)
- [注釈](#注釈)

## 設定
---
Macを使用している場合は「`⌘ + ,`」 、Windowsを使用している場合は「`Ctrl + ,`」でユーザ設定を開くことができます。<br>
ユーザー設定の検索で「`coding-partner`」と検索すると以下の項目が表示されます。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/chat1.png" width="900">

### APIキーの設定
**この項目の設定は必須です。**<br>
この項目を設定しないとチャット機能、コーディング支援共に動作しません。<br>
IOpenAI Platformの[ログインページ](https://platform.openai.com/signup)からサインイン/サインアップしてください。<br>
画面の右上のアカウントアイコン(プラン)をクリックし、「`View API Keys`」をクリックします。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/settings2.png" width="900">

<br>
画面中央左の「`Create new secret key`」を押下しシークレットキーを作成します。<br>
作成後に表示されるシークレットキーは二度と確認できないので必ず保管してください。<br>
作成したシークレットキーをVS Codeのユーザー設定のApikeyに設定してください。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/settings3.png" width="900">

<br>

### ユーザー名設定
「`User Name`」の項目にはチャットを使用する際に表示されるユーザー名を設定することができます。<br>
この項目の設定は任意でデフォルト値は「You」です。

### ボット名の設定
「`Bot Name`」の項目にはチャットを使用する際に表示されるユーザー名を設定することができます。<br>
この項目の設定は任意でデフォルト値は「GPT」です。

<br>

## チャット機能
---
チャット機能はサイドメニューからエクスプローラを選択して、「`ASK THE GPT`」のタブを開くことで使用することができます。(※1)<br>
画面下部のフォームからメッセージを入力し、Enterまたは送信ボタンのクリックでメッセージを送信することができます。<br>
右側に自分が送信したメッセージ、画面左側にボットからの返答が表示されます。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/chat1.png" width="900">

<br>

## サンプルコード生成機能
---
サンプルコード生成は自由記述とテンプレートを利用する2つの方法があります。<br>
自由記述では生成したいコードの要件を自由に記述します。<br>
テンプレートを利用する場合はテンプレートに則ってコード生成の指示をします。

<br>

### 自由記述の場合
編集しているファイルにどのようなコードを生成して欲しいかを記述します。<br>
要件を示した文章を範囲選択し、「`サンプルコードを生成`」をクリックするとサンプルコードが生成されます。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/generate-free1.png" width="900">

<br>

### テンプレートを利用する場合
編集しているファイルで右クリックし、「`テンプレート生成`」をクリックします。<br>
テンプレートには「言語」、「関数/プログラム名」、「関数にするか否か」、「処理詳細」の項目があるため適当な値を設定します。<br>
適当な値を設定後、テンプレートを範囲選択し「`サンプルコードを生成`」をクリックしてサンプルコードを生成します。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/generate-template1.png" width="900">

<br>

## リファクタリング機能
---
リファクタリング機能は選択したコードのリファクタリング案を提案します。
リファクタリング対象のコードを範囲選択後、右クリックし「`選択したコードを最適化`」を選択すると最適化案が提案されます。

<img src="https://github.com/Gomican/coding-partner/blob/main/images/optimize1.png" width="900">

<br>

最適化案はオリジナルのコードと最適化後のコード両方が表示されます。(オリジナルはコメントアウト)<br>
<img src="https://github.com/Gomican/coding-partner/blob/main/images/optimize2.png" width="900">


## 注釈
※1. チャット機能へのアクセスについては今後のアップデートの中でサイドメニューに専用のアイコンを設置することを想定しています。
