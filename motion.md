# 想定している動き
２つのフォトリフレクタのオンオフで４通りの状態について取得できるようになっている。
- 1:オフ　2:オフ
  - 鍵が中間地点にある→モータを動かすと途中で止まってしまうので動作開始してはならない→エラー
- 1:オフ　2:オン
  - 開閉どちらか。動作可能
- 1:オン　2:オフ
  - 開閉どちらか。動作可能
- 1:オン　2:オン
  - 機械的にあり得ない。エラー

基本的にどちらかがオン，もう片方がオフの場合オンオフ関係が逆になるまでモータを回すという制御で十分動作可能。センサー反応→モータストップまでのラグで歯車の噛み合いが外れるので手動での動作可能。