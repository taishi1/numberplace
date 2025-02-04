# これは何
数字パズル「ナンバープレイス」（ナンプレ）をブラウザで遊べるようにする JavaScript です。

ナンプレには81個のセルがありますが、これを長さ81の数値の配列と考えます。  
左上が Index 0で、右下が80です。

その配列に対して、ナンプレのゲームに必要な、種々の処理を行う関数が集められています。

ちなみに、ソースコード不要で遊ぶだけであれば、この JavaScript を使用したページを下記で公開しています。  
https://stonetank.com/numberplace/

# ファイル説明
- example …… numberplace.js を使ったサンプル実装 そのままでも使えるはず
    - index.html 
    - numberplace.css
    - numberplace.ui.js
- LICENSE …… ライセンスファイル
- numberplace.js …… 本体
- README.md …… 本ファイル

本体ファイル `numberplace.js` は UI に関知しないようになっています。  
どのセルに何の数字が表示されているかなどは UI 側の話なので、 `numberplace.js` では扱いません。

サンプル実装では、代わりに `numberplace.ui.js` で UI 表示内容を保持しています。  
例えば各セルの数字を保持する配列は `numbers` です。

各ファイルのコメントでは、ナンプレの横方向の一列を「行」、縦方向を「列」、そして3×3の範囲を「窓」と呼んでいます。

# 補足
`encodeSpell(numbers)`, `decodeSpell(spell)` では、各セルに入れる数値の配列(長さ81の数値の配列)を、54文字の文字列にエンコード/デコードしています。

ナンプレのゲーム自体の機能としては不要かもしれませんので、適宜変更するなり削除するなりしてください。  
(もちろん、そのまま使うことを妨げるものではありません。)

# 免責事項
- 自分たちで遊ぶために作ったもののため、品質はご容赦ください。  
Issue を切っていただければ対応は検討しますが、対応を保証するものではありません。
- 上記を含め、免責事項についてはライセンスをご確認ください。