## コネクションにおけるTLS

コネクションを開始するためのInitialパケットのすぐあとに、通信の開始者はセキュアレイヤーにおけるハンドシェイクのセットアップを開始するCRYPTOフレームを送信します[^4-3_1]。
セキュリティレイヤーにはTLS 1.3が用いられます。
TLSを使用せずにQUICコネクションを行う方法はありません。プロトコルの硬直化を防ぐためにQUICはプロトコルレベルでミドルボックスによる通信の改ざんが難しくなるように設計されています。

[^4-3_1]: 編注: Initialパケットのペイロードにハンドシェイクメッセージを含んだCRYPTOフレームがあります\par draft-22 [https://tools.ietf.org/html/draft-ietf-quic-transport-22#section-17.2.2](https://tools.ietf.org/html/draft-ietf-quic-transport-22#section-17.2.2)
