# navista_map_launch

## 概要

NaVistaのmapモジュールを起動するlaunchファイルが管理されているパッケージ。

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| container_name | [-] | string | コンテナ名 | navista_container |
| map_yaml_file | [-] | string | ロードしたいMapの設定ファイルパス | '' |
| map_params_file | [-] | string | mapモジュールのparamsファイルパス | navista_map_launch/launch/map_modules_params.yaml |
| map_log_level | [-] | string | mapモジュールのログレベル | info |
| use_composition | [-] | bool | componentの使用有無 | true |
| use_sim_time | [-] | false | シミュレーション時間の使用有無 | false |
