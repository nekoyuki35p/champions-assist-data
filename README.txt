Champions Assist 固有スキル持ち主情報 更新パック

アップロード先:
GitHub: nekoyuki35p/champions-assist-data

1. latest.json
   → 既存の10月京都用 latest.json を置き換える
   dataVersion: 2026.10.20260928.2

2. cm_2026_09_classic_longchamp2400.json
   → 既存の凱旋門賞JSONを置き換える
   dataVersion: 2026.09.20260928.3

追加フィールド（category=inherited_unique のみ）:
- ownerCharacter: ウマ娘のベース名
- ownerVariant: 衣装違い。通常衣装は null
- ownerDisplayName: 画面表示用
- isCostumeVariant: 衣装違いなら true
- ownerSourceUrl: 持ち主確認用URL

例:
"ownerCharacter": "キタサンブラック",
"ownerVariant": "正月",
"ownerDisplayName": "キタサンブラック（正月）",
"isCostumeVariant": true

注意:
この更新はJSONへの情報追加です。
現行アプリv0.9.2は新フィールドを無視できるため既存機能は壊しませんが、
画面に「固有：○○」を表示するにはアプリ側UI対応を次版で追加します。

更新件数:
- 10月京都: inherited_unique 27件
- 凱旋門賞: inherited_unique 24件
