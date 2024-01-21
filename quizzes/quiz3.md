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

10 -> 12 -> 20 -> 22 -> 24 -> 14 の順番

## Q2. 

## Q3. 略

デッドロックは生じていない。
Aのプロセスが終わると、リソースaとリソースbが解放される。
