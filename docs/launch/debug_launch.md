# navista_debug_launch

## 概要

NaVistaのdebugモジュールを起動するlaunchファイルが管理されているパッケージ。

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| container_name | [-] | string | コンテナ名 | navista_container |
| debug_params_file | [-] | string | debugモジュールのparamsファイルパス | navista_debug_launch/launch/debug_modules_params.yaml |
| debug_log_level | [-] | string | debugモジュールのログレベル | info |
| use_composition | [-] | bool | componentの使用有無 | true |
| use_debug | [-] | bool | debugモジュールの使用有無 | false |
| use_sim_time | [-] | false | シミュレーション時間の使用有無 | false |
