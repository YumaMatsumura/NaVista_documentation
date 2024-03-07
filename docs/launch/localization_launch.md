# navista_localization_launch

## 概要

NaVistaのlocalizationモジュールを起動するlaunchファイルが管理されているパッケージ。

## 詳細解説

既存パッケージのlidar_localization_ros2を起動する。  
ライフサイクルノードであるため、launchファイル内で自動起動するようにしている。

## パラメータ仕様

| パラメータ名 | 単位 | 型 | 説明 | デフォルト値 |
| --- | --- | --- | --- | --- |
| localization_params_file | [-] | string | localizationモジュールのparamsファイルパス | navista_localization_launch/launch/localization_modules_params.yaml |
| localization_log_level | [-] | string | localizationモジュールのログレベル | warn |
| use_sim_time | [-] | false | シミュレーション時間の使用有無 | false |
