# 学んだことまとめ

>7月8,9日

復習

```
Markdownとは文章を手軽に表現できる便利な言語
Gitとはコードの変更した履歴を確認できる開発に必須なツール
リポジトリとはプロジェクトの履歴を保存する場所
コミットとは変更履歴を保存する操作
Githubはリポジトリをインターネットで共有、保存できるサービス
```

***

>6月24,25日 7月1,2日

ファイルアクセス
```
ファイルを扱うにはFileというクラスを利用する

ファイルへ書き出す　writeAsString
    Future<File> writeAsString( [String] );
    同期処理で実行させたいときは
    void writeAsStringSync( [String] );
ファイルから読み込み readAsString
    try {
        変数 = [File].readAsString();
    } catch (e) {}
    
```

***

>6月10~11日

ToDoアプリを作る
```
リスト4-7を応用して作る
アイコン等を追加するときはbody内に書く（サイズ、色など）
押したときの処理等はそのいろいろ下のほうにかく
```

***

>6月4日

ウィジェットいろいろ
```
AppBarのプロパティ
title: タイトル、基本はテキスト
leading:  左端、ボタンやアイコン
action: 右側、ボタンアイコンなどのリスト
bottom: 上記の下に追加表示

ListTile(
    leading:  ,                <表示するアイコン
    title:  ,                  <内容
    selected: bool値 ,         <選択状態
    on Tap: 関数,              <クリックされたときのイベント処理
    onLongPress: 関数          <ロングクリックされたときのイベント処理
    )
```

***

>6月3日

アラートとダイアログ
```
showDialog(                            <アラートを画面に表示する
    context: <<BuildContext>>,        　<ウィジェットのベース
    builder: <<WidgetBuilder>>          <関数を利用するためにある
    )

SimpleDialogOption(                <入力できるダイアログ
    child: ウィジェット,
    children:  処理 ,
    )

```

***

>5月29日

入力するui
```
TextField(                 <テキストを入力できる
    controller: ,          <値を管理している
    style: ,               
         )

イベントを起こすonChangedなどもある（修正されたときに発生する）
複数のうち１つを選択させたいとき Radio
複数選択させたいとき　Checkbox
```
***

>5月28日

uiの基本、ボタンについて
```
TextButton(key:null,       <テキストボタンの場合
onPressed: 関数　,         <クリックされたときの処理
child: ウィジェット         <使うものtextとかiconとか
          )

Padding()              <余白を表示するコンテナになる
```
***

>5月21日
```
ボタンをいつも同じ場所に表示させるときはFloatingActionButtonというクラスを使う
```
***
>5月20日

```
libフォルダでアプリケーションのプログラムを組む
mainという関数がアプリを起動したときに呼び出される処理になる
```
