# PlantUML

## Usage

```bash
$ git clone git@github.com:watter46/PlantUML.git
$ cd PlantUML
$ make init
```

## Access

http://localhost:29000

## 詳しい書き方
<https://maku.blog/p/tn6y85z/>


## Notation

###はじめに

@startuml ~ @endumlの間に記述する

コメントはシングルクォーテーションで書ける

```bash
  @startuml
    <この間に記述する>

    '<コメント内容>
  @enduml
```

####クラスの書き方
```bash
  class <クラス名> {

  }
```

####テーブルの書き方
  +をつけることで、緑の中点をつけれる[PK]
  ♯をつけることで、黄色の中点をつけれる[FK]
```bash
  entity <テーブル名> {
    + id INT(10)
    --

    ~~~~~~~~~~
    ~~~~~~~~~~

    ♯ user_id
  }
```

####タイトルの書き方
```bash
  title <タイトル名>
```

####キャプションの書き方
```bash
  caption <キャプション名>
```

####依存関係
```bash
  classA ..> classB
```

####誘導可能性矢印(実線)
```bash
  classA --|> classB
```

####リレーションの書き方(1対多)
```bash
  classA --{ classB
```
