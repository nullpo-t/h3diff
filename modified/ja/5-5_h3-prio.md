## HTTP/3における優先制御

HTTP/3のストリームのフレームの一つに `PRIORITY` があります。
これはストリーム上の優先順位と依存関係を設定するためのもので、その方法はHTTP/2に似ています。
このフレームは、2個のストリーム間の依存性と、特定のストリームの"weight"を設定することができます。

依存関係を持つストリームは、それが依存するすべてのストリームがクローズされている、またはそれ以上処理を進めることができない場合のみ、リソースが割り当てられるべきです。
ストリームのweightは1から256の間の値で、同じ親を持つストリームには、そのweightに比例したリソースが割り当てられるべきであると定義されています。
