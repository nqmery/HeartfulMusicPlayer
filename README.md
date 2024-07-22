# HeartfulMusicPlayer

某ラジオ局の音響のソフトの練習用。

## 機能
### 実装済み
- なし
### 未実装
- **UI**
  - **再生画面**
    - 各音源のボタン
      - 1画面につき6x6(1920x1080ディスプレイにおいて)
      - 音源タイトル部
        - タイトル文字
          - ファイル名を表示するのかタイトルを表示するのか
        - 再生時間
        - 枠
          - 非選択 -> 白色
          - 再生中 -> 赤色
          - 選択中(次に再生) -> 青色
      - リピートボタン(チェックボックス)
      - シークバー
      - ファイル選択ボタン
    - ページ切り替えボタン
      - ページの上限数:未定
    - ショートカットキーモードの切り替えボタン
      - 現場モード(ミキサーのフェーダーの$ - \infty$のところにキースイッチが設置されている)
        - ミキサーのフェーダーが$- \infty$になったときに停止
        - ミキサーのフェーダーが$- \infty#から上がったときに選択中の音源を再生
        - (スイッチの押下/離す に別のキーを割り当てるか、同じキーの押下状態で判別するか)
      - パソコン用ポン出しモード(できれば)
        - 各音源にキーを割り当て、押したキーに対応する音源を最初から再生
        - 同時再生は可能にするか不可にするか(現場は不可だが…)
        - 全停止キーも割り当てたい
      - 無効
        - 一切のショートカットキーを無効化
    - 音源配置の保存ボタン
      - 保存形式:未定
    - 設定ボタン
  - **設定画面**
    - 再生デバイスの変更
    - ショートカットキーの変更
    - サウンドドライバの変更
- **ファイルの入出力**
  - 音源ファイルの読み込み
  - 配置の読み込み/保存
  - 設定の読み込み/保存
- **音源部**
  - **再生制御**
    - 音源ボタンを直接クリックすることによる再生/停止
    - ショートカットキー入力による音源の再生/停止
    - リピートボタンによるループ再生のON/OFF
    - シークバーによる再生位置変更
  - **サウンドドライバ関連**
    - 読み込み形式
      - wav
      - mp3
      - flac(できれば)
      - ogg (できれば)
      - その他(できればffmpeg等で対応したい)
    - 再生デバイスの変更
    - サウンドドライバの変更(できれば)
      - WASAPI(デフォルト)
      - DirectSound(できれば)
      - MME(できれば)
    - 
