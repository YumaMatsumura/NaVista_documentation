# navista_points_converter

## 概要

sensor_msgs::msg::PointCloud2型の点群データをoctomap_msgs::msg::Octomap型のデータに変換するノード。

## 入力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /pcd | sensor_msgs::msg::PointCloud2 | 点群データ |

## 出力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /octomap | octomap_msgs::msg::Octomap | Octomap形式の点群データ |

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| resolution | [m/cell] | double | Octomapの解像度 | 0.1 |
| pcd_type | [-] | string | PCDのタイプ（XYZ, XYZI, XYZRGB） | XYZ |
