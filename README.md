# Goodays
アプリ名は渡部さんの案が秀逸だったのでパクりましたすみません。

## どんなアプリ？
地図を見ながらお天気情報や周辺施設を検索できるアプリです。
地図上に表示されるお天気マークを見ながらお出かけプランを考える事ができます。
現在地から目的地の経路上にあるスポットの天気も表示できるのが目標です。

## どのように実現するの？
GooglePlayServicesの中にあるGoogleMapsAPIを使ったマップを中心に開発をしていきます。
地名、施設検索はGeocoderで名前から緯度経度を取得し、マップの表示に反映していきます。
天気情報の取得はOpenWeatherAPIを使用してGeocoderで取得した緯度経度をパラメータとして渡して取得します。
このAPIの仕様上最大16日後まで天気予報が取得できるので、このアプリで提供する天気情報も最大16日後までとします。
経路情報については調べ中です。
