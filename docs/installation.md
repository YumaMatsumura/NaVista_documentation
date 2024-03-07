# 環境セットアップ

## 依存パッケージ

- [https://github.com/YumaMatsumura/MapVista](https://github.com/YumaMatsumura/MapVista)
- [https://github.com/rsasaki0109/ndt_omp_ros2](https://github.com/rsasaki0109/ndt_omp_ros2)
- [https://github.com/rsasaki0109/lidar_localization_ros2](https://github.com/rsasaki0109/lidar_localization_ros2)

## インストール手順

1. ワークスペースを作成する。

   ```bash
   mkdir -p ~/ros2_ws/src && cd ~/ros2_ws/src
   ```

2. 必要なパッケージをインストールする。

   ```bash
   git clone https://github.com/YumaMatsumura/NaVista
   git clone https://github.com/rsasaki0109/ndt_omp_ros2 -b humble
   git clone https://github.com/rsasaki0109/lidar_localization_ros2
   ```

3. rosdepコマンドで依存するパッケージをインストールする。

   ```bash
   rosdep install -r -y --from-paths .
   ```

4. ビルドする。

   ```bash
   cd ~/ros2_ws
   colcon build
   ```

!!! Tip
    手順3のrosdepコマンドを実行したときにエラーが表示されたときは、以下の手順に従い、rosdepパッケージのインストールと初期化・アップデートを行う。
    ```bash
    sudo apt install python-rosdep2
    sudo rosdep init
    rosdep update
    ```
