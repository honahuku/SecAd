```mermaid
sequenceDiagram
    participant User as ユーザー
    participant Site as Webページ
    participant AdsPlatformer as 広告事業者
    participant ISP as ISP
    participant MonitoringSystem as SecAd
    User->>Site: 訪問
    Site->>AdsPlatformer: 広告リクエスト
    AdsPlatformer->>Site: 広告を表示
    AdsPlatformer->>ISP: サイトの情報
    ISP->>MonitoringSystem: サイトの情報
    alt サイトが有害
        MonitoringSystem->>User: 警告を送信
    end

```
