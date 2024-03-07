# navista_voxel_grid_filter

## 概要

点群データをvoxel_gridフィルタでフィルタリングするノード。

## 入力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /input_pcd | sensor_msgs::msg::PointCloud2 | フィルタリングしたい点群データ |

## 出力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /outut_pcd | sensor_msgs::msg::PointCloud2 | フィルタリングした点群データ |

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| voxel_leaf_x | [m] | double | voxel_grid_filterのx軸方向におけるリーフサイズ | 0.1 |
| voxel_leaf_y | [m] | double | voxel_grid_filterのy軸方向におけるリーフサイズ | 0.1 |
| voxel_leaf_z | [m] | double | voxel_grid_filterのz軸方向におけるリーフサイズ | 0.1 |
| pcd_type | [-] | string | PCDのタイプ（XYZ, XYZI, XYZRGB） | XYZ |
