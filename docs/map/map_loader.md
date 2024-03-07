# navista_map_loader

## 概要

MapVistaで保存したマップの設定ファイルYAMLファイルを解釈し、OctomapファイルとPCDファイルをロードするノード。
ロードしたマップはROSトピックとしてパブリッシュされる。

## 出力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /pcd_map | sensor_msgs::msg::PointCloud2 | PCDマップの生データ |
| /octomap | octomap_msgs::msg::Octomap | octomapの生データ |

## 入力サービス仕様

| サービス名 | 型 | 説明 |
| --- | --- | --- |
| /load_map | navista_map_msgs::srv::LoadMap | ロードするマップの設定ファイルパス |

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| global_frame_id | [-] | string | グローバル座標系 | map |
