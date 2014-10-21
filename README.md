# Java Base Classes

## Base

* これをExtendすることでいろいろと楽になる予定

### getPrintWriter()
ファイル名 String を入力すると、それに書き込む PrintWriter を返してくれる。  
ちゃんと close() すること。

### getFileBr()
ファイル名 String を入力すると、それを読み込む BufferedReader を返してくれる。

### getBufferedReader()
標準入力の BufferedReader を返してくれる。

### getStringFromFile()
ファイル名 String を入力すると、ファイルから String を改行付きで全部読んでくれる。

### getDateString()
Format を渡してやるとそれに従って、  
引数なしだと "yyyyMMddhhmmss" 形式で、日付の文字列を返してくれる。

### listFiles()
ファイル名 String を入力すると、隠しファイル（"."で始まるファイル）を除いたファイル一覧を
ArrayList<File> で返してくれる。

### lisdDirs()
ガイル名 String を入力すると、隠しファイル（"."で始まるファイル）を除いたファイル一覧の中で、
ディレクトリだけを ArrayList<File> で返してくれる。

## Logger

* ログ取得用

* Logger.setLogName でログの名前を指定して
  * Logger.sPrintln() とかでログを書き込む
  * 最後は Logger.sClose() してください

* ファイル名を指定してインスタンス化しても使える
  * println() でログを書き込む
  * close() で完了