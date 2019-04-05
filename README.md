# 元号一覧

Wikipediaの情報をベースにWebAPIっぽいものを作ってみました。

## 変更履歴
| 更新日  |  |
|:-----------|:------------|
| 2019-04-05 | 初版 |

## レスポンス

| パラメータ名  |   |   | 出現回数 | 型 | 説明 |
|:-----------|:------------|:-------------|:-----------|:------------|:-------------|
| (Response) |  |  | 1 | complexType | レスポンスルートノード |
| @attributes |  |  | 1 | complexType | 属性情報 |
|  | api_version |  | 1 | string | APIのバージョン |
|  | appendix |  | 1 | complexType | 参照情報 |
|  |  | title | 1 | string | 参照ページタイトル |
|  |  | url | 1 | string | 参照ページURL |
| era |  | | 複数回 | complexType | 元号情報 |
|  | ad | | 1 | integer | 西暦 |
|  | period | | 1 | string | 時代 |
|  | era_kanji | | 1 | string | 元号名(漢字) |
|  | era_yomi | | 1 | string | 元号名(読み) |
|  | reason | | 1 | string | 改元理由 |
