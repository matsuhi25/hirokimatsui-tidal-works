# Patterns vol.1

BandcampでリリースしたPatterns vol.1 (October 22, 2025)のソースコードです


## 実行環境

各トラックの.tidalファイルにより演奏し、一発録りとして収録しました。

orbitごとにマルチトラックとしてDAWに録音し、音量調整やEQ、空間エフェクトの追加などポストプロセスをしています。

Tidalはモジュラー上にマウントしたRaspberryPi (4B, 8GBRAM)で実行しています。


### Code
- d1~d8の各トラックはモノラルにカスタムし、Audio I/OであるES-8から出力しています。
- sound `"midi"`はMutant Brain (Hexinverter)に接続し、モジュールの制御に使っています。
- - Mutant Brainの設定ファイルは`config_files/mb_surgery.syx`です。
- MIDI outputや一部のオーディオはGeneration loss mkIIでプロセスしています。

## 追加予定
- SCD startup file
- modular grid link
- custom samples