# set up
```bash
$ mkdir backend
$ mkdir frontend
$ brew install maven # Mavenのインストール
$ brew install node # Node.jsのインストール
```

```
$ cd backend && mvn archetype:generate -DgroupId=com.example.todoapp -DartifactId=todoapp-backend -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```
- mvn archetype:generate: Mavenを使用してプロジェクトを生成
  - DgroupId=com.example.todoapp: プロジェクトのグループIDを指定します。これはJavaのパッケージ構造に対応し、通常はドメイン名を逆にした形式で記述されます。
  - DartifactId=todoapp-backend: プロジェクトの名前（アーティファクトID）を指定します。
  - DarchetypeArtifactId=maven-archetype-quickstart: 使用するアーキタイプ（テンプレート）を指定します。この場合、基本的なJavaプロジェクトのテンプレートを使用します。
  - DinteractiveMode=false: 対話モードを無効にし、すべての設定をコマンドラインで指定します。
```
$ cd frontend && npx create-react-app todoapp-frontend
```
- npx create-react-app todoapp-frontend: Create React Appを使用してReactプロジェクトを作成します。
  - npx: Node.jsのパッケージランナーで、ローカルにインストールされていないパッケージを実行できます。
  - create-react-app: Reactアプリケーションを簡単にセットアップするためのツールです。
  - todoapp-frontend: 作成するプロジェクトの名前を指定します。
