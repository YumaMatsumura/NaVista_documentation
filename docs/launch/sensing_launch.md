# navista_sensing_launch

## 概要

NaVistaのseningモジュールを起動するlaunchファイルが管理されているパッケージ。

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| container_name | [-] | string | コンテナ名 | navista_container |
| sensing_params_file | [-] | string | sensingモジュールのparamsファイルパス | navista_sensing_launch/launch/sensing_modules_params.yaml |
| sensing_log_level | [-] | string | sensingモジュールのログレベル | info |
| use_composition | [-] | bool | componentの使用有無 | true |
| use_sim_time | [-] | false | シミュレーション時間の使用有無 | false |
