# このリポジトリについて

Magic: the Gathering のカードのフレーバーテキストを取得し、日本語と他言語を対照して解析するためのプログラム及び解析したデータが保存されています。

# それぞれのプログラムについて

## DataFetcher.ipynb

Scryfallからデータを取得するためのノートブックです。このノートブックを実行することにより、カード名とフレーバーテキストが日英及びその他一つの言語ごとに収集され、結果が「out*.csv」に保存されます。

## DataAnalyzer.ipynb

「out*.csv」を手作業で処理して、対応する語を「correspond」列に埋めていきます。結果は「worked.csv」に保存されます。

「worked.csv」 は「out*.csv」に存在していた情報に加え、新たにcorrespond列を持ちます。correspondは対応する文字列がハイフン区切りで保存されています。

## DataCollector.ipynb

「worked.csv」を整形・表示します。
