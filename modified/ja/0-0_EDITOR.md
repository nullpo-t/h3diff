# 著者序文

<!--
Hello fellow Internet-protocol enthusiast!

This book is our attempt at explaining this next chapter of HTTP evolution on the Internet. I've worked on writing HTTP related code for over twenty years in my role as founder and lead developer of curl, and I've been involved in HTTP standardization for more than ten years within the IETF. I'm thrilled that you, my Japanese friends, now get the opportunity to read up on the details of HTTP/3 in your own language and subsequently join in the fun. HTTP/3 has not even shipped for real yet and the specs and software around it are young and immature. There's lots of room for all of us to dive in and help out!

Enjoy HTTP/3 Explained!

Daniel Stenberg  
July 2019
-->

やあ、インターネットプロトコル愛好家の同志たち！

本書は、インターネットにおけるHTTPの進化の新たな一章を説明しようとする私たちの試みです。
私は、curlの作者およびリードデベロッパとして、20年以上にわたりHTTPに関するコードを書いてきました。
そして、IETFで10年以上にわたりHTTPの標準化に関わってきました。

私の日本の友人である皆さんが、今こうして自身の言語でHTTP/3の詳解を読んで理解する機会を持ち、そして楽しめることに、私は感激しています。
HTTP/3はまだ本格的にリリースされておらず、それを取り巻く仕様やソフトウェアは若くて未熟です。
私たち全員でそこに参加し、手助けする余地があります！

それでは、『詳解 HTTP/3』を楽しんでください！

\begin{flushright}
2019年7月\\
Daniel Stenberg  
\end{flushright}

# 編者序文

本書は、curlの作者であるDaniel Stenberg氏が公開している『HTTP/3 explained』および有志による日本語訳『詳解 HTTP/3』の編著です。

私は、原著の翻訳を最初に始めた太田航平さんからその存在を知りました。
翻訳と査読に参加させていただき、HTTP/3の仕組みと魅力を理解しました。
そして、より多くの方に知ってもらいたいと思い、本書の発行に至りました。
本書では、HTTP/3の仕組みを皆さんが円滑に理解できる筆致を心がけました。
正確な日本語訳に徹したWeb版に対し、本書は意訳や難解な部分への補足を積極的に行いました。
編集中に気づいた原著および日本語訳の改善点は、少しずつフィードバックしていくつもりです。

本書の発行に関わったすべての方に感謝します。
体系的でわかりやすいHTTP/3の解説書を世に出し、
突然のお願いにもかかわらず、本書に向けた序文を書いてくださったDaniel Stenberg氏。
ともに議論を重ね、技術者として刺激を与えてくださった訳者の皆さん。
そして、原著の主要な訳者で、本書を査読してくださった太田航平さん。
本当にありがとうございます。

本書が皆さんのHTTP/3への最初の一歩になることを願います。

\begin{flushright}
2019年7月\\  
伊勢 駿介
\end{flushright}

### 意見と質問

本書の内容は細心の注意をもって確認していますが、誤りや誤解を招く表現に気づかれることもあるでしょう。
それらは、今後の版で改善しますので、発行者である同人サークル「[ぬるぽ帝国](https://nullpo-t.net)」までご連絡いただければ幸いです。

### ライセンス

原著は[Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/) に基づきライセンスされています。
ライセンスに従い、原著に加えた変更を発行者のウェブサイトに掲載しています。
