# google_my_map-GAS
Link Google Spreadsheets and Google My Maps via GAS and KML
#English
1. Prepare your spreadsheet
Open Google Spreadsheet and set up the following columns:
Column A: Point name
Column B: Address
Column C: Latitude
Column D: Longitude
Column E: Point color (red, blue, green, yellow, purple, orange)
Enter the header in the first row (e.g. "Point name", "Address", "Latitude", "Longitude", "Color")
Enter the actual data from the second row onwards

2. Prepare My Maps
Access Google My Maps
Create a new map or select an existing map
Copy the part after "mid=" from the map URL (this is the map ID)

3. Set up Google Apps Script
In the spreadsheet, click "Extensions" → "Apps Script"
In the newly opened script editor, delete all existing code
Paste the script code provided
Change the MY_MAP_ID variable in the script to the map ID you copied earlier
Click the "Save" button (enter any name when asked for a name)

4. Script execution and menu display
In the script editor, select onOpen from the function dropdown
Click the "Execute" button (permissions must be approved the first time)
Return to the spreadsheet and refresh the page (F5 key)
A menu called "Google Maps" will appear at the top of the screen
If the menu does not appear:
In the script editor, add onOpen(); to the last line, save it, and run it again
Or run the updateMyMap function directly in the script editor

5. Creating and importing a KML file
Click "Create KML file" from the "Google Maps" menu in the spreadsheet
If the menu does not appear, run the updateMyMap function directly in the script editor
The script will run and a pop-up will appear with a link to the KML file and instructions
Click the My Maps URL displayed in the pop-up
Click the "+" button for layers on the My Maps screen
Select "Import" and select the generated KML file from Google Drive
The KML file can be accessed from the link displayed in the pop-up
Once the import is complete, the points entered in the spreadsheet will appear on the map

6. Procedures for updating data
Update and add data in the spreadsheet
Click "Google Maps" menu → "Create KML file" again
Import the newly generated KML file to My Maps using the same procedure
Notes
Be sure to enter the point name in the spreadsheet (blank rows will be skipped)
Enter latitude and longitude as numbers
Enter the color as red, blue, green, yellow, purple, or orange (case is not important)
The KML file is saved in Google Drive, so you can also check the history of past updates
This method makes it easy to update data from a spreadsheet to My Maps.

#Japanese
1. スプレッドシートの準備

Google スプレッドシートを開き、以下の列を設定します：

A列: ポイント名
B列: 住所
C列: 緯度
D列: 経度
E列: ポイントの色（red, blue, green, yellow, purple, orange のいずれか）


1行目にはヘッダーを入力（例：「ポイント名」「住所」「緯度」「経度」「色」）
2行目以降に実際のデータを入力します

2. マイマップの準備

Google マイマップ にアクセス
新しいマップを作成するか、既存のマップを選択
マップの URL から「mid=」の後ろの部分をコピー（これがマップID）

3. Google Apps Script の設定

スプレッドシートで「拡張機能」→「Apps Script」をクリック
新しく開いたスクリプトエディタで、既存のコードをすべて削除
提供したスクリプトコードを貼り付け
スクリプト内の MY_MAP_ID 変数を、先ほどコピーしたマップID に変更
「保存」ボタンをクリック（名前を聞かれたら任意の名前を入力）

4. スクリプトの実行とメニューの表示

スクリプトエディタで、関数のドロップダウンから onOpen を選択
「実行」ボタンをクリック（初回実行時は権限の承認が必要）
スプレッドシートに戻り、ページを更新（F5キー）
画面上部に「Google マップ」というメニューが表示される

メニューが表示されない場合：

スクリプトエディタで、最後の行に onOpen(); を追加して保存し、再度実行
またはスクリプトエディタで直接 updateMyMap 関数を実行

5. KML ファイルの作成とインポート

スプレッドシートの「Google マップ」メニューから「KML ファイルを作成」をクリック

メニューが表示されない場合は、スクリプトエディタで直接 updateMyMap 関数を実行


スクリプトが実行され、ポップアップに KML ファイルのリンクと手順が表示される
ポップアップに表示されたマイマップの URL をクリック
マイマップ画面でレイヤーの「+」ボタンをクリック
「インポート」を選択し、生成された KML ファイルを Google ドライブから選択

ポップアップに表示されたリンクから KML ファイルにアクセス可能


インポートが完了すると、スプレッドシートに入力したポイントがマップ上に表示される

6. データ更新時の手順

スプレッドシートのデータを更新・追加
「Google マップ」メニュー→「KML ファイルを作成」を再度実行
新しく生成された KML ファイルを同じ手順でマイマップにインポート

注意点

スプレッドシートのポイント名は必ず入力してください（空白の行はスキップされます）
緯度・経度は数値で入力してください
色は red, blue, green, yellow, purple, orange のいずれかを入力（大文字小文字は区別しません）
KML ファイルは Google ドライブに保存されるため、過去の更新履歴も確認できます

この方法を使うことで、スプレッドシートからマイマップへのデータ更新が簡単に行えます。
