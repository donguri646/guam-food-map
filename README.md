Guam Family Travel MAP — リアル詳細MAP版

グルメMAPの最初からOpenStreetMapベースの道路地図を使用。
- 道路・地形・街区が見える詳細地図
- 1ピン=1店舗
- ピンタップで店舗情報
- 店舗一覧から店舗位置へズーム
- 朝食/ランチ/ディナー等の絞り込みがMAPにも連動
- 料理写真ギャラリー
- 公式サイト / Google Maps
- iPhone向け
- OpenStreetMap attribution included


重要: 詳細MAP版のJavaScript構文エラーを修正し、Leaflet地図が初期化されることを確認した修正版です。


【最終方式変更】Leafletを完全削除。外部JavaScriptライブラリに依存せず、OpenStreetMapのEmbed iframeを使用。店舗一覧タップで選択店舗の位置へ地図を切り替えます。


【重要修正】店舗の経度データが西経(-144.xxx)になっていたため、グアムの東経(144.xxx)へ正規化。これにより全28店舗のピンを詳細MAP上に表示。Leaflet等の外部JSは使用せず、OSM Embed + ピンオーバーレイ方式。


【MAP同期修正】OpenStreetMap iframe上に固定ピンを重ねる方式を廃止。OSMタイルを直接描画し、Web Mercator座標で地図と店舗ピンを同じ座標系で計算。スワイプ移動・＋−ズーム・ピン位置が完全連動。外部Leaflet等のJSライブラリ不要。
