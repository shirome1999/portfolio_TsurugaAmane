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

SELECT * FROM AnimalTable;
+-----------+------+---------+-------------+--------+-----------+
| animal_id | Name | Species | DateOfBirth | Gender | Enclosure |
+-----------+------+---------+-------------+--------+-----------+
|         1 | LELE | Panda   | 2025-11-11  | Female | Cute Zone |
+-----------+------+---------+-------------+--------+-----------+
