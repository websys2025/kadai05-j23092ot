## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
　　*エンドポイントは "https://zipcloud.ibsnet.co.jp/api/search"　で機能としては入力さてた郵便番号から、住所を返す
* リクエストとレスポンスのフォーマット
  　* ${endpoint}?zipcode=${zipcode}　でエンドポイントと郵便番号を合わせたURIをリクエストすると、message,results,status がレスポンスとしてかえってきて、resultsの中のaddress1,sddress2,address3にそれぞれ、県、市、字の情報が入っている
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
　　* 名称は天気予測APIのopen-Meteo URLはhttps://open-meteo.com/
* エンドポイントと機能
  　* エンドポイントはhttps://api.open-meteo.com/v1/forecast?latitude=${latitude}&longitude=${longitude}&daily=temperature_2m_max,temperature_2m_min&timezone=Asia%2FTokyo　であり、入力した緯度、経度の値から最高気温を出力します。
* リクエストとレスポンスのフォーマット
　　* latitude=${latitude}で緯度を入力し、longitude=${longitude}で経度を入力します。daily=temperature_2m_maxから最高気温、temperature_2m_minから最低気温の値が欲しいとリクエストします。今回は最高気温と、最低気温をリクエストしたので、レスポンスのdailyの中にdaily=temperature_2m_max、temperature_2m_minの値が入っており、それをHTMLに出力する。
### Q3-3. 感想
* 今回の課題で苦労したこと
　　* WebAPIの仕組みが授業では理解できず、複数サイトを見ることで理解した
* 演習を通して理解できたこと
　　*APIの利用方法が少し、理解できた。 
* Web APIの利便性や課題など
　　*今回は、テキストボックスに打った入力から、値を返すようなAPIしか使わなかったが、調べている中で、音声を使ったものや、PayPayなどのAPIも発見したので使い方を覚えていきたい。 
