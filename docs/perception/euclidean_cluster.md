# navista_euclidean_cluster

## 概要

点群データをeuclidean_clusterでクラスタリングするノード。

## 入力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /input_points | sensor_msgs::msg::PointCloud2 | クラスタリングしたい点群データ |

## 出力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /cluster_points | sensor_msgs::msg::PointCloud2 | クラスタリングした点群データ |

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| seg_max_iteration | [回] | int | RANSACアルゴリズムにおける最大反復回数 | 100 |
| min_cluster_size | [点] | int | クラスタが有効とみなされる最小の点数 | 100 |
| max_cluster_size | [点] | int | クラスタが有効とみなされる最大の点数 | 25000 |
| seg_distance_threshold | [m] | double | RANSACアルゴリズムで使用される距離しきい値 | 0.02 |
| cluster_tolerance | [m] | double | クラスタリング時に点が同じクラスタに属するとみなされる距離の最大値 | 0.3 |
