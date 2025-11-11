# Portfolio

## Profile
- 敦賀天音 (Tsuruga Amane)  
- 1999/09/06 Female  
- 慶應義塾大学 通信教育過程 法学部甲類(法律) 在学中  
- RPA/Uipathを用いた業務改善をDXエンジニア・セールスエンジニアとして半年間経験  
- 東京都支援事業にてSQLおよびJava研修を受講  

---

## Project Overview
このリポジトリは、SQLの基本操作と応用を学びながら「ZooDB」という動物データベースを構築したサンプルです。  
動物の名前・種類・生年月日・性別・飼育エリアを管理できるテーブルを設計し、  
実際にデータを挿入・検索することでSQLの基礎から応用までを実践しました。  

---

## SQL Sample Code
```sql
CREATE DATABASE ZooDB;
USE ZooDB;

CREATE TABLE AnimalTable (
    animal_id INT PRIMARY KEY AUTO_INCREMENT,
    Name VARCHAR(50),
    Species VARCHAR(50),
    DateOfBirth DATE,
    Gender VARCHAR(10),
    Enclosure VARCHAR(50)
);

INSERT INTO AnimalTable (Name, Species, DateOfBirth, Gender, Enclosure)
VALUES ('LELE', 'Panda', '2025-11-11', 'Female', 'Cute Zone');

```

+-----------+------+---------+-------------+--------+-----------+
| animal_id | Name | Species | DateOfBirth | Gender | Enclosure |
+-----------+------+---------+-------------+--------+-----------+
|         1 | LELE | Panda   | 2025-11-11  | Female | Cute Zone |
+-----------+------+---------+-------------+--------+-----------+


## ZooDatabase_All.sqlの説明
このファイルには、ZooDBデータベースを構築・操作するための一連のSQLコードをまとめています。  
具体的には以下の操作を含みます：

- データベースとテーブルの作成（CREATE DATABASE / CREATE TABLE）
- データの追加（INSERT）
- データの更新（UPDATE）
- データの削除（DELETE）
- 条件分岐による分類（CASE文）
- 並び替え（ORDER BY）

ZooDatabase_All.sql を実行することで、SQLの基本操作（CRUD）から応用的なクエリまでを一通り確認できます。  
ポートフォリオとして「SQLを使ってデータベースを設計・操作できる」ことを示すサンプルです。

## 実行結果スクリーンショット参照先
![AnimalTable結果](images/AnimalTable.png)

## Skills & Learning
- SQL基礎: CREATE, INSERT, SELECT, UPDATE, DELETE, JOIN
- 条件分岐: CASE文
- 並び替え: ORDER BY
- データベース設計の基本理解

## Future Work
- ER図を作成してデータベース設計を可視化
- JavaやRPAとの連携による業務改善シナリオへの応用
