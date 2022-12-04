### Android開発までの手順
・インストールするもの
git: https://git-scm.com/download/win

Android studio: https://developer.android.com/studio?gclid=EAIaIQobChMIyIWjween-wIVCmoqCh3PNAvtEAAYASABEgJF7fD_BwE&gclsrc=aw.ds#downloads

・アカウント登録
github: https://github.co.jp/

### git bashの起動時のディレクトリを変更する
1. git-bash.exeのショートカットを作成
2. ショートカットのプロパティを開き、ショートカットのタブを開く
3. 作業フォルダーのパスを開きたいディレクトリに変更する
4. 再起動して起動場所が変更されていれば完了

### androidアプリ開発の基礎を学ぶ
#で見出しが作れ、その数で大きさが変わる

### git command
- リモートリポジトリにプッシュ
   1. git add ファイル名（.ですべて選択）
   2. git status（コミットされるファイルを確認）
   3. git commit -m "[ブランチ名] コミットメッセージ"（コミット時に変更内容を追記する）
   4. git push origin ブランチ名

- オプション
   - git commit -amend -m "コミットメッセージ"（直前のメッセージを変更する）
   - git push -u origin ブランチ名（今のローカルからプッシュするブランチを固定する）

### 小ワザ
リポジトリ名とユーザー名と同じにすると、ホーム画面をカスタマイズできる（画像やgifなどを追加など）

### android studioショートカット
自動整形：Ctrl + Alt + L 

###  kotlinの基礎知識
関数定義：「fun 関数名(引数){関数}」

変数定義：「val 変数名: データ型 = 中身」：再代入できない変数(Javaのfinalと同じ)
         「var 変数名: データ型 = 中身」：再代入できる変数
            →内容を初回で固定する場合はval、再度入れ替える場合はvarを使う
            →「: データ型」を宣言しなくても中身を自動で認識してくれる

データ型：Double ：64bit浮動小数点数
         Float  ：32bit浮動小数点数
         Long   ：64bit符号付き整数
         Int    ：32bit符号付き整数
         Short  ：16bit符号付き整数
         Byte   ：8bit符号付き整数
         Char   ：文字('で囲う)
         String ：文字列("で囲う)