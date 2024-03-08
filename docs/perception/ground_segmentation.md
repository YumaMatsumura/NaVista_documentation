# navista_ground_segmentation

## 概要

点群データの地面と非地面をクラスタリングするノード。

## 入力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /input_points | sensor_msgs::msg::PointCloud2 | セグメンテーションしたい点群データ |

## 出力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /ground_points | sensor_msgs::msg::PointCloud2 | 地面の点群データ |
| /obstacle_points | sensor_msgs::msg::PointCloud2 | 非地面の点群データ |

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| angle_resolution | [-] | int | リングの分割数 | 100 |
| ground_height_threshold | [m] | float | 地面とみなされる点の高さの最大値 | 0.1 |
| grid_ring_space | [m] | float | グリッドのリング間の距離 | 0.1 |
| max_slope | [度] | float | 地面とみなされる面の最大勾配 | 1.0 |
| pcl_type | [-] | string | 点群データのタイプ | XYZI |

## 参考文献

- [https://www.mdpi.com/2072-4292/13/16/3239](https://www.mdpi.com/2072-4292/13/16/3239)
