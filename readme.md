# soundPlayerモジュール

bassを利用した音声データ再生モジュール


## 概要

　本モジュールは、音声データ再生に関する処理を簡素化する者である。
内部は、pyBass、およびその拡張部分によって構成される。

　bass関連モジュール、および同ライブラリの使用条件は、各配布元にて確認のこと。
https://www.un4seen.com/


## インストール

- pip install https://github.com/actlaboratory/soundPlayer/archive/0.5.4.zip


## 変更履歴

- Version 0.5.4 2023.11.05
	- 不要ファイル削除に伴うpyinstaller使用時の不具合を修正

- Version 0.5.3 2023.10.09
	- Python3.11への対応漏れを修正
	- 不要なファイルを削除

- Version 0.5.2 2023.10.09
	- Python3.11での使用に対応

- Version 0.5.1 2023.02.05
	- URL指定に改行コードが含まれていると正しく動作しない問題を修正（2行目以降はHTTPヘッダー）

- Version 0.5.0 2022.10.03
	- BASSおよび関連ライブラリを最新版に更新した。これでHLS再生が途中で止まったりすることがなくなるはず。

- Version 0.4.0 2022.04.29
	- プロキシ設定機能を追加

- Version 0.3.1 2021.01.02
	- デバイスエラーの判定条件を改善

- Version 0.3.0 2021.01.02
	- ハンドルが生成できない理由がファイル要因の場合、playerが停止状態となるように改善
	- ストリーミングの長さに1を返していた問題に対処

- Version 0.2.4 2020.12.19
	- Appleロスレスに対応
	- WavPackに対応

- Version 0.2.3 2020.12.2
	- デバイスエラー復帰時にステータスが戻らないことがある問題を修正

- Version 0.2.2 2020.11.22
	- EOFを検知できない問題に対処

- Version 0.2.1 2020.11.22
	- デバイス一覧取得の処理を改善

- Version 0.2.0 2020.11.21
	- デバイス異常検知の制度を改善
	- 今後、デバイスエラー検知後、変更先のデバイスでエラーが継続する場合は STATUS_PAUSE を返します。
	- デバイスの正常性を確認する isDeviceOk() を追加

- Version 0.1.0 2020.11.14
	- wma、flac、opusへの対応

- Version 0.0.9 2020.10.24
	- 動作の軽量化

- Version 0.0.8 2020.10.13
	- playerの音量差分調整が適切なリターンを返すように修正
	- ソフトウェアが動作を停止する問題に対処

- Version 0.0.7 2020.09.13
	- fxPlayerにて、デバイス名でも出力先が指定できるように修正
	- 各playerオブジェクトに対し、、デバイス一覧取得が可能になった。

- Version 0.0.6 2020.09.13
	- 存在しないプレイヤーの制御を試みることでエラーとなる不具合を修正

- Version 0.0.5 2020.09.12
	- pyinstaller4.0以降のためのhookを追加

- Version 0.0.1 2020.09.02
	- 初回リリース
