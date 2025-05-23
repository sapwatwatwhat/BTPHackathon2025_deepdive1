# SAP AI Core サンプルコード

このリポジトリには、SAP AI Coreを使用してAIモデルを管理・実行するためのサンプルコードが含まれています。

## 免責事項

> [!WARNING]
> このサンプルコードは、教育および情報提供のみを目的として提供されています。本コードは「現状有姿」で提供され、明示または黙示を問わず、いかなる種類の保証も伴いません。SAPおよび本コードの作成者は、このサンプルコードの使用に起因するいかなる直接的、間接的、偶発的、特別、典型的、または結果的な損害についても責任を負いません。
>
> このリポジトリのコードは本番環境での使用を意図したものではなく、適切なテストと評価なしに実稼働システムに実装すべきではありません。ユーザーは、このコードを使用する前に、自身の環境でテストし、必要に応じて調整することが推奨されます。
>
> また、本サンプルコードに含まれる機能やAPIは、断りなく将来のSAP製品のリリースで変更される可能性があります。


> [!TIP]
> ## ハンズオンマニュアル
>
> ハンズオンの進め方は以下のマニュアルを参照してください：
>
> ### RAGハンズオン
> [RAGハンズオン手順書](99_handson_manual_2025/01_SAPAICore_RAG/README.md)
>
> #### デモ動画
> [![Grounding デモ動画](https://img.youtube.com/vi/vExXOQprhXk/0.jpg)](https://youtu.be/vExXOQprhXk)
> [![Orchestration デモ動画](https://img.youtube.com/vi/crbT2v8LVlU/0.jpg)](https://youtu.be/crbT2v8LVlU)
>
> ### AI Agentハンズオン
> [AI Agent ハンズオン手順書](99_handson_manual_2025/02_AIAgent_on_BTP/README.md)
>
> #### デモ動画
> [![AI Agent デモ動画](https://img.youtube.com/vi/U7Z9AH0B458/0.jpg)](https://youtu.be/U7Z9AH0B458)

## 目次と機能概要

このリポジトリでは、以下のSAP AI Coreの主要機能を体験できます：

- **01_grounding**: 企業のドキュメントやナレッジベースをAIモデルに接続し、信頼性の高い回答を得るためのGrounding機能を実装します。PDFやテキスト文書からの情報抽出、ベクトル検索、類似文書の取得方法を学びます。

- **02_orchestration**: 複数のAIサービスやデータソースを連携させるワークフローを構築します。Groundingモジュールからの情報取得、テンプレート処理、LLMによる回答生成など、複数のステップを組み合わせた高度なAIパイプラインを作成します。

- **03_promptRegistry**: 効果的なプロンプトを一元管理し、バージョン管理するためのプロンプトレジストリ機能を活用します。組織全体で再利用可能なプロンプトテンプレートの作成と管理方法を学びます。

- **04_aiAgentApp**: HANA Cloud Vector Engineを活用した高度なAIエージェントアプリケーションを構築します。ベクトルデータベース、エンべディングモデル、LLM、およびLangChainフレームワークを組み合わせたエンタープライズ向けのAIソリューションを開発します。

- **05_aiAgentApp_simple**: シンプルな構成のAIエージェントアプリケーションを構築します。Vector Engine機能を使わず、基本的なRAG（検索拡張生成）機能を実装する方法を学びます。

## ディレクトリ構成

- `01_grounding/` - ドキュメントグラウンディングのサンプルコード
- `02_orchestration/` - オーケストレーションのサンプルコード
- `03_promptRegistry/` - プロンプトレジストリのサンプルコード
- `04_aiAgentApp/` - AIエージェントアプリケーションのサンプルコード
- `05_aiAgentApp_simple/` - シンプル版のAIエージェントアプリケーションのサンプルコード
- `credentials/` - 認証情報ファイル格納ディレクトリ
- `99_handson_manual_2025/` - ハンズオン手順書

## 01_grounding
### 概要
![01_groundingの概要](01_grounding/assets/00_grounding_overview.png)

### 参考情報
- [SAP AI Core - ドキュメントグラウンディング](https://help.sap.com/docs/sap-ai-core/sap-ai-core-service-guide/document-grounding)
-[SAP AI Core - Generative AI Hubの新機能Groundingを解き明かす](https://community.sap.com/t5/technology-blogs-by-sap/sap-ai-core-generative-ai-hub%E3%81%AE%E6%96%B0%E6%A9%9F%E8%83%BDgrounding%E3%82%92%E8%A7%A3%E3%81%8D%E6%98%8E%E3%81%8B%E3%81%99/ba-p/14065096)

## 02_orchestration
### 概要
![02_orchestrationの概要](02_orchestration/assets/00_orchestration_overview.png)

### 参考情報
- [SAP AI Core Orchestration機能 を解き明かす](https://community.sap.com/t5/technology-blogs-by-sap/sap-ai-core-orchestration%E6%A9%9F%E8%83%BD-%E3%82%92%E8%A7%A3%E3%81%8D%E6%98%8E%E3%81%8B%E3%81%99/ba-p/14066141)
- [SAP AI Core - オーケストレーション](https://help.sap.com/docs/sap-ai-core/sap-ai-core-service-guide/orchestration)

## 03_promptRegistry
### 概要
![03_promptRegistryの概要](03_promptRegistry/assets/00_promptRegistry_overview.png)

### 参考情報
- [SAP AI Core Generative AI Hubのプロンプトレジストリ機能を解き明かす](https://community.sap.com/t5/technology-blogs-by-sap/sap-ai-core-generative-ai-hub%E3%81%AE%E3%83%97%E3%83%AD%E3%83%B3%E3%83%97%E3%83%88%E3%83%AC%E3%82%B8%E3%82%B9%E3%83%88%E3%83%AA%E6%A9%9F%E8%83%BD%E3%82%92%E8%A7%A3%E3%81%8D%E6%98%8E%E3%81%8B%E3%81%99/ba-p/14072026) 
- [SAP AI Core - プロンプトレジストリ](https://help.sap.com/docs/sap-ai-core/sap-ai-core-service-guide/prompt-registry) 

## 04_aiAgentApp
### 概要
SAP HANA Cloud, Vector Engine に追加されたIn-Database Vectorizationと、SAP AI Core - Generative AI HubによるSAPのLLMパートナー企業から提供されるEmbeddingモデルを併用した、LangChainフレームワークによるAI Agentアプリケーションを構築します。

![04_aiAgentAppの概要](04_aiAgentApp/assets/README/setup/00_aiAgentApp_overview.png)

## 05_aiAgentApp_simple
### 概要
SAP HANA Cloud, Vector Engineによるベクトル化の機能を取り除き、`04_aiAgentApp` の簡易版のAIエージェントアプリを構築します。

## 前提条件

- SAP BTP アカウント
- SAP AI Core インスタンス
- Object Store (Amazon S3互換) へのアクセス
- Node.js 環境

## 認証情報の設定

以下の認証情報ファイルを `credentials` ディレクトリに配置する必要があります：

1. `ai_core_sk.json` - SAP AI Coreのサービスキー
2. `object_store_sk.json` - Object Store (S3) のサービスキー
3. `user_defined_variable.json` - ユーザー定義変数（リソースグループIDとシークレット名）

## 実行手順

各ディレクトリのREADME.mdを参照してください。

## 注意事項

- 認証情報ファイル（`credentials/`ディレクトリ内）は適切に保護してください
- 各機能の実行には時間がかかる場合があります
- リソースグループが既に存在する場合は、その旨のメッセージが表示されます