# 理解確認クイズ

### Q1. 優先度に基づくプリエンプティブなスケジューリングを行うリアルタイムOSで、二つのタスクA、Bをスケジューリングする。Aの方がＢよりも優先度が高い場合にリアルタイムOSが行う動作のうち、適切なものはどれか。

- [ ] ア Aの実行中にBに起動がかかると、Aを実行可能状態にしてBを実行する。
- [ ] イ Aの実行中にBに起動がかかると、Aを待ち状態にしてBを実行する。
- [x] ウ Bの実行中にAに起動がかかると、Bを実行可能状態にしてAを実行する。
- [ ] ェ Bの実行中にAに起動がかかると、Bを待ち状態にしてAを実行する。


### Q2. タスクのディスパッチの説明として、適切なものはどれか。

- [ ] ア 各タスクの実行順序を決定すること。
- [x] イ 実行可能なタスクに対してプロセッサの使用権を割り当てること。
- [ ] ウ タスクの実行に必要な情報であるコンテキストのこと。
- [ ] ェ 一つのプロセッサで複数のタスクを同時に実行しているかのように見せかける機能のこと。

ディスパッチャ: 実行可能状態(Ready)(CPU時間割当待ち)のプロセスの集合の中から、次にCPU時間を割り当てて実行するプロセスを選ぶこと。
ラウンドロビン方式: 1つのCPUをごく短い時間づつ交代で利用する。

### Q3. デバイスドライバの説明として、適切なものはどれか。

- [x] ア PCに接続された周辺機器を制御するソフトウェア
- [ ] イ アプリケーションプログラムをPCに導入するソフトウェア
- [ ] ウ キーボードなどの操作手順を登録して、その操作を自動化するソフトウェア
- [ ] ェ 他のPCに入り込んで不利益をもたらすソフトウェア

### Q4. 略

- [ ] ア 2
- [x] イ 3
- [ ] ウ 4
- [ ] ェ 5

### Q5. スケジューリングに関する記述のうち、ラウンドロビン方式の説明として、適切なものはどれか。

- [x] ア 各タスクに、均等にCPU時間を割り当てて実行させる方式である。
- [ ] イ 各タスクに、ターンアラウンドタイムに比例したCPU時間を割り当てて実行させる方式である。
- [ ] ウ 各タスクの実行イベント発生に応じて、リアルタイムに実行させる方式である。
- [ ] ェ 各タスクを、優先度の高い順に実行させる方式である。

ェはプリエンプション方式

### Q6. 略

- [ ] ア
- [ ] イ
- [x] ウ
- [ ] ェ

### Q7. 略

- [ ] ア
- [ ] イ
- [x] ウ
- [ ] ェ

実行状態の退避 -> プロセスの選択 -> 実行状態の回復
