# 理解確認クイズ

## Q1. 次の2つのプロセスを実行したときCounterの値が元の値-1となった。各行はどのような順番で実行されたか。

```
10 COPY AX, COUNTER
12 ADD AX, '1'
14 COPY COUNTER, AX
```

```
20 COPY AX, COUNTER
22 SUB AX, '1'
24 COPY COUNTER, AX
```

20 -> 22 -> 10 -> 12 -> 14 -> 24 の順番
**プロセスは復元される**。

## Q2. TestAndSet命令を、次のようなソフトウェアでは実現できない理由を述べよ。

> [!NOTE]
> TestAndSet命令は機械語の**1命令**で行う。

> [!TIP]
> これならOK

```
bool TestAndSet(bool *target) {
    bool rv = *target;
    *target = true;
    return rv;
}
```

> [!CAUTION]
> これはダメ!

```
bool TestAndSet(bool *target) {
    bool rv = *target;
    if *target == false {
        *target = true;
    }
    return rv;
}
```

Test してから次に Set をしてしまっているから。

## Q3. 略

デッドロックは生じていない。
Aのプロセスが終わると、リソースaとリソースbが解放される。

デッドロックの起きる4条件
- 相互排除: 占有しなくては使えないリソースがある。
- 確保と待機: あるプロセスがあるリソースを確保したままほかのリソースが空くのを待って居る。
- 中断不可: リソースの強制解放はできない。
- 循環待機: 複数プロセス間でリソースの確保とリソースの待ちにサイクルがある。
