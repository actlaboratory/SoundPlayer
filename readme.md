# soundPlayerモジュール

bassを利用した音声データ再生モジュール


## 概要

　本モジュールは、音声データ再生に関する処理を簡素化する者である。
内部は、pyBass、およびその拡張部分によって構成される。

　bass関連モジュール、および同ライブラリの使用条件は、各配布元にて確認のこと。
https://www.un4seen.com/


## インストール

- pip install https://github.com/actlaboratory/soundPlayer/archive/0.0.6.zip


## 変更履歴

- Version 0.0.6 2020.9.13
	- 存在しないプレイヤーの制御を試みることでエラーとなる不具合を修正

- Version 0.0.5 2020.09.12
	- pyinstaller4.0以降のためのhookを追加

- Version 0.0.1 2020.09.02
	- 初回リリース
