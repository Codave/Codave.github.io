---
title: NTRU算法的分析
date: 2019-01-23 20:19:19
categories:
- 密码学
tags:
- NTRU
---

## NTRU简述

​       NTRU(Number Theory Research Unit)公开密钥体制是由美国布朗大学三位数学教授(Jeffrey Hoffstein,JillPipher,Joseph H.Silverman)发明的，其安全性是基于数论中在一个非常大的维数格中寻找一个很短向量的数学难题。相对于离散对数或大数分解等公开秘密体制来说，它有许多优势。在安全性方面，NTRU算法具有抵抗量子计算攻击的能力，而RSA和ECC算法是无法抵抗量子计算的。

## NTRU算法的描述

### NTRU算法的数论基础

​       设有整数环Z、整数N$ \geq$2，用R表示多项式截断环时，R可以写成：R=Z[X]/(X^N^-1)，对于任意的正整数q，令R _q_ 代表模q的多项式截断环时，R _q_可以写成：

$$ R _q_ =(Z/ _q_ Z )[X]/(X ^N^ -1)

 可以证明当q时素数时，R具有可逆性。

### NTRU算法的描述