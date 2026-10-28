# KDV Hesaplama Aracı

Vanilla JS ile yazılmış, PWA, offline-first KDV hesaplayıcı.

**Demo:** https://www.invoiceluxe.com/tr/calculator.html

## Problem

`600 - 120 = 480` yanlış, `600 / 1.20 = 500` doğru.

## Çözüm

```js
const net = brut / (1 + kdvOrani); // 600 / 1.20 = 500
const kdv = brut - net; // 100
