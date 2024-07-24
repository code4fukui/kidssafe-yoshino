# キッズセーフ 越前市 吉野地区 / KidsSafe for Echizen-city Yoshino

- https://code4fukui.github.io/kidssafe-yoshino/

- 〇〇市〇〇地区の地域安全マップを作成して、スマホやパソコンで見られる形で共有するツールです
- ExcelやNumbersを使ってCSVデータを編集しアップロードすることで更新できます
- [キッズセーフ by Code for FUKUI](https://github.com/code4fukui/kidssafe/) を使って作られています

## サイトをホーム画面に追加する方法
◆スマホの操作が苦手な方にも、すぐにキッズセーフが閲覧できるように分かりやすい説明を作りました。

・[ホーム画面登録(android）.pptx](https://github.com/code4fukui/kidssafe-okamoto/files/14518682/android.pptx)

・[ホーム画面登録(iphone).pptx](https://github.com/code4fukui/kidssafe-okamoto/files/14518806/iphone.pptx)

## サイトの表示を外国語に切り替える方法

◆サイトの表示を外国語に切り替えて表示したいという時の設定方法を解説してあります。

・[外国語変換方法(iphone).pptx](https://github.com/code4fukui/kidssafe-okamoto/files/14518975/iphone.pptx)

## データの更新方法

1. 変更したいデータを確認する (例、[aed.csv](aed.csv))
2. ダウンロードボタンを押し、ダウンロードする

<img width="306" alt="image" src="https://github.com/code4fukui/kidssafe-template/assets/1715217/053db2b7-1931-4b7c-b369-326523190d64">

3. Excelで編集する
4. 位置情報は、「[緯度経度地図](https://fukuno.jig.jp/app/map/latlng/#%E8%B6%8A%E5%89%8D%E5%B8%82)」から該当場所に動かして、Geo3x3欄に表示された文字列を項目Geo3x3にコピーする

<img width="511" alt="image" src="https://user-images.githubusercontent.com/1715217/219602296-2d3b72ce-581a-4ba8-8c69-edbe1b95ee76.png">

5. Excelで保存する
6. [./](./) に編集したファイルをドロップし、アップロード(Upload)する

<img width="306" alt="image" src="https://github.com/code4fukui/kidssafe-template/assets/1715217/53bdf652-f38a-47dc-8b3e-defa62f989ce">

7. 1分ほど待つと更新される（しばらくはキャッシュが使われることがあるので、プライベートモードなどで開いて確認するといい）

## データ種の追加方法

1. [template.csv](template.csv)をダウンロードし、Excelで開く
2. 2行目以降に地図に設定したい情報を記述する（項目は自由に増やせます）
3. Excelの「ファイル」「名前を付けて保存」を選び「ファイル形式」を「CSV UTF-8(コンマ区切り)(.csv)」に変更して、データ種類がわかるような英数ファイル名で保存する
4. [index.csv](index.csv)をダウンロードし、Excelで開く
5. 3で保存したファイル名とデータ種類名、アイコンファイル名を記述する
6. [./](./) にindex.csvと3で保存したファイルをドロップし、アップロード(Upload)する
7. 1分ほど待つと更新される（しばらくはキャッシュが使われることがあるので、プライベートモードなどで開いて確認するといい）

## アイコン追加方法

1. 大きさ100x100程度の画像を用意し、PNG形式、半角英数名で保存する（JPEGだと背景が透けません）
2. [icon](icon)フォルダを表示し、エクスプローラーなどからドロップし、アップロード(Upload)する
3. [index.csv](index.csv)や各データをダウンロードし、Excelで開き、icon項目を該当ファイル名に変更する
4. 編集したファイルを [./](./) へアップロードする
5. 1分ほど待つと更新される（しばらくはキャッシュが使われることがあるので、プライベートモードなどで開いて確認するといい）

## 通学路などを追加する方法

1. [地理院地図](https://maps.gsi.go.jp/#16/35.930774/136.163506/&base=std&ls=std&disp=1&vs=c1g1j0h0k0l0u0t0z0r0s0m0f1)の作図ツールで描いて、GeoJSON形式で保存
2. アプリに反映する

## 要望などは

- この地区のキッズセーフについて [Issues](../../issues)
- キッズセーフのアプリについて [キッズセーフのIssues](https://github.com/code4fukui/kidssafe/issues)
