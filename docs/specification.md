# 仕様

        ## 対象レコード

        - `term`
- `pattern`
- `antiPattern`
- `practiceNote`

        ## 必須項目

        `title`, `pattern`, `nextAction`

        ## 警告項目

        `citation`, `reviewDate`

        ## フロー

        1. 入力レコードを受け取る。
        2. `src/core/scenarioEngine.js` が必須項目と警告項目を評価する。
        3. `src/report/reportBuilder.js` が検証結果を集計する。
        4. `dist/validation-result.json` を release evidence の前提証跡にする。

        ## 保存方針

        公開辞書として個人情報を含めず、引用元と更新日を必須管理する
