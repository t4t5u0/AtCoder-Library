# AtCoder-Library
自作のAtCoderのライブラリを保管しています。  
高速化に成功したアルゴリズムや理解して次回以降は  
0から書くと時間のかかるアルゴリズムの大枠などをまとめています。

## BFS
|コード名|用途 ・ 説明|その他 ・ 備考|
|:--:|:--:|:--:|
|BreadthFirstSearch.py|幅優先探索|迷路の最短経路を考える問題の時などに役に立つ|

## BitSearch
|コード名|用途 ・ 説明|その他 ・ 備考|
|:--:|:--:|:--:|
|BitSearch.py|Bit全探索|スイッチの ON / OFF 問題などに使える  計算量は O(2 ^ N) |

## DFS
|コード名|用途 ・ 説明|その他 ・ 備考|
|:--:|:--:|:--:|
|DepthFirstSearch.py|深さ優先探索|辺を辿っていく問題などの時に役に立つ|

## MathLibrary
|コード名|用途 ・ 説明|その他 ・ 備考|
|:--:|:--:|:--:|
|divisor.py|約数列挙|約数の列挙を行ってくれる|
|factorization.py|素因数分解|素因数分解を行ってくれる|
|PrimaryCheck.py|素数判定|その数が素数かどうかの判定を行ってくれる  一般的には十分高速だが, 競プロ界隈だと遅い|
|SieveOfEratosthenes_1|エラトステネスの篩 (Ver.1) |O(√N)よりも高速に素数を列挙してくれる （緑Diff以上になってくると使用するタイミングが出てくる）|
|SieveOfEratosthenes_1|エラトステネスの篩 (Ver.2) |Ver.1 の時よりも高速に素数を列挙することができる|

## RunLnegthEncoding
|コード名|用途 ・ 説明|その他 ・ 備考|
|:--:|:--:|:--:|
|rle.py|ランレングス圧縮|２種類くらいのランダム文字列を何の文字が何連続で出てきたかを出力してくれる|

## UnionFindTree
|コード名|用途 ・ 説明|その他 ・ 備考|
|:--:|:--:|:--:|
|UnionFind.py|素集合に分割するアルゴリズム|まだ使用しているのみで, 具体的な構造はわかっていない|
