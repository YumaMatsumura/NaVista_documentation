# navista_octomap_debug

## 概要

指定された範囲のoctomapの各ボクセルをマーカで表示するノード。

## 入力トピック仕様

| トピック名 | 型 | 説明 |
| --- | --- | --- |
| /octomap | octomap_msgs::msg::Octomap | octomapデータ |

## 出力トピック仕様

| サービス名 | 型 | 説明 |
| --- | --- | --- |
| /octomap_debug | visualization_msgs::msg::MarkerArray | octomapのボクセルマーカ |

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| min_x | [m] | double | マーカで表示したいxの最小座標 | -0.1 |
| min_y | [m] | double | マーカで表示したいyの最小座標 | -0.1 |
| min_z | [m] | double | マーカで表示したいzの最小座標 | -0.1 |
| max_x | [m] | double | マーカで表示したいxの最大座標 | 0.1 |
| max_y | [m] | double | マーカで表示したいyの最大座標 | 0.1 |
| max_z | [m] | double | マーカで表示したいzの最大座標 | 0.1 |
