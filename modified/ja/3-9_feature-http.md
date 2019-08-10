## HTTP/3 over QUIC

HTTP/3と呼ばれるHTTPレイヤーはHTTPに準拠した転送を行います。HTTPヘッダーの圧縮にはQPACKを使用しており、これはHTTP/2のHPACK（[RFC 7541](https://tools.ietf.org/html/rfc7541)）に似ています。
HPACKアルゴリズムはストリーム間の到達順序が保証されることを前提とするため、修正せずにHTTP/3で使用することは不可能でした。
これは、QUICストリームが到達順書を保証しないためです。
QPACKはHPACKのQUIC対応版と言えます。
