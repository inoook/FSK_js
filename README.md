# FSK_js

ブラウザ上で動く、音響データ通信（FSK/OOK）と関連検証ツールの実験用HTML集です。  
各ファイルは単体で開いて使う想定です。

## ファイル一覧と機能

| ファイル | 機能 |
|---|---|
| `fsk-encoder.html` | 初期版の高周波（近超音波）FSK送信ツール。文字列をビット化し、音声再生/WAV保存する。 |
| `fsk-decoder.html` | 初期版の高周波FSK受信ツール。マイク入力またはWAV解析でデータ復号する。 |
| `fsk-decoder-v2.html` | デコーダー改良版。受信UI・解析表示を強化した高周波FSK受信ページ。 |
| `fsk-encoder-v3.html` | FEC（Hamming(7,4)+interleave）とCRC-16対応のFSK送信ページ。チャネルシミュレータ付き。 |
| `fsk-decoder-v3.html` | v3エンコーダー系に対応したFEC復号付きFSK受信ページ。マイク/WAVの両入力に対応。 |
| `fsk-encoder-v4.html` | 2-TONE純サインFSK方式の送信ページ。FEC対応・可聴域寄りパラメータで検証可能。 |
| `fsk-decoder-v4.html` | 2-TONE純サインFSK向け受信ページ。SYNC判定、FEC/RAW判別、CRC確認まで行う。 |
| `fsk-encoder-v5.html` | 畳み込み符号（Conv, rate 1/2）対応のFSK送信ページ。インターリーブとCRCを併用。 |
| `fsk-decoder-v5.html` | v5系の畳み込み符号に対応したFSK受信ページ。復号時の訂正処理を実装。 |
| `fsk-encoder-v6.html` | リードインのLFMチャープ同期付きFSK送信ページ。FECとチャネルシミュレーション対応。 |
| `fsk-decoder-v6.html` | チャープ整合フィルタで同期検出するFSK受信ページ。FEC復号と可視化を強化。 |
| `fsk-encoder-v7.html` | 可聴域向けに調整したv7送信ページ。チャープ同期付きで実環境テストしやすい。 |
| `fsk-decoder-v7.html` | v7可聴域系の受信ページ。チャープ相関表示・ソフト判定・復号確認に対応。 |
| `ook-encoder-v3.html` | OOK（tone=1 / silence=0）方式の送信ページ。FEC/CRCとチャネルシミュレータ付き。 |
| `ook-decoder-v3.html` | OOK方式の受信ページ。トーン有無判定と位相/レート探索で復号する。 |
| `fsk-benchmark-v3.html` | FEC有無（FEC vs RAW）の通信性能を比較するベンチマークページ。 |
| `hz-meter.html` | マイク入力のピーク周波数をリアルタイム表示する周波数メーター。 |
| `vlc-blink.html` | 画面点滅（白黒OOK）とカメラで行う光データ通信実験ページ。 |
| `index.html` | 現状は `html` の1行のみで、ランディングページとしては未実装。 |
