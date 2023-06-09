## 用途
各種フロー図の作成

## 環境構築
[Visual Studio Code で UML を描こう！](https://qiita.com/couzie/items/9dedb834c5aff09ea7b2)

## サンプルコード
![PlantUML](./images/PlantUML.png) 
```
@startuml xxシステム
participant ユーザ as U
participant xxシステム as AP 
participant xxシステム as SYS
participant xxシステム管理者 as SYSM

== 通常 ==
U -> AP: xxシス転送設定を行い報告
AP -> AP: 報告更新
AP -> SYS: 報告転送

== 異常検知 ==
AP -> SYS: 報告転送
SYS -> SYS: 異常検知
note right
下層でエラーがエラーが発生した場合
end note
SYSM -> U: 運用フローのお知らせ
@enduml

```

## 参照
[PlantUML](https://plantuml.com/ja/)
