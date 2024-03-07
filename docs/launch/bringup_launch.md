# navista_bringup_launch

## 概要

NaVistaの全モジュールを起動するlaunchファイルが管理されているパッケージ。

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| container_name | [-] | string | コンテナ名 | navista_container |
| localization_launch_file | [-] | string | localizationモジュールのlaunchファイルパス | navista_localization_launch/launch/localization_modules.launch.py |
| localization_params_file | [-] | string | localizationモジュールのparamsファイルパス | navista_localization_launch/launch/localization_modules_params.yaml |
| localization_log_level | [-] | string | localizationモジュールのログレベル | warn |
| map_yaml_file | [-] | string | ロードしたいMapの設定ファイルパス | '' |
| map_launch_file | [-] | string | mapモジュールのlaunchファイルパス | navista_map_launch/launch/map_modules.launch.py |
| map_params_file | [-] | string | mapモジュールのparamsファイルパス | navista_map_launch/launch/map_modules_params.yaml |
| map_log_level | [-] | string | mapモジュールのログレベル | info |
| sensing_launch_file | [-] | string | sensingモジュールのlaunchファイルパス | navista_sensing_launch/launch/sensing_modules.launch.py |
| sensing_params_file | [-] | string | sensingモジュールのparamsファイルパス | navista_sensing_launch/launch/sensing_modules_params.yaml |
| sensing_log_level | [-] | string | sensingモジュールのログレベル | info |
| system_launch_file | [-] | string | systemモジュールのlaunchファイルパス | navista_system_launch/launch/system_modules.launch.py |
| system_params_file | [-] | string | systemモジュールのparamsファイルパス | navista_system_launch/launch/system_modules_params.yaml |
| system_log_level | [-] | string | systemモジュールのログレベル | info |
| debug_launch_file | [-] | string | debugモジュールのlaunchファイルパス | navista_debug_launch/launch/debug_modules.launch.py |
| debug_params_file | [-] | string | debugモジュールのparamsファイルパス | navista_debug_launch/launch/debug_modules_params.yaml |
| debug_log_level | [-] | string | debugモジュールのログレベル | info |
| use_composition | [-] | bool | componentの使用有無 | true |
| use_debug | [-] | bool | debugモジュールの使用有無 | false |
| use_sim_time | [-] | false | シミュレーション時間の使用有無 | false |
