by Takaya S.
# Waiting System

## 環境構築手順
以下の手順を踏むことで環境構築が可能。
1. docker desktopをインストール→起動
2. git clone git@github.com:TakayaShimabukuro/onct-12th.git
3. docker-compose up -d

## それぞれのページURL
dockerが立ち上がったら以下のURLにアクセスできる。
- frontend : http://localhost:3000/ 
- backend : http://localhost:8080/
- nginx : http://localhost:9001/
## 使用言語
- React
- fastAPI
- nodejs
- nginx



## 注意事項
- frontendのライブラリインストールはyarnとpackage.jsonで管理。追加するには、frontendコンテナのターミナルに入って、以下を実行する。
  - yarn add <package name>
- backendのライブラリインストールはpoetryで管理。追加するには、backendコンテナのターミナルに入って、以下を実行する。
  - poetry add <package name>
  - poetry update

## 参考文献
- https://cloudsmith.co.jp/blog/virtualhost/docker/2022/12/2241971.html
