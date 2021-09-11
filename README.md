# AtCoder

## TL;DR
C++の勉強としてAtCoderを利用。
そのため基本的にはC++のみでの実装。
記法については42同様、norminetteを通しても可能な状態での提出を目指したい。

## 使用言語
C++のみ

## 使用コンパイラ
GCC

## 入出力
- 入力に関してはcinを使用。
```
cin >> n;
```
- 出力に関してはcoutを使用。
```
cout << n;
```


## 高速化メモ
- コンパイラの自動ベクトル化をサポートさせ、ループ処理をベクトル化し、高速化する。
```
#pragma GCC target("avx")
```
- g++の最適化オプションには -O -O0 -O1 -O2 -O3 -Os -Ofast -Og があるが、-Ofastは厳格な標準準拠を無視してしまう為、-O3を使用。
```
#pragma GCC optimize("O3")
```
- ループの最大回数を分割して減らす（ループ自体の数を増やして、ループ回数を少なくする）コード内のループ回数が多くない時は使用を非推奨。。
```
#pragma GCC optimize("unroll-loops")
```
