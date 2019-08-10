## UDP上の転送プロトコル

QUICはUDPのユーザー空間に実装された転送プロトコルです。
あなたのネットワークトラフィックを軽く確認してみれば、QUICはUDPパケットとして見えるでしょう。

UDP上に実装されている以上、QUICもまた、UDPのポート番号を利用して、与えられたIPアドレス上にある特定のサービスを識別します。
現在、既知のQUICのすべては、ユーザー空間で動作するように実装されています。
これは通常、カーネル空間で実装するよりも素早い発展が可能です。

### うまく動作しますか？

エンタープライズのネットワークなどではポート53（DNS）以外のUDPトラフィックをブロックするように設定することがあります。
他にも、制御技術がQUICの性能をTCPを利用したプロトコルよりも悪くすることがあります。
このような、運用者が行うかもしれないことに関する議論には果てがありません。
近いうちにおいては、すべてのQUICをもとにした転送の用途は、もう一つの（TCPをもとにした）代替手段に正常に切り替えられる必要があるでしょう。
これについて、Googleのエンジニアによると、計測では1桁台前半の失敗率だったとのことです。

### 良くなりますか？

QUICがインターネットの世界にとって価値のある追加物だと証明されれば、人々はそれを使いたいと考え、自分たちのネットワークで機能することを望み、企業はそれに対する障害について考え直すでしょう。
長年にわたりQUICの開発は進んでおり、インターネットにおいてQUICを利用した接続の成功率は向上しています。