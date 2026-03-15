
# STREAM DIRECTOR プライバシーポリシー（AIエージェント機能対応版）

[@dhq_boiler](https://twitter.com/dhq_boiler) （以下「開発者」という）は開発者の提供する STREAM DIRECTOR の利用者（以下「ユーザー」という）に関する個人情報を含んだ情報（以下「ユーザー情報」という）の取扱いについて、以下のとおりプライバシーポリシー（以下「本ポリシー」という）を定めます。

## 1. 情報を取得するアプリ提供者

[@dhq_boiler](https://twitter.com/dhq_boiler)

## 2. 取得するユーザー情報と目的

本アプリケーションで取得するユーザー情報と目的は以下のとおりです。

### ユーザーが自ら提供する情報

|取得するユーザー情報|利用目的|
|-|-|
|AIチャットに入力されたテキストメッセージ|OpenAI API に送信し、AIエージェントからの応答を生成するために使用します。|
|音声入力（マイク録音）によるデータ|OpenAI Whisper API に送信し、音声をテキストに変換するために使用します。|
|OpenAI API キー|OpenAI API への認証に使用します。ローカルデバイス上に暗号化して保存され、外部には API 認証時のみ送信されます。|

## 3. 取得するデバイス情報と目的

本アプリケーションで取得するデバイス情報と目的は以下のとおりです。

### 自動で収集する情報

|取得するデバイス情報|利用目的|
|-|-|
|サウンド入力デバイスの名称|ユーザーが音声キャプチャするデバイスを識別できるようにします。|
|サウンド出力デバイスの名称|ユーザーが音声出力するデバイスを識別できるようにします。|
|プロセス音声キャプチャの名称|ユーザーが音声キャプチャするプロセスを識別できるようにします。|
|サウンド入力デバイスのフォーマット（サンプリングレート、ビット深度、チャンネル数）| 音声キャプチャしたバッファを正しく取り扱うために使います。|
|サウンド出力デバイスのフォーマット（サンプリングレート、ビット深度、チャンネル数）|サウンド出力デバイスに与えられたバッファを正しく再生させるために使います。|

## 4. 取得方法

- デバイス情報は、本アプリケーションの起動直後に自動で収集します。
- AIチャットのメッセージおよび音声データは、ユーザーがAIエージェント機能を使用した際に取得します。
- API キーは、ユーザーがAI設定画面で入力した際に取得します。

## 5. 通知・公表または同意取得の方法・利用者関与の方法

### (1) 通知・公表

開発者は、本ポリシーに関する通知・公表は本アプリケーションまたは本アプリケーションのリポジトリに掲載する方法で行います。

### (2) 同意取得の方法

ユーザーがアプリを起動した時に同意したものと見なします。

### (3) 利用者関与の方法

- ユーザー情報の取得は、本アプリケーションを終了またはアンインストールすることで中止することができます。
- AIエージェント機能を使用しなければ、外部サービスへのデータ送信は行われません。

## 6. 外部送信・第三者提供

### (1) 外部送信

AIエージェント機能を使用する場合、以下の情報が外部サービスに送信されます。

|送信先|送信される情報|目的|
|-|-|-|
|OpenAI API (`api.openai.com`)|チャットメッセージ、アプリの状態情報（デバイス名、接続状態等）|AIエージェントの応答生成|
|OpenAI Whisper API (`api.openai.com`)|音声録音データ|音声からテキストへの変換|

送信されたデータの取扱いについては、[OpenAI のプライバシーポリシー](https://openai.com/policies/privacy-policy)をご確認ください。

AIエージェント機能を使用しない場合、一切外部に送信しません。

### (2) 第三者提供

本アプリケーションは、上記 (1) に記載された外部送信を除き、取得したユーザー情報を第三者に提供しません。

## 7. データの保存

|保存されるデータ|保存場所|保存方法|
|-|-|-|
|OpenAI API キー|ローカルデバイス|Windows DPAPI による暗号化|
|AI設定（モデル選択等）|ローカルデバイス|YAML ファイル（`%LOCALAPPDATA%\dhq_boiler\STREAMDIRECTOR\AiAgentSettings.yml`）|
|チャット履歴|ローカルデバイス（メモリ上のみ）|アプリ終了時に破棄されます|

## 8. お問い合わせ

本ポリシーに関する、ご意見、ご質問、苦情の申し出その他ユーザー情報の取扱いに関するお問い合わせは、以下の窓口にご連絡ください。

**問い合わせ窓口**
[@dhq_boiler](https://twitter.com/dhq_boiler) (https://twitter.com/dhq_boiler)

## 9. 改定

開発者は、開発者の裁量に基づいて、本ポリシーを変更します。ただし、取得するユーザー情報、利用目的、第三者提供に変更が発生した場合、本アプリケーションまたは本アプリケーションのリポジトリで通知します。

## 10. 制定日・改定日

制定：2024年8月11日
改定：2026年3月16日

---

# STREAM DIRECTOR Privacy Policy (AI Agent Feature Edition)

[@dhq_boiler](https://twitter.com/dhq_boiler) (hereinafter referred to as "the Developer") establishes the following Privacy Policy (hereinafter referred to as "this Policy") regarding the handling of information, including personal information, of users (hereinafter referred to as "Users") of STREAM DIRECTOR provided by the Developer (hereinafter referred to as "User Information").

## 1. App Provider That Collects Information

[@dhq_boiler](https://twitter.com/dhq_boiler)

## 2. User Information Collected and Purpose of Use

The User Information collected by this application and its purposes are as follows.

### Information Provided by Users

|User Information Collected|Purpose of Use|
|-|-|
|Text messages entered in AI chat|Sent to the OpenAI API to generate responses from the AI agent.|
|Audio input (microphone recording) data|Sent to the OpenAI Whisper API to convert speech to text.|
|OpenAI API key|Used for authentication with the OpenAI API. Stored encrypted on the local device and transmitted externally only during API authentication.|

## 3. Device Information Collected and Purpose of Use

The device information collected by this application and its purposes are as follows.

### Automatically Collected Information

|Device Information Collected|Purpose of Use|
|-|-|
|Sound input device names|To allow Users to identify devices for audio capture.|
|Sound output device names|To allow Users to identify devices for audio output.|
|Process audio capture names|To allow Users to identify processes for audio capture.|
|Sound input device format (sample rate, bit depth, number of channels)|Used to correctly handle captured audio buffers.|
|Sound output device format (sample rate, bit depth, number of channels)|Used to correctly play back buffers on sound output devices.|

## 4. Collection Method

- Device information is automatically collected immediately upon application startup.
- AI chat messages and audio data are collected when Users use the AI agent feature.
- The API key is collected when Users enter it in the AI settings screen.

## 5. Notification, Disclosure, Consent, and User Involvement

### (1) Notification and Disclosure

The Developer will notify and disclose matters related to this Policy by posting them in the application or in the application's repository.

### (2) Consent

By launching the application, Users are deemed to have consented to this Policy.

### (3) User Involvement

- Users can stop the collection of User Information by closing or uninstalling the application.
- No data is transmitted to external services if the AI agent feature is not used.

## 6. External Transmission and Third-Party Disclosure

### (1) External Transmission

When using the AI agent feature, the following information is transmitted to external services.

|Destination|Information Transmitted|Purpose|
|-|-|-|
|OpenAI API (`api.openai.com`)|Chat messages, application state information (device names, connection status, etc.)|AI agent response generation|
|OpenAI Whisper API (`api.openai.com`)|Audio recording data|Speech-to-text conversion|

For the handling of transmitted data, please refer to the [OpenAI Privacy Policy](https://openai.com/policies/privacy-policy).

When the AI agent feature is not used, no information is transmitted externally.

### (2) Third-Party Disclosure

This application does not disclose collected User Information to third parties, except for the external transmissions described in (1) above.

## 7. Data Storage

|Data Stored|Storage Location|Storage Method|
|-|-|-|
|OpenAI API key|Local device|Encrypted using Windows DPAPI|
|AI settings (model selection, etc.)|Local device|YAML file (`%LOCALAPPDATA%\dhq_boiler\STREAMDIRECTOR\AiAgentSettings.yml`)|
|Chat history|Local device (in memory only)|Discarded when the application is closed|

## 8. Contact

For opinions, questions, complaints, or other inquiries regarding the handling of User Information under this Policy, please contact the following:

**Contact**
[@dhq_boiler](https://twitter.com/dhq_boiler) (https://twitter.com/dhq_boiler)

## 9. Revisions

The Developer may revise this Policy at its discretion. However, if there are changes to the User Information collected, the purposes of use, or third-party disclosure, the Developer will notify Users through the application or the application's repository.

## 10. Effective Date and Revision Date

Established: August 11, 2024
Revised: March 16, 2026
