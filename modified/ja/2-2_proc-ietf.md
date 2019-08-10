## IETF

QUICプロトコルを標準化するためにIETF内で設立されたQUICワーキンググループは、当初からQUICをHTTP"だけ"ではなく、他のプロトコルの転送にも使用できるべきだと決めました。
Google版のQUICはHTTPだけを転送していました。実際には、HTTP/2のフレーム構文を用いてHTTP/2フレームを効率よく転送していました。
また、IETF版のQUICは、Google版のQUICで用いられた独自の手法ではなく、TLS 1.3に基づいた暗号化とセキュリティを取り入れることを宣言しました。

HTTP以外のプロトコルにも適用したいという要求を満たすため、IETF版のQUICプロトコルのアーキテクチャは2つの異なるレイヤーに分割されました。
"QUICトランスポート"レイヤーと"HTTP over QUIC"レイヤーです（後者は"hq"と呼ばれることがあります）。
このレイヤー分割は、無害に見えますが、IETF QUICとGoogle QUICの間に大きな差を生みました。

ワーキンググループはQUICバージョン1をスケジュール通りに提供するため、HTTPに範囲を絞り、HTTP以外は後回しにしました。
私達が本書を書き始めた2018年3月の時点では、QUICバージョン1の最終仕様は2018年11月にリリースされる予定でしたが、現在では2019年7月に延期しています。

IETF版のQUICが進むにつれて、GoogleチームはIETF版から詳細を取り込み、Google版のQUICをIETF版が目指すであろうプロトコルに向けて進めています。Googleは引き続き、Google版のQUICを彼らのブラウザやサービスで運用しています。
開発中の新しい実装のほとんど[^2-2_1]はIETF版に焦点を置いており、Google版との互換性はありません。

[^2-2_1]: [https://github.com/quicwg/base-drafts/wiki/Implementations](https://github.com/quicwg/base-drafts/wiki/Implementations)
