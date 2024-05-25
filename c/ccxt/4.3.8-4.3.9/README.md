# Comparing `tmp/ccxt-4.3.8.tar.gz` & `tmp/ccxt-4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-4.3.8.tar", last modified: Thu Apr 25 18:16:36 2024, max compression
+gzip compressed data, was "dist/ccxt-4.3.9.tar", last modified: Fri Apr 26 17:27:01 2024, max compression
```

## Comparing `ccxt-4.3.8.tar` & `ccxt-4.3.9.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.711214 ccxt-4.3.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-25 18:11:51.000000 ccxt-4.3.8/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-25 16:48:28.000000 ccxt-4.3.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   115320 2024-04-25 18:16:36.719215 ccxt-4.3.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-25 16:48:28.000000 ccxt-4.3.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.063167 ccxt-4.3.8/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15655 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.179175 ccxt-4.3.8/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98736 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16041 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15507 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10977 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10368 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41650 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47182 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151398 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.439194 ccxt-4.3.8/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15408 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41874 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47394 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152186 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.443194 ccxt-4.3.8/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   107190 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.455195 ccxt-4.3.8/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92644 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   614239 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   185234 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42099 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71973 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158868 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41699 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   423787 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45758 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   200028 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   126994 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68920 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136836 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71265 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92765 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102352 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92005 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20605 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49185 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36973 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23680 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51828 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36869 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   411940 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70274 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   207970 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87777 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79171 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35864 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   247930 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103683 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46206 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47132 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91060 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23760 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   130350 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151059 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   161229 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   168860 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115075 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   321438 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81132 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   153964 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76332 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   422776 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88462 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   100190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73435 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32429 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52237 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125943 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117245 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218785 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119225 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    96401 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79527 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115881 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46126 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51378 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35575 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   241987 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   109086 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64667 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151634 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   372441 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88559 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54455 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   219623 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102501 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78194 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76750 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71643 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123369 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24094 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82087 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114100 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51638 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108793 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   139440 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53500 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28139 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80871 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.463196 ccxt-4.3.8/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-25 17:02:53.000000 ccxt-4.3.8/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   275089 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7992 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   611571 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   184198 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41839 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71533 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158134 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41391 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   422163 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45528 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   199108 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   126416 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68516 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136178 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70879 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92265 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102020 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91571 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20477 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48793 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36695 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23486 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51478 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36651 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   410160 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69924 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   206918 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87223 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78665 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35658 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   246642 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103195 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45940 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46890 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90626 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23608 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   129778 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   150451 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160453 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   167890 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114443 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   319760 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80619 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152918 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75898 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   420420 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87962 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99670 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72959 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32169 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51929 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125341 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116757 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   217713 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118623 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95985 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79051 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115169 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45788 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51064 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35333 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   240809 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108562 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64299 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151110 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   370866 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88107 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54213 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218811 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101953 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77808 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.567204 ccxt-4.3.8/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152488 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71843 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58380 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25807 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20791 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60658 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35105 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41652 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30043 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36988 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76358 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/probit.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.571204 ccxt-4.3.8/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.579204 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.579204 ccxt-4.3.8/ccxt/static_dependencies/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.587205 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.591205 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.591205 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.595206 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.595206 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.599206 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.611207 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.651210 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.651210 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.655210 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.659210 ccxt-4.3.8/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.659210 ccxt-4.3.8/ccxt/static_dependencies/msgpack/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.667211 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.671211 ccxt-4.3.8/ccxt/static_dependencies/toolz/
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.675212 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.679212 ccxt-4.3.8/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.711214 ccxt-4.3.8/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-25 17:02:58.000000 ccxt-4.3.8/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-25 17:02:55.000000 ccxt-4.3.8/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-25 17:02:54.000000 ccxt-4.3.8/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_last_price.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_margin_mode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-25 17:02:54.000000 ccxt-4.3.8/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78755 2024-04-25 17:02:58.000000 ccxt-4.3.8/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77736 2024-04-25 17:02:58.000000 ccxt-4.3.8/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71281 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123007 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23900 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81605 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113550 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51336 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108191 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   138550 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53216 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27957 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80557 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.063167 ccxt-4.3.8/ccxt.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)   115320 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12555 2024-04-25 18:11:50.000000 ccxt-4.3.8/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-25 18:16:36.719215 ccxt-4.3.8/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-25 16:48:28.000000 ccxt-4.3.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.266837 ccxt-4.3.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-26 17:25:58.000000 ccxt-4.3.9/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-26 17:01:40.000000 ccxt-4.3.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115320 2024-04-26 17:27:01.266837 ccxt-4.3.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-26 17:01:40.000000 ccxt-4.3.9/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.198836 ccxt-4.3.9/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15655 2024-04-26 17:25:57.000000 ccxt-4.3.9/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.214836 ccxt-4.3.9/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98736 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16032 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15507 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10977 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10368 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-26 17:03:24.000000 ccxt-4.3.9/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41650 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47182 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151398 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.238837 ccxt-4.3.9/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15408 2024-04-26 17:25:57.000000 ccxt-4.3.9/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41874 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47394 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152186 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.238837 ccxt-4.3.9/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   107190 2024-04-26 17:25:57.000000 ccxt-4.3.9/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.238837 ccxt-4.3.9/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92644 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   614239 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   185648 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42099 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71973 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158868 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41699 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   423787 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45758 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   200028 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126994 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68920 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136836 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71265 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92765 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102352 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92005 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20605 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49185 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36973 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23680 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51828 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36869 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   411940 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70274 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   207970 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87777 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79171 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35864 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   259028 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103683 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46206 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80999 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47132 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91060 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23760 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   130350 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151059 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   161229 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   168860 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115075 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   321438 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81132 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   153964 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76332 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   422776 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88462 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100190 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73435 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32429 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52237 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125943 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117245 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218785 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119225 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96401 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79527 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115881 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46126 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51378 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35575 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   241987 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   109086 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64667 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151634 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   375250 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88559 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54455 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   219623 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102501 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78194 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76750 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71643 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123369 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24094 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82087 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114100 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51638 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108793 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   139440 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53500 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28139 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80871 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.238837 ccxt-4.3.9/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-26 17:13:32.000000 ccxt-4.3.9/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   275089 2024-04-26 17:25:57.000000 ccxt-4.3.9/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7992 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92190 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   611571 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   184612 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41839 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71533 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158134 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41391 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   422163 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45528 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   199108 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126416 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68516 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136178 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70879 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92265 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102020 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91571 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20477 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48793 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36695 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23486 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51478 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36651 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   410160 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69924 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   206918 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87223 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78665 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35658 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   257752 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103195 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45940 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80679 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46890 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90626 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23608 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129778 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   150451 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160453 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   167890 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114443 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   319760 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80619 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152918 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75898 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   420420 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87962 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99670 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72959 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32169 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51929 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125341 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116757 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217713 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118623 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95985 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79051 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115169 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45788 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51064 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35333 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   240809 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108562 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64299 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151110 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   373663 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88107 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54213 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218811 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101953 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77808 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.250837 ccxt-4.3.9/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2024-04-26 17:25:57.000000 ccxt-4.3.9/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152488 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71843 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58380 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25807 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20791 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60658 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35105 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41652 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30043 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36988 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76358 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/probit.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.250837 ccxt-4.3.9/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.250837 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.250837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.254837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.258837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.258837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.258837 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.258837 ccxt-4.3.9/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.258837 ccxt-4.3.9/ccxt/static_dependencies/msgpack/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.258837 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.262837 ccxt-4.3.9/ccxt/static_dependencies/toolz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.262837 ccxt-4.3.9/ccxt/static_dependencies/toolz/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/static_dependencies/toolz/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.262837 ccxt-4.3.9/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.266837 ccxt-4.3.9/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-26 17:13:35.000000 ccxt-4.3.9/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-26 17:13:33.000000 ccxt-4.3.9/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-26 17:13:32.000000 ccxt-4.3.9/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_last_price.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_margin_mode.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-26 17:13:32.000000 ccxt-4.3.9/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-26 17:14:39.000000 ccxt-4.3.9/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78755 2024-04-26 17:13:35.000000 ccxt-4.3.9/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77736 2024-04-26 17:13:35.000000 ccxt-4.3.9/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71281 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123007 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23900 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81605 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113550 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51336 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108191 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   138550 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53216 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27957 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80557 2024-04-26 17:01:40.000000 ccxt-4.3.9/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 17:27:01.198836 ccxt-4.3.9/ccxt.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)   115320 2024-04-26 17:27:01.000000 ccxt-4.3.9/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-26 17:27:01.000000 ccxt-4.3.9/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-26 17:27:01.000000 ccxt-4.3.9/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-26 17:27:01.000000 ccxt-4.3.9/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-26 17:27:01.000000 ccxt-4.3.9/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12412 2024-04-26 17:25:58.000000 ccxt-4.3.9/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-26 17:27:01.266837 ccxt-4.3.9/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-26 17:01:40.000000 ccxt-4.3.9/setup.py
```

### Comparing `ccxt-4.3.8/LICENSE.txt` & `ccxt-4.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/PKG-INFO` & `ccxt-4.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.3.8
+Version: 4.3.9
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -222,21 +222,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.3.8/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.9/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.3.9/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.9/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.3.8/README.rst` & `ccxt-4.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/__init__.py` & `ccxt-4.3.9/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.3.8'
+__version__ = '4.3.9'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-4.3.8/ccxt/abstract/ace.py` & `ccxt-4.3.9/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/alpaca.py` & `ccxt-4.3.9/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/ascendex.py` & `ccxt-4.3.9/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bequant.py` & `ccxt-4.3.9/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bigone.py` & `ccxt-4.3.9/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/binance.py` & `ccxt-4.3.9/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/binancecoinm.py` & `ccxt-4.3.9/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/binanceus.py` & `ccxt-4.3.9/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/binanceusdm.py` & `ccxt-4.3.9/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bingx.py` & `ccxt-4.3.9/ccxt/abstract/bingx.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,21 +82,21 @@
     wallets_v1_private_get_capital_subaccount_innertransfer_records = walletsV1PrivateGetCapitalSubAccountInnerTransferRecords = Entry('capital/subAccount/innerTransfer/records', ['wallets', 'v1', 'private'], 'GET', {'cost': 1})
     wallets_v1_private_post_capital_withdraw_apply = walletsV1PrivatePostCapitalWithdrawApply = Entry('capital/withdraw/apply', ['wallets', 'v1', 'private'], 'POST', {'cost': 3})
     wallets_v1_private_post_capital_innertransfer_apply = walletsV1PrivatePostCapitalInnerTransferApply = Entry('capital/innerTransfer/apply', ['wallets', 'v1', 'private'], 'POST', {'cost': 3})
     wallets_v1_private_post_capital_subaccountinnertransfer_apply = walletsV1PrivatePostCapitalSubAccountInnerTransferApply = Entry('capital/subAccountInnerTransfer/apply', ['wallets', 'v1', 'private'], 'POST', {'cost': 3})
     wallets_v1_private_post_capital_deposit_createsubaddress = walletsV1PrivatePostCapitalDepositCreateSubAddress = Entry('capital/deposit/createSubAddress', ['wallets', 'v1', 'private'], 'POST', {'cost': 1})
     subaccount_v1_private_get_list = subAccountV1PrivateGetList = Entry('list', ['subAccount', 'v1', 'private'], 'GET', {'cost': 3})
     subaccount_v1_private_get_assets = subAccountV1PrivateGetAssets = Entry('assets', ['subAccount', 'v1', 'private'], 'GET', {'cost': 3})
-    subaccount_v1_private_get_apikey_query = subAccountV1PrivateGetApiKeyQuery = Entry('apiKey/query', ['subAccount', 'v1', 'private'], 'GET', {'cost': 1})
     subaccount_v1_private_post_create = subAccountV1PrivatePostCreate = Entry('create', ['subAccount', 'v1', 'private'], 'POST', {'cost': 3})
     subaccount_v1_private_post_apikey_create = subAccountV1PrivatePostApiKeyCreate = Entry('apiKey/create', ['subAccount', 'v1', 'private'], 'POST', {'cost': 3})
     subaccount_v1_private_post_apikey_edit = subAccountV1PrivatePostApiKeyEdit = Entry('apiKey/edit', ['subAccount', 'v1', 'private'], 'POST', {'cost': 3})
     subaccount_v1_private_post_apikey_del = subAccountV1PrivatePostApiKeyDel = Entry('apiKey/del', ['subAccount', 'v1', 'private'], 'POST', {'cost': 3})
     subaccount_v1_private_post_updatestatus = subAccountV1PrivatePostUpdateStatus = Entry('updateStatus', ['subAccount', 'v1', 'private'], 'POST', {'cost': 3})
     account_v1_private_get_uid = accountV1PrivateGetUid = Entry('uid', ['account', 'v1', 'private'], 'GET', {'cost': 1})
+    account_v1_private_get_apikey_query = accountV1PrivateGetApiKeyQuery = Entry('apiKey/query', ['account', 'v1', 'private'], 'GET', {'cost': 1})
     account_v1_private_post_innertransfer_authorizesubaccount = accountV1PrivatePostInnerTransferAuthorizeSubAccount = Entry('innerTransfer/authorizeSubAccount', ['account', 'v1', 'private'], 'POST', {'cost': 3})
     user_auth_private_post_userdatastream = userAuthPrivatePostUserDataStream = Entry('userDataStream', ['user', 'auth', 'private'], 'POST', {'cost': 1})
     user_auth_private_put_userdatastream = userAuthPrivatePutUserDataStream = Entry('userDataStream', ['user', 'auth', 'private'], 'PUT', {'cost': 1})
     copytrading_v1_private_get_swap_trace_currenttrack = copyTradingV1PrivateGetSwapTraceCurrentTrack = Entry('swap/trace/currentTrack', ['copyTrading', 'v1', 'private'], 'GET', {'cost': 1})
     copytrading_v1_private_post_swap_trace_closetrackorder = copyTradingV1PrivatePostSwapTraceCloseTrackOrder = Entry('swap/trace/closeTrackOrder', ['copyTrading', 'v1', 'private'], 'POST', {'cost': 1})
     copytrading_v1_private_post_swap_trace_settpsl = copyTradingV1PrivatePostSwapTraceSetTPSL = Entry('swap/trace/setTPSL', ['copyTrading', 'v1', 'private'], 'POST', {'cost': 1})
     copytrading_v1_private_post_spot_trader_sellorder = copyTradingV1PrivatePostSpotTraderSellOrder = Entry('spot/trader/sellOrder', ['copyTrading', 'v1', 'private'], 'POST', {'cost': 1})
```

### Comparing `ccxt-4.3.8/ccxt/abstract/bit2c.py` & `ccxt-4.3.9/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitbank.py` & `ccxt-4.3.9/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitbay.py` & `ccxt-4.3.9/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitbns.py` & `ccxt-4.3.9/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitcoincom.py` & `ccxt-4.3.9/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitfinex.py` & `ccxt-4.3.9/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitfinex2.py` & `ccxt-4.3.9/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitflyer.py` & `ccxt-4.3.9/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitget.py` & `ccxt-4.3.9/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bithumb.py` & `ccxt-4.3.9/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitmart.py` & `ccxt-4.3.9/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitmex.py` & `ccxt-4.3.9/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitopro.py` & `ccxt-4.3.9/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitpanda.py` & `ccxt-4.3.9/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitrue.py` & `ccxt-4.3.9/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitso.py` & `ccxt-4.3.9/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitstamp.py` & `ccxt-4.3.9/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitteam.py` & `ccxt-4.3.9/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bitvavo.py` & `ccxt-4.3.9/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bl3p.py` & `ccxt-4.3.9/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/blockchaincom.py` & `ccxt-4.3.9/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/blofin.py` & `ccxt-4.3.9/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/btcalpha.py` & `ccxt-4.3.9/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/btcbox.py` & `ccxt-4.3.9/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/btcmarkets.py` & `ccxt-4.3.9/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/btcturk.py` & `ccxt-4.3.9/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/bybit.py` & `ccxt-4.3.9/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/cex.py` & `ccxt-4.3.9/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinbase.py` & `ccxt-4.3.9/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinbaseinternational.py` & `ccxt-4.3.9/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinbasepro.py` & `ccxt-4.3.9/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coincheck.py` & `ccxt-4.3.9/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinex.py` & `ccxt-4.3.9/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinlist.py` & `ccxt-4.3.9/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinmate.py` & `ccxt-4.3.9/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinmetro.py` & `ccxt-4.3.9/ccxt/abstract/coinmetro.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     public_get_exchange_prices = publicGetExchangePrices = Entry('exchange/prices', 'public', 'GET', {'cost': 1})
     public_get_exchange_ticks_pair_from = publicGetExchangeTicksPairFrom = Entry('exchange/ticks/{pair}/{from}', 'public', 'GET', {'cost': 3})
     public_get_assets = publicGetAssets = Entry('assets', 'public', 'GET', {'cost': 1})
     public_get_markets = publicGetMarkets = Entry('markets', 'public', 'GET', {'cost': 1})
     public_get_exchange_book_pair = publicGetExchangeBookPair = Entry('exchange/book/{pair}', 'public', 'GET', {'cost': 3})
     public_get_exchange_bookupdates_pair_from = publicGetExchangeBookUpdatesPairFrom = Entry('exchange/bookUpdates/{pair}/{from}', 'public', 'GET', {'cost': 1})
     private_get_users_balances = privateGetUsersBalances = Entry('users/balances', 'private', 'GET', {'cost': 1})
+    private_get_users_wallets = privateGetUsersWallets = Entry('users/wallets', 'private', 'GET', {'cost': 1})
     private_get_users_wallets_history_since = privateGetUsersWalletsHistorySince = Entry('users/wallets/history/{since}', 'private', 'GET', {'cost': 1.67})
     private_get_exchange_orders_status_orderid = privateGetExchangeOrdersStatusOrderID = Entry('exchange/orders/status/{orderID}', 'private', 'GET', {'cost': 1})
     private_get_exchange_orders_active = privateGetExchangeOrdersActive = Entry('exchange/orders/active', 'private', 'GET', {'cost': 1})
     private_get_exchange_orders_history_since = privateGetExchangeOrdersHistorySince = Entry('exchange/orders/history/{since}', 'private', 'GET', {'cost': 1.67})
     private_get_exchange_fills_since = privateGetExchangeFillsSince = Entry('exchange/fills/{since}', 'private', 'GET', {'cost': 1.67})
     private_get_exchange_margin = privateGetExchangeMargin = Entry('exchange/margin', 'private', 'GET', {'cost': 1})
     private_post_jwt = privatePostJwt = Entry('jwt', 'private', 'POST', {'cost': 1})
```

### Comparing `ccxt-4.3.8/ccxt/abstract/coinone.py` & `ccxt-4.3.9/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinsph.py` & `ccxt-4.3.9/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/coinspot.py` & `ccxt-4.3.9/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/cryptocom.py` & `ccxt-4.3.9/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/currencycom.py` & `ccxt-4.3.9/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/delta.py` & `ccxt-4.3.9/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/deribit.py` & `ccxt-4.3.9/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/digifinex.py` & `ccxt-4.3.9/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/exmo.py` & `ccxt-4.3.9/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/fmfwio.py` & `ccxt-4.3.9/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/gate.py` & `ccxt-4.3.9/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/gateio.py` & `ccxt-4.3.9/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/gemini.py` & `ccxt-4.3.9/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/hitbtc.py` & `ccxt-4.3.9/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/hitbtc3.py` & `ccxt-4.3.9/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/hollaex.py` & `ccxt-4.3.9/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/htx.py` & `ccxt-4.3.9/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/huobi.py` & `ccxt-4.3.9/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/huobijp.py` & `ccxt-4.3.9/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/idex.py` & `ccxt-4.3.9/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/independentreserve.py` & `ccxt-4.3.9/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/indodax.py` & `ccxt-4.3.9/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/kraken.py` & `ccxt-4.3.9/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/krakenfutures.py` & `ccxt-4.3.9/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/kucoin.py` & `ccxt-4.3.9/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/kucoinfutures.py` & `ccxt-4.3.9/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/kuna.py` & `ccxt-4.3.9/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/latoken.py` & `ccxt-4.3.9/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/lbank.py` & `ccxt-4.3.9/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/luno.py` & `ccxt-4.3.9/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/lykke.py` & `ccxt-4.3.9/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/mercado.py` & `ccxt-4.3.9/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/mexc.py` & `ccxt-4.3.9/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/ndax.py` & `ccxt-4.3.9/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/novadax.py` & `ccxt-4.3.9/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/oceanex.py` & `ccxt-4.3.9/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/okcoin.py` & `ccxt-4.3.9/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/okx.py` & `ccxt-4.3.9/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/onetrading.py` & `ccxt-4.3.9/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/p2b.py` & `ccxt-4.3.9/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/paymium.py` & `ccxt-4.3.9/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/phemex.py` & `ccxt-4.3.9/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/poloniex.py` & `ccxt-4.3.9/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/poloniexfutures.py` & `ccxt-4.3.9/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/probit.py` & `ccxt-4.3.9/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/timex.py` & `ccxt-4.3.9/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/tokocrypto.py` & `ccxt-4.3.9/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/tradeogre.py` & `ccxt-4.3.9/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/upbit.py` & `ccxt-4.3.9/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/wavesexchange.py` & `ccxt-4.3.9/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/wazirx.py` & `ccxt-4.3.9/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/whitebit.py` & `ccxt-4.3.9/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/woo.py` & `ccxt-4.3.9/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/yobit.py` & `ccxt-4.3.9/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/zaif.py` & `ccxt-4.3.9/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/abstract/zonda.py` & `ccxt-4.3.9/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/ace.py` & `ccxt-4.3.9/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/alpaca.py` & `ccxt-4.3.9/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/ascendex.py` & `ccxt-4.3.9/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/__init__.py` & `ccxt-4.3.9/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.3.8'
+__version__ = '4.3.9'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-4.3.8/ccxt/async_support/ace.py` & `ccxt-4.3.9/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/alpaca.py` & `ccxt-4.3.9/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/ascendex.py` & `ccxt-4.3.9/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/exchange.py` & `ccxt-4.3.9/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.3.8'
+__version__ = '4.3.9'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-4.3.8/ccxt/async_support/base/throttler.py` & `ccxt-4.3.9/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/__init__.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/cache.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/client.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/fast_client.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/functions.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/future.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/order_book.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-4.3.9/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bequant.py` & `ccxt-4.3.9/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bigone.py` & `ccxt-4.3.9/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/binance.py` & `ccxt-4.3.9/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/binancecoinm.py` & `ccxt-4.3.9/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/binanceus.py` & `ccxt-4.3.9/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/binanceusdm.py` & `ccxt-4.3.9/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bingx.py` & `ccxt-4.3.9/ccxt/async_support/bingx.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,14 @@
                 },
                 'subAccount': {
                     'v1': {
                         'private': {
                             'get': {
                                 'list': 3,
                                 'assets': 3,
-                                'apiKey/query': 1,
                             },
                             'post': {
                                 'create': 3,
                                 'apiKey/create': 3,
                                 'apiKey/edit': 3,
                                 'apiKey/del': 3,
                                 'updateStatus': 3,
@@ -317,14 +316,15 @@
                     },
                 },
                 'account': {
                     'v1': {
                         'private': {
                             'get': {
                                 'uid': 1,
+                                'apiKey/query': 1,
                             },
                             'post': {
                                 'innerTransfer/authorizeSubAccount': 3,
                             },
                         },
                     },
                 },
@@ -1752,27 +1752,32 @@
         request: dict = {
             'symbol': market['id'],
             'type': type,
             'side': side.upper(),
         }
         isMarketOrder = type == 'MARKET'
         isSpot = marketType == 'spot'
+        stopLossPrice = self.safe_string(params, 'stopLossPrice')
+        takeProfitPrice = self.safe_string(params, 'takeProfitPrice')
+        triggerPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
+        isTriggerOrder = triggerPrice is not None
+        isStopLossPriceOrder = stopLossPrice is not None
+        isTakeProfitPriceOrder = takeProfitPrice is not None
         exchangeClientOrderId = 'newClientOrderId' if isSpot else 'clientOrderID'
         clientOrderId = self.safe_string_2(params, exchangeClientOrderId, 'clientOrderId')
         if clientOrderId is not None:
             request[exchangeClientOrderId] = clientOrderId
         timeInForce = self.safe_string_upper(params, 'timeInForce')
         postOnly, params = self.handle_post_only(isMarketOrder, timeInForce == 'PostOnly', params)
         if postOnly or (timeInForce == 'PostOnly'):
             request['timeInForce'] = 'PostOnly'
         elif timeInForce == 'IOC':
             request['timeInForce'] = 'IOC'
         elif timeInForce == 'GTC':
             request['timeInForce'] = 'GTC'
-        triggerPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
         if isSpot:
             cost = self.safe_number_2(params, 'cost', 'quoteOrderQty')
             params = self.omit(params, 'cost')
             if cost is not None:
                 request['quoteOrderQty'] = self.parse_to_numeric(self.cost_to_precision(symbol, cost))
             else:
                 if isMarketOrder and (price is not None):
@@ -1787,25 +1792,27 @@
                 if isMarketOrder and self.safe_string(request, 'quoteOrderQty') is None:
                     raise ArgumentsRequired(self.id + ' createOrder() requires the cost parameter(or the amount + price) for placing spot market-buy trigger orders')
                 request['stopPrice'] = self.price_to_precision(symbol, triggerPrice)
                 if type == 'LIMIT':
                     request['type'] = 'TRIGGER_LIMIT'
                 elif type == 'MARKET':
                     request['type'] = 'TRIGGER_MARKET'
+            elif (stopLossPrice is not None) or (takeProfitPrice is not None):
+                stopTakePrice = stopLossPrice if (stopLossPrice is not None) else takeProfitPrice
+                if type == 'LIMIT':
+                    request['type'] = 'TAKE_STOP_LIMIT'
+                elif type == 'MARKET':
+                    request['type'] = 'TAKE_STOP_MARKET'
+                request['stopPrice'] = self.parse_to_numeric(self.price_to_precision(symbol, stopTakePrice))
         else:
             if timeInForce == 'FOK':
                 request['timeInForce'] = 'FOK'
-            stopLossPrice = self.safe_string(params, 'stopLossPrice')
-            takeProfitPrice = self.safe_string(params, 'takeProfitPrice')
             trailingAmount = self.safe_string(params, 'trailingAmount')
             trailingPercent = self.safe_string_2(params, 'trailingPercent', 'priceRate')
             trailingType = self.safe_string(params, 'trailingType', 'TRAILING_STOP_MARKET')
-            isTriggerOrder = triggerPrice is not None
-            isStopLossPriceOrder = stopLossPrice is not None
-            isTakeProfitPriceOrder = takeProfitPrice is not None
             isTrailingAmountOrder = trailingAmount is not None
             isTrailingPercentOrder = trailingPercent is not None
             isTrailing = isTrailingAmountOrder or isTrailingPercentOrder
             stopLoss = self.safe_value(params, 'stopLoss')
             takeProfit = self.safe_value(params, 'takeProfit')
             isStopLoss = stopLoss is not None
             isTakeProfit = takeProfit is not None
@@ -1875,15 +1882,15 @@
             positionSide = None
             if reduceOnly:
                 positionSide = 'SHORT' if (side == 'buy') else 'LONG'
             else:
                 positionSide = 'LONG' if (side == 'buy') else 'SHORT'
             request['positionSide'] = positionSide
             request['quantity'] = self.parse_to_numeric(self.amount_to_precision(symbol, amount))
-            params = self.omit(params, ['reduceOnly', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice', 'trailingAmount', 'trailingPercent', 'trailingType', 'takeProfit', 'stopLoss', 'clientOrderId'])
+        params = self.omit(params, ['reduceOnly', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice', 'trailingAmount', 'trailingPercent', 'trailingType', 'takeProfit', 'stopLoss', 'clientOrderId'])
         return self.extend(request, params)
 
     async def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
         """
         create a trade order
         :see: https://bingx-api.github.io/docs/#/en-us/swapV2/trade-api.html#Trade%20order
         :see: https://bingx-api.github.io/docs/#/en-us/spot/trade-api.html#Create%20an%20Order
@@ -1893,17 +1900,17 @@
         :param float amount: how much you want to trade in units of the base currency
         :param float [price]: the price at which the order is to be fullfilled, in units of the quote currency, ignored in market orders
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.clientOrderId]: a unique id for the order
         :param bool [params.postOnly]: True to place a post only order
         :param str [params.timeInForce]: spot supports 'PO', 'GTC' and 'IOC', swap supports 'PO', 'GTC', 'IOC' and 'FOK'
         :param bool [params.reduceOnly]: *swap only* True or False whether the order is reduce only
-        :param float [params.triggerPrice]: *swap only* triggerPrice at which the attached take profit / stop loss order will be triggered
-        :param float [params.stopLossPrice]: *swap only* stop loss trigger price
-        :param float [params.takeProfitPrice]: *swap only* take profit trigger price
+        :param float [params.triggerPrice]: triggerPrice at which the attached take profit / stop loss order will be triggered
+        :param float [params.stopLossPrice]: stop loss trigger price
+        :param float [params.takeProfitPrice]: take profit trigger price
         :param float [params.cost]: the quote quantity that can be used alternative for the amount
         :param float [params.trailingAmount]: *swap only* the quote amount to trail away from the current market price
         :param float [params.trailingPercent]: *swap only* the percent to trail away from the current market price
         :param dict [params.takeProfit]: *takeProfit object in params* containing the triggerPrice at which the attached take profit order will be triggered
         :param float [params.takeProfit.triggerPrice]: take profit trigger price
         :param dict [params.stopLoss]: *stopLoss object in params* containing the triggerPrice at which the attached stop loss order will be triggered
         :param float [params.stopLoss.triggerPrice]: stop loss trigger price
```

### Comparing `ccxt-4.3.8/ccxt/async_support/bit2c.py` & `ccxt-4.3.9/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitbank.py` & `ccxt-4.3.9/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitbns.py` & `ccxt-4.3.9/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitcoincom.py` & `ccxt-4.3.9/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitfinex.py` & `ccxt-4.3.9/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitfinex2.py` & `ccxt-4.3.9/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitflyer.py` & `ccxt-4.3.9/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitget.py` & `ccxt-4.3.9/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bithumb.py` & `ccxt-4.3.9/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitmart.py` & `ccxt-4.3.9/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitmex.py` & `ccxt-4.3.9/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitopro.py` & `ccxt-4.3.9/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitrue.py` & `ccxt-4.3.9/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitso.py` & `ccxt-4.3.9/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitstamp.py` & `ccxt-4.3.9/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitteam.py` & `ccxt-4.3.9/ccxt/async_support/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bitvavo.py` & `ccxt-4.3.9/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bl3p.py` & `ccxt-4.3.9/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/blockchaincom.py` & `ccxt-4.3.9/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/blofin.py` & `ccxt-4.3.9/ccxt/async_support/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/btcalpha.py` & `ccxt-4.3.9/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/btcbox.py` & `ccxt-4.3.9/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/btcmarkets.py` & `ccxt-4.3.9/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/btcturk.py` & `ccxt-4.3.9/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/bybit.py` & `ccxt-4.3.9/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/cex.py` & `ccxt-4.3.9/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinbase.py` & `ccxt-4.3.9/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinbaseinternational.py` & `ccxt-4.3.9/ccxt/async_support/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinbasepro.py` & `ccxt-4.3.9/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coincheck.py` & `ccxt-4.3.9/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinex.py` & `ccxt-4.3.9/ccxt/coinex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
-from ccxt.async_support.base.exchange import Exchange
+from ccxt.base.exchange import Exchange
 from ccxt.abstract.coinex import ImplicitAPI
-import asyncio
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, Leverages, MarginModification, Market, Num, Order, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
@@ -489,16 +488,16 @@
                 'broad': {
                     'ip not allow visit': PermissionDenied,
                     'service too busy': ExchangeNotAvailable,
                 },
             },
         })
 
-    async def fetch_currencies(self, params={}) -> Currencies:
-        response = await self.v1PublicGetCommonAssetConfig(params)
+    def fetch_currencies(self, params={}) -> Currencies:
+        response = self.v1PublicGetCommonAssetConfig(params)
         #     {
         #         "code": 0,
         #         "data": {
         #             "USDT-ERC20": {
         #                  "asset": "USDT",
         #                  "chain": "ERC20",
         #                  "withdrawal_precision": 6,
@@ -612,33 +611,33 @@
             result[code]['info'] = info
             result[code]['fee'] = self.parse_number(minFeeString)
             result[code]['precision'] = self.parse_number(minPrecisionString)
             result[code]['limits']['deposit']['min'] = self.parse_number(minDepositString)
             result[code]['limits']['withdraw']['min'] = self.parse_number(minWithdrawString)
         return result
 
-    async def fetch_markets(self, params={}) -> List[Market]:
+    def fetch_markets(self, params={}) -> List[Market]:
         """
         retrieves data on all markets for coinex
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of objects representing market data
         """
         promisesUnresolved = [
             self.fetch_spot_markets(params),
             self.fetch_contract_markets(params),
         ]
-        promises = await asyncio.gather(*promisesUnresolved)
+        promises = promisesUnresolved
         spotMarkets = promises[0]
         swapMarkets = promises[1]
         return self.array_concat(spotMarkets, swapMarkets)
 
-    async def fetch_spot_markets(self, params):
-        response = await self.v2PublicGetSpotMarket(params)
+    def fetch_spot_markets(self, params):
+        response = self.v2PublicGetSpotMarket(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "base_ccy": "SORA",
         #                 "base_ccy_precision": 8,
@@ -714,16 +713,16 @@
                     },
                 },
                 'created': None,
                 'info': market,
             })
         return result
 
-    async def fetch_contract_markets(self, params):
-        response = await self.v2PublicGetFuturesMarket(params)
+    def fetch_contract_markets(self, params):
+        response = self.v2PublicGetFuturesMarket(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "base_ccy": "BTC",
         #                 "base_ccy_precision": 8,
@@ -870,33 +869,33 @@
             'percentage': None,
             'average': None,
             'baseVolume': self.safe_string(ticker, 'volume'),
             'quoteVolume': None,
             'info': ticker,
         }, market)
 
-    async def fetch_ticker(self, symbol: str, params={}) -> Ticker:
+    def fetch_ticker(self, symbol: str, params={}) -> Ticker:
         """
         fetches a price ticker, a statistical calculation with the information calculated over the past 24 hours for a specific market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-ticker
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-ticker
         :param str symbol: unified symbol of the market to fetch the ticker for
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `ticker structure <https://docs.ccxt.com/#/?id=ticker-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
         response = None
         if market['swap']:
-            response = await self.v2PublicGetFuturesTicker(self.extend(request, params))
+            response = self.v2PublicGetFuturesTicker(self.extend(request, params))
         else:
-            response = await self.v2PublicGetSpotTicker(self.extend(request, params))
+            response = self.v2PublicGetSpotTicker(self.extend(request, params))
         #
         # Spot
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -940,35 +939,35 @@
         #         "message": "OK"
         #     }
         #
         data = self.safe_list(response, 'data', [])
         result = self.safe_dict(data, 0, {})
         return self.parse_ticker(result, market)
 
-    async def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
+    def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
         """
         fetches price tickers for multiple markets, statistical information calculated over the past 24 hours for each market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-ticker
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-ticker
         :param str[]|None symbols: unified symbols of the markets to fetch the ticker for, all market tickers are returned if not assigned
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `ticker structures <https://docs.ccxt.com/#/?id=ticker-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         symbols = self.market_symbols(symbols)
         market = None
         if symbols is not None:
             symbol = self.safe_value(symbols, 0)
             market = self.market(symbol)
         marketType, query = self.handle_market_type_and_params('fetchTickers', market, params)
         response = None
         if marketType == 'swap':
-            response = await self.v2PublicGetFuturesTicker(query)
+            response = self.v2PublicGetFuturesTicker(query)
         else:
-            response = await self.v2PublicGetSpotTicker(query)
+            response = self.v2PublicGetSpotTicker(query)
         #
         # Spot
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -1011,56 +1010,56 @@
         #         ],
         #         "message": "OK"
         #     }
         #
         data = self.safe_list(response, 'data', [])
         return self.parse_tickers(data, symbols)
 
-    async def fetch_time(self, params={}):
+    def fetch_time(self, params={}):
         """
         fetches the current integer timestamp in milliseconds from the exchange server
         :see: https://docs.coinex.com/api/v2/common/http/time
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns int: the current integer timestamp in milliseconds from the exchange server
         """
-        response = await self.v2PublicGetTime(params)
+        response = self.v2PublicGetTime(params)
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "timestamp": 1711699867777
         #         },
         #         "message": "OK"
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         return self.safe_integer(data, 'timestamp')
 
-    async def fetch_order_book(self, symbol: str, limit: Int = 20, params={}):
+    def fetch_order_book(self, symbol: str, limit: Int = 20, params={}):
         """
         fetches information on open orders with bid(buy) and ask(sell) prices, volumes and other data
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-depth
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-depth
         :param str symbol: unified symbol of the market to fetch the order book for
         :param int [limit]: the maximum amount of order book entries to return
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: A dictionary of `order book structures <https://docs.ccxt.com/#/?id=order-book-structure>` indexed by market symbols
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if limit is None:
             limit = 20  # default
         request = {
             'market': market['id'],
             'limit': limit,
             'interval': '0',
         }
         response = None
         if market['swap']:
-            response = await self.v2PublicGetFuturesDepth(self.extend(request, params))
+            response = self.v2PublicGetFuturesDepth(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": {
             #             "depth": {
             #                 "asks": [
             #                     ["70851.94", "0.2119"],
@@ -1079,15 +1078,15 @@
             #             "is_full": True,
             #             "market": "BTCUSDT"
             #         },
             #         "message": "OK"
             #     }
             #
         else:
-            response = await self.v2PublicGetSpotDepth(self.extend(request, params))
+            response = self.v2PublicGetSpotDepth(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": {
             #             "depth": {
             #                 "asks": [
             #                     ["70875.31", "0.28670282"],
@@ -1226,38 +1225,38 @@
             'takerOrMaker': takerOrMaker,
             'price': priceString,
             'amount': amountString,
             'cost': costString,
             'fee': fee,
         }, market)
 
-    async def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
+    def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
         """
         get the list of the most recent trades for a particular symbol
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-deals
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-deals
         :param str symbol: unified symbol of the market to fetch trades for
         :param int [since]: timestamp in ms of the earliest trade to fetch
         :param int [limit]: the maximum amount of trades to fetch
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Trade[]: a list of `trade structures <https://docs.ccxt.com/#/?id=public-trades>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             # 'last_id': 0,
         }
         if limit is not None:
             request['limit'] = limit
         response = None
         if market['swap']:
-            response = await self.v2PublicGetFuturesDeals(self.extend(request, params))
+            response = self.v2PublicGetFuturesDeals(self.extend(request, params))
         else:
-            response = await self.v2PublicGetSpotDeals(self.extend(request, params))
+            response = self.v2PublicGetSpotDeals(self.extend(request, params))
         #
         # Spot and Swap
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -1269,31 +1268,31 @@
         #             },
         #         ],
         #         "message": "OK"
         #     }
         #
         return self.parse_trades(response['data'], market, since, limit)
 
-    async def fetch_trading_fee(self, symbol: str, params={}) -> TradingFeeInterface:
+    def fetch_trading_fee(self, symbol: str, params={}) -> TradingFeeInterface:
         """
         fetch the trading fees for a market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `fee structure <https://docs.ccxt.com/#/?id=fee-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
         response = None
         if market['spot']:
-            response = await self.v2PublicGetSpotMarket(self.extend(request, params))
+            response = self.v2PublicGetSpotMarket(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1307,15 +1306,15 @@
             #                 "taker_fee_rate": "0.002"
             #             }
             #         ],
             #         "message": "OK"
             #     }
             #
         else:
-            response = await self.v2PublicGetFuturesMarket(self.extend(request, params))
+            response = self.v2PublicGetFuturesMarket(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1333,28 +1332,28 @@
             #         "message": "OK"
             #     }
             #
         data = self.safe_list(response, 'data', [])
         result = self.safe_dict(data, 0, {})
         return self.parse_trading_fee(result, market)
 
-    async def fetch_trading_fees(self, params={}) -> TradingFees:
+    def fetch_trading_fees(self, params={}) -> TradingFees:
         """
         fetch the trading fees for multiple markets
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `fee structures <https://docs.ccxt.com/#/?id=fee-structure>` indexed by market symbols
         """
-        await self.load_markets()
+        self.load_markets()
         type = None
         type, params = self.handle_market_type_and_params('fetchTradingFees', None, params)
         response = None
         if type == 'swap':
-            response = await self.v2PublicGetFuturesMarket(params)
+            response = self.v2PublicGetFuturesMarket(params)
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1369,15 +1368,15 @@
             #                 "taker_fee_rate": "0"
             #             }
             #         ],
             #         "message": "OK"
             #     }
             #
         else:
-            response = await self.v2PublicGetSpotMarket(params)
+            response = self.v2PublicGetSpotMarket(params)
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1434,39 +1433,39 @@
             self.safe_number(ohlcv, 'open'),
             self.safe_number(ohlcv, 'high'),
             self.safe_number(ohlcv, 'low'),
             self.safe_number(ohlcv, 'close'),
             self.safe_number(ohlcv, 'value'),
         ]
 
-    async def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
+    def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
         """
         fetches historical candlestick data containing the open, high, low, and close price, and the volume of a market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-kline
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-kline
         :param str symbol: unified symbol of the market to fetch OHLCV data for
         :param str timeframe: the length of time each candle represents
         :param int [since]: timestamp in ms of the earliest candle to fetch
         :param int [limit]: the maximum amount of candles to fetch
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns int[][]: A list of candles ordered, open, high, low, close, volume
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'period': self.safe_string(self.timeframes, timeframe, timeframe),
         }
         if limit is not None:
             request['limit'] = limit
         response = None
         if market['swap']:
-            response = await self.v2PublicGetFuturesKline(self.extend(request, params))
+            response = self.v2PublicGetFuturesKline(self.extend(request, params))
         else:
-            response = await self.v2PublicGetSpotKline(self.extend(request, params))
+            response = self.v2PublicGetSpotKline(self.extend(request, params))
         #
         # Spot and Swap
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -1482,17 +1481,17 @@
         #         ],
         #         "message": "OK"
         #     }
         #
         data = self.safe_list(response, 'data', [])
         return self.parse_ohlcvs(data, market, timeframe, since, limit)
 
-    async def fetch_margin_balance(self, params={}):
-        await self.load_markets()
-        response = await self.v2PrivateGetAssetsMarginBalance(params)
+    def fetch_margin_balance(self, params={}):
+        self.load_markets()
+        response = self.v2PrivateGetAssetsMarginBalance(params)
         #
         #     {
         #         "data": [
         #             {
         #                 "margin_account": "BTCUSDT",
         #                 "base_ccy": "BTC",
         #                 "quote_ccy": "USDT",
@@ -1535,17 +1534,17 @@
             baseAccount['used'] = self.safe_string(used, 'base_ccy')
             baseDebt = self.safe_string(loan, 'base_ccy')
             baseInterest = self.safe_string(interest, 'base_ccy')
             baseAccount['debt'] = Precise.string_add(baseDebt, baseInterest)
             result[baseCurrencyCode] = baseAccount
         return self.safe_balance(result)
 
-    async def fetch_spot_balance(self, params={}):
-        await self.load_markets()
-        response = await self.v2PrivateGetAssetsSpotBalance(params)
+    def fetch_spot_balance(self, params={}):
+        self.load_markets()
+        response = self.v2PrivateGetAssetsSpotBalance(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "available": "0.00000046",
         #                 "ccy": "USDT",
@@ -1563,17 +1562,17 @@
             code = self.safe_currency_code(currencyId)
             account = self.account()
             account['free'] = self.safe_string(entry, 'available')
             account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
-    async def fetch_swap_balance(self, params={}):
-        await self.load_markets()
-        response = await self.v2PrivateGetAssetsFuturesBalance(params)
+    def fetch_swap_balance(self, params={}):
+        self.load_markets()
+        response = self.v2PrivateGetAssetsFuturesBalance(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "available": "0.00000046",
         #                 "ccy": "USDT",
@@ -1594,17 +1593,17 @@
             code = self.safe_currency_code(currencyId)
             account = self.account()
             account['free'] = self.safe_string(entry, 'available')
             account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
-    async def fetch_financial_balance(self, params={}):
-        await self.load_markets()
-        response = await self.v2PrivateGetAssetsFinancialBalance(params)
+    def fetch_financial_balance(self, params={}):
+        self.load_markets()
+        response = self.v2PrivateGetAssetsFinancialBalance(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "available": "0.00000046",
         #                 "ccy": "USDT",
@@ -1622,15 +1621,15 @@
             code = self.safe_currency_code(currencyId)
             account = self.account()
             account['free'] = self.safe_string(entry, 'available')
             account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
-    async def fetch_balance(self, params={}) -> Balances:
+    def fetch_balance(self, params={}) -> Balances:
         """
         query for balance and get the amount of funds available for trading or funds locked in orders
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-spot-balance         # spot
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-futures-balance      # swap
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-marigin-balance      # margin
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-financial-balance    # financial
         :param dict [params]: extra parameters specific to the exchange API endpoint
@@ -1640,21 +1639,21 @@
         marketType = None
         marketType, params = self.handle_market_type_and_params('fetchBalance', None, params)
         marginMode = None
         marginMode, params = self.handle_margin_mode_and_params('fetchBalance', params)
         marketType = 'margin' if (marginMode is not None) else marketType
         params = self.omit(params, 'margin')
         if marketType == 'margin':
-            return await self.fetch_margin_balance(params)
+            return self.fetch_margin_balance(params)
         elif marketType == 'swap':
-            return await self.fetch_swap_balance(params)
+            return self.fetch_swap_balance(params)
         elif marketType == 'financial':
-            return await self.fetch_financial_balance(params)
+            return self.fetch_financial_balance(params)
         else:
-            return await self.fetch_spot_balance(params)
+            return self.fetch_spot_balance(params)
 
     def parse_order_status(self, status):
         statuses = {
             'rejected': 'rejected',
             'open': 'open',
             'not_deal': 'open',
             'part_deal': 'open',
@@ -1685,15 +1684,15 @@
         #         "price": "170.00000000",
         #         "status": "done",
         #         "taker_fee_rate": "0.0005",
         #         "type": "sell",
         #         "client_id": "",
         #     }
         #
-        # Spot and Margin createOrder, createOrders, cancelOrder, cancelOrders, fetchOrder
+        # Spot and Margin cancelOrder, cancelOrders, fetchOrder
         #
         #      {
         #          "amount":"1.5",
         #          "asset_fee":"0",
         #          "avg_price":"0.14208538",
         #          "client_id":"",
         #          "create_time":1650993819,
@@ -1713,15 +1712,15 @@
         #          "status":"done",
         #          "stock_fee":"0",
         #          "taker_fee_rate":"0.002",
         #          "type":"buy"
         #          "client_id": "",
         #      }
         #
-        # Swap createOrder, cancelOrder, fetchOrder
+        # Swap cancelOrder, fetchOrder
         #
         #     {
         #         "amount": "0.0005",
         #         "client_id": "",
         #         "create_time": 1651004578.618224,
         #         "deal_asset_fee": "0.00000000000000000000",
         #         "deal_fee": "0.00000000000000000000",
@@ -1750,18 +1749,14 @@
         #         "taker_fee": "0.00050",
         #         "target": 0,
         #         "type": 1,
         #         "update_time": 1651004578.618224,
         #         "user_id": 3620173
         #     }
         #
-        # Stop order createOrder
-        #
-        #     {"status":"success"}
-        #
         # Swap Stop cancelOrder, fetchOrder
         #
         #     {
         #         "amount": "0.0005",
         #         "client_id": "",
         #         "create_time": 1651034023.008771,
         #         "effect_type": 1,
@@ -1926,166 +1921,257 @@
         #         "taker_fee": "0.00050",
         #         "target": 0,
         #         "type": 1,
         #         "update_time": 1701233721.718884,
         #         "user_id": 3620173
         #     }
         #
+        # Spot and Margin createOrder, createOrders v2
+        #
+        #     {
+        #         "amount": "0.0001",
+        #         "base_fee": "0",
+        #         "ccy": "BTC",
+        #         "client_id": "x-167673045-a0a3c6461459a801",
+        #         "created_at": 1714114386250,
+        #         "discount_fee": "0",
+        #         "filled_amount": "0",
+        #         "filled_value": "0",
+        #         "last_fill_amount": "0",
+        #         "last_fill_price": "0",
+        #         "maker_fee_rate": "0.002",
+        #         "market": "BTCUSDT",
+        #         "market_type": "SPOT",
+        #         "order_id": 117178743547,
+        #         "price": "61000",
+        #         "quote_fee": "0",
+        #         "side": "buy",
+        #         "taker_fee_rate": "0.002",
+        #         "type": "limit",
+        #         "unfilled_amount": "0.0001",
+        #         "updated_at": 1714114386250
+        #     }
+        #
+        # Spot, Margin and Swap trigger createOrder, createOrders v2
+        #
+        #     {
+        #         "stop_id": 117180138153
+        #     }
+        #
+        # Swap createOrder, createOrders v2
+        #
+        #     {
+        #         "amount": "0.0001",
+        #         "client_id": "x-167673045-1471b81d747080a0",
+        #         "created_at": 1714116769986,
+        #         "fee": "0",
+        #         "fee_ccy": "USDT",
+        #         "filled_amount": "0",
+        #         "filled_value": "0",
+        #         "last_filled_amount": "0",
+        #         "last_filled_price": "0",
+        #         "maker_fee_rate": "0.0003",
+        #         "market": "BTCUSDT",
+        #         "market_type": "FUTURES",
+        #         "order_id": 136913377780,
+        #         "price": "61000.42",
+        #         "realized_pnl": "0",
+        #         "side": "buy",
+        #         "taker_fee_rate": "0.0005",
+        #         "type": "limit",
+        #         "unfilled_amount": "0.0001",
+        #         "updated_at": 1714116769986
+        #     }
+        #
+        # Swap stopLossPrice and takeProfitPrice createOrder v2
+        #
+        #     {
+        #         "adl_level": 1,
+        #         "ath_margin_size": "2.14586666",
+        #         "ath_position_amount": "0.0001",
+        #         "avg_entry_price": "64376",
+        #         "bkr_price": "0",
+        #         "close_avbl": "0.0001",
+        #         "cml_position_value": "6.4376",
+        #         "created_at": 1714119054558,
+        #         "leverage": "3",
+        #         "liq_price": "0",
+        #         "maintenance_margin_rate": "0.005",
+        #         "maintenance_margin_value": "0.03218632",
+        #         "margin_avbl": "2.14586666",
+        #         "margin_mode": "cross",
+        #         "market": "BTCUSDT",
+        #         "market_type": "FUTURES",
+        #         "max_position_value": "6.4376",
+        #         "open_interest": "0.0001",
+        #         "position_id": 303884204,
+        #         "position_margin_rate": "3.10624785634397912265",
+        #         "realized_pnl": "-0.0032188",
+        #         "settle_price": "64376",
+        #         "settle_value": "6.4376",
+        #         "side": "long",
+        #         "stop_loss_price": "62000",
+        #         "stop_loss_type": "latest_price",
+        #         "take_profit_price": "0",
+        #         "take_profit_type": "",
+        #         "unrealized_pnl": "0",
+        #         "updated_at": 1714119054559
+        #     }
+        #
         rawStatus = self.safe_string(order, 'status')
         timestamp = self.safe_timestamp(order, 'create_time')
+        if timestamp is None:
+            timestamp = self.safe_integer(order, 'created_at')
+        update = self.safe_timestamp(order, 'update_time')
+        if update is None:
+            update = self.safe_integer(order, 'updated_at')
         marketId = self.safe_string(order, 'market')
         defaultType = self.safe_string(self.options, 'defaultType')
         orderType = 'swap' if ('source' in order) else defaultType
         market = self.safe_market(marketId, market, None, orderType)
-        feeCurrencyId = self.safe_string(order, 'fee_asset')
+        feeCurrencyId = self.safe_string_2(order, 'fee_asset', 'fee_ccy')
         feeCurrency = self.safe_currency_code(feeCurrencyId)
         if feeCurrency is None:
             feeCurrency = market['quote']
-        rawSide = self.safe_integer(order, 'side')
+        rawIntegerSide = self.safe_integer(order, 'side')
+        rawStringSide = self.safe_string(order, 'side')
         side: Str = None
-        if rawSide == 1:
+        if rawIntegerSide == 1:
             side = 'sell'
-        elif rawSide == 2:
+        elif rawIntegerSide == 2:
             side = 'buy'
+        elif (rawStringSide == 'buy') or (rawStringSide == 'sell'):
+            side = rawStringSide
         else:
             side = self.safe_string(order, 'type')
         rawType = self.safe_string(order, 'order_type')
         type: Str = None
         if rawType is None:
             typeInteger = self.safe_integer(order, 'type')
+            typeString = self.safe_string(order, 'type')
             if typeInteger == 1:
                 type = 'limit'
             elif typeInteger == 2:
                 type = 'market'
+            elif (typeString == 'limit') or (typeString == 'market'):
+                type = typeString
+            elif typeString == 'maker_only':
+                type = 'limit'
         else:
             type = rawType
         clientOrderId = self.safe_string(order, 'client_id')
         if clientOrderId == '':
             clientOrderId = None
         return self.safe_order({
-            'id': self.safe_string_2(order, 'id', 'order_id'),
+            'id': self.safe_string_n(order, ['id', 'order_id', 'stop_id']),
             'clientOrderId': clientOrderId,
             'datetime': self.iso8601(timestamp),
             'timestamp': timestamp,
-            'lastTradeTimestamp': self.safe_timestamp(order, 'update_time'),
+            'lastTradeTimestamp': update,
             'status': self.parse_order_status(rawStatus),
             'symbol': market['symbol'],
             'type': type,
             'timeInForce': None,
             'postOnly': None,
             'reduceOnly': None,
             'side': side,
             'price': self.safe_string(order, 'price'),
             'stopPrice': self.safe_string(order, 'stop_price'),
             'triggerPrice': self.safe_string(order, 'stop_price'),
             'takeProfitPrice': self.safe_number(order, 'take_profit_price'),
             'stopLossPrice': self.safe_number(order, 'stop_loss_price'),
-            'cost': self.safe_string(order, 'deal_money'),
-            'average': self.safe_string(order, 'avg_price'),
+            'cost': self.safe_string_2(order, 'deal_money', 'filled_value'),
+            'average': self.safe_string_2(order, 'avg_price', 'avg_entry_price'),
             'amount': self.safe_string(order, 'amount'),
-            'filled': self.safe_string(order, 'deal_amount'),
-            'remaining': self.safe_string(order, 'left'),
+            'filled': self.safe_string_2(order, 'deal_amount', 'filled_amount'),
+            'remaining': self.safe_string_2(order, 'left', 'unfilled_amount'),
             'trades': None,
             'fee': {
                 'currency': feeCurrency,
-                'cost': self.safe_string(order, 'deal_fee'),
+                'cost': self.safe_string_n(order, ['deal_fee', 'quote_fee', 'fee']),
             },
             'info': order,
         }, market)
 
-    async def create_market_buy_order_with_cost(self, symbol: str, cost: float, params={}):
+    def create_market_buy_order_with_cost(self, symbol: str, cost: float, params={}):
         """
         create a market buy order by providing the symbol and cost
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade003_market_order
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-order
         :param str symbol: unified symbol of the market to create an order in
         :param float cost: how much you want to trade in units of the quote currency
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if not market['spot']:
             raise NotSupported(self.id + ' createMarketBuyOrderWithCost() supports spot orders only')
         params['createMarketBuyOrderRequiresPrice'] = False
-        return await self.create_order(symbol, 'market', 'buy', cost, None, params)
+        return self.create_order(symbol, 'market', 'buy', cost, None, params)
 
     def create_order_request(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
         market = self.market(symbol)
         swap = market['swap']
         clientOrderId = self.safe_string_2(params, 'client_id', 'clientOrderId')
-        stopPrice = self.safe_value_2(params, 'stopPrice', 'triggerPrice')
-        stopLossPrice = self.safe_value(params, 'stopLossPrice')
-        takeProfitPrice = self.safe_value(params, 'takeProfitPrice')
+        stopPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
+        stopLossPrice = self.safe_string(params, 'stopLossPrice')
+        takeProfitPrice = self.safe_string(params, 'takeProfitPrice')
         option = self.safe_string(params, 'option')
         isMarketOrder = type == 'market'
-        postOnly = self.is_post_only(isMarketOrder, option == 'MAKER_ONLY', params)
-        positionId = self.safe_integer_2(params, 'position_id', 'positionId')  # Required for closing swap positions
-        timeInForceRaw = self.safe_string(params, 'timeInForce')  # Spot: IOC, FOK, PO, GTC, ... NORMAL(default), MAKER_ONLY
-        reduceOnly = self.safe_value(params, 'reduceOnly')
+        postOnly = self.is_post_only(isMarketOrder, option == 'maker_only', params)
+        timeInForceRaw = self.safe_string_upper(params, 'timeInForce')
+        reduceOnly = self.safe_bool(params, 'reduceOnly')
         if reduceOnly:
             if not market['swap']:
                 raise InvalidOrder(self.id + ' createOrder() does not support reduceOnly for ' + market['type'] + ' orders, reduceOnly orders are supported for swap markets only')
-            if positionId is None:
-                raise ArgumentsRequired(self.id + ' createOrder() requires a position_id/positionId parameter for reduceOnly orders')
         request = {
             'market': market['id'],
         }
         if clientOrderId is None:
             defaultId = 'x-167673045'
             brokerId = self.safe_string(self.options, 'brokerId', defaultId)
             request['client_id'] = brokerId + '-' + self.uuid16()
         else:
             request['client_id'] = clientOrderId
+        if (stopLossPrice is None) and (takeProfitPrice is None):
+            if not reduceOnly:
+                request['side'] = side
+            requestType = type
+            if postOnly:
+                requestType = 'maker_only'
+            elif timeInForceRaw is not None:
+                if timeInForceRaw == 'IOC':
+                    requestType = 'ioc'
+                elif timeInForceRaw == 'FOK':
+                    requestType = 'fok'
+            if not isMarketOrder:
+                request['price'] = self.price_to_precision(symbol, price)
+            request['type'] = requestType
         if swap:
+            request['market_type'] = 'FUTURES'
             if stopLossPrice or takeProfitPrice:
-                request['stop_type'] = self.safe_integer(params, 'stop_type', 1)  # 1: triggered by the latest transaction, 2: mark price, 3: index price
-                if positionId is None:
-                    raise ArgumentsRequired(self.id + ' createOrder() requires a position_id parameter for stop loss and take profit orders')
-                request['position_id'] = positionId
                 if stopLossPrice:
                     request['stop_loss_price'] = self.price_to_precision(symbol, stopLossPrice)
+                    request['stop_loss_type'] = self.safe_string(params, 'stop_type', 'latest_price')
                 elif takeProfitPrice:
                     request['take_profit_price'] = self.price_to_precision(symbol, takeProfitPrice)
+                    request['take_profit_type'] = self.safe_string(params, 'stop_type', 'latest_price')
             else:
-                requestSide = 2 if (side == 'buy') else 1
+                request['amount'] = self.amount_to_precision(symbol, amount)
                 if stopPrice is not None:
-                    request['stop_price'] = self.price_to_precision(symbol, stopPrice)
-                    request['stop_type'] = self.safe_integer(params, 'stop_type', 1)  # 1: triggered by the latest transaction, 2: mark price, 3: index price
-                    request['amount'] = self.amount_to_precision(symbol, amount)
-                    request['side'] = requestSide
-                    if type == 'limit':
-                        request['price'] = self.price_to_precision(symbol, price)
-                    request['amount'] = self.amount_to_precision(symbol, amount)
-                timeInForce = None
-                if (type != 'market') or (stopPrice is not None):
-                    if postOnly:
-                        request['option'] = 1
-                    elif timeInForceRaw is not None:
-                        if timeInForceRaw == 'IOC':
-                            timeInForce = 2
-                        elif timeInForceRaw == 'FOK':
-                            timeInForce = 3
-                        else:
-                            timeInForce = 1
-                        request['effect_type'] = timeInForce  # exchange takes 'IOC' and 'FOK'
-                if type == 'limit' and stopPrice is None:
-                    if reduceOnly:
-                        request['position_id'] = positionId
-                    else:
-                        request['side'] = requestSide
-                    request['price'] = self.price_to_precision(symbol, price)
-                    request['amount'] = self.amount_to_precision(symbol, amount)
-                elif type == 'market' and stopPrice is None:
-                    if reduceOnly:
-                        request['position_id'] = positionId
-                    else:
-                        request['side'] = requestSide
-                        request['amount'] = self.amount_to_precision(symbol, amount)
+                    request['trigger_price'] = self.price_to_precision(symbol, stopPrice)
+                    request['trigger_price_type'] = self.safe_string(params, 'stop_type', 'latest_price')
         else:
-            request['type'] = side
+            marginMode = None
+            marginMode, params = self.handle_margin_mode_and_params('createOrder', params)
+            if marginMode is not None:
+                request['market_type'] = 'MARGIN'
+            else:
+                request['market_type'] = 'SPOT'
             if (type == 'market') and (side == 'buy'):
                 createMarketBuyOrderRequiresPrice = True
                 createMarketBuyOrderRequiresPrice, params = self.handle_option_and_params(params, 'createOrder', 'createMarketBuyOrderRequiresPrice', True)
                 cost = self.safe_number(params, 'cost')
                 params = self.omit(params, 'cost')
                 if createMarketBuyOrderRequiresPrice:
                     if (price is None) and (cost is None):
@@ -2096,203 +2182,272 @@
                         quoteAmount = self.parse_to_numeric(Precise.string_mul(amountString, priceString))
                         costRequest = cost if (cost is not None) else quoteAmount
                         request['amount'] = self.cost_to_precision(symbol, costRequest)
                 else:
                     request['amount'] = self.cost_to_precision(symbol, amount)
             else:
                 request['amount'] = self.amount_to_precision(symbol, amount)
-            if (type == 'limit') or (type == 'ioc'):
-                request['price'] = self.price_to_precision(symbol, price)
             if stopPrice is not None:
-                request['stop_price'] = self.price_to_precision(symbol, stopPrice)
-            if (type != 'market') or (stopPrice is not None):
-                # following options cannot be applied to vanilla market orders(but can be applied to stop-market orders)
-                if (timeInForceRaw is not None) or postOnly:
-                    if (postOnly or (timeInForceRaw != 'IOC')) and ((type == 'limit') and (stopPrice is not None)):
-                        raise InvalidOrder(self.id + ' createOrder() only supports the IOC option for stop-limit orders')
-                    if postOnly:
-                        request['option'] = 'MAKER_ONLY'
-                    else:
-                        if timeInForceRaw is not None:
-                            request['option'] = timeInForceRaw  # exchange takes 'IOC' and 'FOK'
-        accountId = self.safe_integer(params, 'account_id')
-        marginMode = None
-        marginMode, params = self.handle_margin_mode_and_params('createOrder', params)
-        if marginMode is not None:
-            if accountId is None:
-                raise BadRequest(self.id + ' createOrder() requires an account_id parameter for margin orders')
-            request['account_id'] = accountId
-        params = self.omit(params, ['reduceOnly', 'positionId', 'timeInForce', 'postOnly', 'stopPrice', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice'])
+                request['trigger_price'] = self.price_to_precision(symbol, stopPrice)
+        params = self.omit(params, ['reduceOnly', 'timeInForce', 'postOnly', 'stopPrice', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice'])
         return self.extend(request, params)
 
-    async def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
+    def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
         """
         create a trade order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade001_limit_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade003_market_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade004_IOC_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade005_stop_limit_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade006_stop_market_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http017_put_limit
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http018_put_market
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http019_put_limit_stop
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http020_put_market_stop
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http031_market_close
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http030_limit_close
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-order
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-stop-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-stop-order
+        :see: https://docs.coinex.com/api/v2/futures/position/http/close-position
+        :see: https://docs.coinex.com/api/v2/futures/position/http/set-position-stop-loss
+        :see: https://docs.coinex.com/api/v2/futures/position/http/set-position-take-profit
         :param str symbol: unified symbol of the market to create an order in
         :param str type: 'market' or 'limit'
         :param str side: 'buy' or 'sell'
         :param float amount: how much you want to trade in units of the base currency
         :param float [price]: the price at which the order is to be fullfilled, in units of the quote currency, ignored in market orders
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param float [params.triggerPrice]: price to trigger stop orders
         :param float [params.stopLossPrice]: price to trigger stop loss orders
         :param float [params.takeProfitPrice]: price to trigger take profit orders
         :param str [params.timeInForce]: 'GTC', 'IOC', 'FOK', 'PO'
         :param boolean [params.postOnly]: set to True if you wish to make a post only order
         :param boolean [params.reduceOnly]: *contract only* indicates if self order is to reduce the size of a position
-        :param int [params.position_id]: *required for reduce only orders* the position id to reduce
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
-        reduceOnly = self.safe_value(params, 'reduceOnly')
-        triggerPrice = self.safe_number_2(params, 'stopPrice', 'triggerPrice')
-        stopLossTriggerPrice = self.safe_number(params, 'stopLossPrice')
-        takeProfitTriggerPrice = self.safe_number(params, 'takeProfitPrice')
+        reduceOnly = self.safe_bool(params, 'reduceOnly')
+        triggerPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
+        stopLossTriggerPrice = self.safe_string(params, 'stopLossPrice')
+        takeProfitTriggerPrice = self.safe_string(params, 'takeProfitPrice')
         isTriggerOrder = triggerPrice is not None
         isStopLossTriggerOrder = stopLossTriggerPrice is not None
         isTakeProfitTriggerOrder = takeProfitTriggerPrice is not None
         isStopLossOrTakeProfitTrigger = isStopLossTriggerOrder or isTakeProfitTriggerOrder
         request = self.create_order_request(symbol, type, side, amount, price, params)
         response = None
         if market['spot']:
             if isTriggerOrder:
-                if type == 'limit':
-                    response = await self.v1PrivatePostOrderStopLimit(request)
-                else:
-                    response = await self.v1PrivatePostOrderStopMarket(request)
+                response = self.v2PrivatePostSpotStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": {
+                #             "stop_id": 117180138153
+                #         },
+                #         "message": "OK"
+                #     }
+                #
             else:
-                if type == 'limit':
-                    response = await self.v1PrivatePostOrderLimit(request)
-                else:
-                    response = await self.v1PrivatePostOrderMarket(request)
+                response = self.v2PrivatePostSpotOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": {
+                #             "amount": "0.0001",
+                #             "base_fee": "0",
+                #             "ccy": "BTC",
+                #             "client_id": "x-167673045-a0a3c6461459a801",
+                #             "created_at": 1714114386250,
+                #             "discount_fee": "0",
+                #             "filled_amount": "0",
+                #             "filled_value": "0",
+                #             "last_fill_amount": "0",
+                #             "last_fill_price": "0",
+                #             "maker_fee_rate": "0.002",
+                #             "market": "BTCUSDT",
+                #             "market_type": "SPOT",
+                #             "order_id": 117178743547,
+                #             "price": "61000",
+                #             "quote_fee": "0",
+                #             "side": "buy",
+                #             "taker_fee_rate": "0.002",
+                #             "type": "limit",
+                #             "unfilled_amount": "0.0001",
+                #             "updated_at": 1714114386250
+                #         },
+                #         "message": "OK"
+                #     }
+                #
         else:
             if isTriggerOrder:
-                if type == 'limit':
-                    response = await self.v1PerpetualPrivatePostOrderPutStopLimit(request)
-                else:
-                    response = await self.v1PerpetualPrivatePostOrderPutStopMarket(request)
+                response = self.v2PrivatePostFuturesStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": {
+                #             "stop_id": 136915460994
+                #         },
+                #         "message": "OK"
+                #     }
+                #
             elif isStopLossOrTakeProfitTrigger:
                 if isStopLossTriggerOrder:
-                    response = await self.v1PerpetualPrivatePostPositionStopLoss(request)
+                    response = self.v2PrivatePostFuturesSetPositionStopLoss(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "adl_level": 1,
+                    #             "ath_margin_size": "2.14586666",
+                    #             "ath_position_amount": "0.0001",
+                    #             "avg_entry_price": "64376",
+                    #             "bkr_price": "0",
+                    #             "close_avbl": "0.0001",
+                    #             "cml_position_value": "6.4376",
+                    #             "created_at": 1714119054558,
+                    #             "leverage": "3",
+                    #             "liq_price": "0",
+                    #             "maintenance_margin_rate": "0.005",
+                    #             "maintenance_margin_value": "0.03218632",
+                    #             "margin_avbl": "2.14586666",
+                    #             "margin_mode": "cross",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "max_position_value": "6.4376",
+                    #             "open_interest": "0.0001",
+                    #             "position_id": 303884204,
+                    #             "position_margin_rate": "3.10624785634397912265",
+                    #             "realized_pnl": "-0.0032188",
+                    #             "settle_price": "64376",
+                    #             "settle_value": "6.4376",
+                    #             "side": "long",
+                    #             "stop_loss_price": "62000",
+                    #             "stop_loss_type": "latest_price",
+                    #             "take_profit_price": "0",
+                    #             "take_profit_type": "",
+                    #             "unrealized_pnl": "0",
+                    #             "updated_at": 1714119054559
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
                 elif isTakeProfitTriggerOrder:
-                    response = await self.v1PerpetualPrivatePostPositionTakeProfit(request)
+                    response = self.v2PrivatePostFuturesSetPositionTakeProfit(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "adl_level": 1,
+                    #             "ath_margin_size": "2.14586666",
+                    #             "ath_position_amount": "0.0001",
+                    #             "avg_entry_price": "64376",
+                    #             "bkr_price": "0",
+                    #             "close_avbl": "0.0001",
+                    #             "cml_position_value": "6.4376",
+                    #             "created_at": 1714119054558,
+                    #             "leverage": "3",
+                    #             "liq_price": "0",
+                    #             "maintenance_margin_rate": "0.005",
+                    #             "maintenance_margin_value": "0.03218632",
+                    #             "margin_avbl": "2.14586666",
+                    #             "margin_mode": "cross",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "max_position_value": "6.4376",
+                    #             "open_interest": "0.0001",
+                    #             "position_id": 303884204,
+                    #             "position_margin_rate": "3.10624785634397912265",
+                    #             "realized_pnl": "-0.0032188",
+                    #             "settle_price": "64376",
+                    #             "settle_value": "6.4376",
+                    #             "side": "long",
+                    #             "stop_loss_price": "62000",
+                    #             "stop_loss_type": "latest_price",
+                    #             "take_profit_price": "70000",
+                    #             "take_profit_type": "latest_price",
+                    #             "unrealized_pnl": "0",
+                    #             "updated_at": 1714119054559
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
             else:
                 if reduceOnly:
-                    if type == 'limit':
-                        response = await self.v1PerpetualPrivatePostOrderCloseLimit(request)
-                    else:
-                        response = await self.v1PerpetualPrivatePostOrderCloseMarket(request)
+                    response = self.v2PrivatePostFuturesClosePosition(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "amount": "0.0001",
+                    #             "client_id": "x-167673045-4f264600c432ac06",
+                    #             "created_at": 1714119323764,
+                    #             "fee": "0.003221",
+                    #             "fee_ccy": "USDT",
+                    #             "filled_amount": "0.0001",
+                    #             "filled_value": "6.442017",
+                    #             "last_filled_amount": "0.0001",
+                    #             "last_filled_price": "64420.17",
+                    #             "maker_fee_rate": "0",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "order_id": 136915813578,
+                    #             "price": "0",
+                    #             "realized_pnl": "0.004417",
+                    #             "side": "sell",
+                    #             "taker_fee_rate": "0.0005",
+                    #             "type": "market",
+                    #             "unfilled_amount": "0",
+                    #             "updated_at": 1714119323764
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
                 else:
-                    if type == 'limit':
-                        response = await self.v1PerpetualPrivatePostOrderPutLimit(request)
-                    else:
-                        response = await self.v1PerpetualPrivatePostOrderPutMarket(request)
-        #
-        # Spot and Margin
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "amount": "0.0005",
-        #             "asset_fee": "0",
-        #             "avg_price": "0.00",
-        #             "client_id": "",
-        #             "create_time": 1650951627,
-        #             "deal_amount": "0",
-        #             "deal_fee": "0",
-        #             "deal_money": "0",
-        #             "fee_asset": null,
-        #             "fee_discount": "1",
-        #             "finished_time": null,
-        #             "id": 74510932594,
-        #             "left": "0.0005",
-        #             "maker_fee_rate": "0.002",
-        #             "market": "BTCUSDT",
-        #             "money_fee": "0",
-        #             "order_type": "limit",
-        #             "price": "30000",
-        #             "status": "not_deal",
-        #             "stock_fee": "0",
-        #             "taker_fee_rate": "0.002",
-        #             "type": "buy"
-        #         },
-        #         "message": "Success"
-        #     }
-        #
-        # Swap
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "amount": "0.0005",
-        #             "client_id": "",
-        #             "create_time": 1651004578.618224,
-        #             "deal_asset_fee": "0.00000000000000000000",
-        #             "deal_fee": "0.00000000000000000000",
-        #             "deal_profit": "0.00000000000000000000",
-        #             "deal_stock": "0.00000000000000000000",
-        #             "effect_type": 1,
-        #             "fee_asset": "",
-        #             "fee_discount": "0.00000000000000000000",
-        #             "last_deal_amount": "0.00000000000000000000",
-        #             "last_deal_id": 0,
-        #             "last_deal_price": "0.00000000000000000000",
-        #             "last_deal_role": 0,
-        #             "last_deal_time": 0,
-        #             "last_deal_type": 0,
-        #             "left": "0.0005",
-        #             "leverage": "3",
-        #             "maker_fee": "0.00030",
-        #             "market": "BTCUSDT",
-        #             "order_id": 18221659097,
-        #             "position_id": 0,
-        #             "position_type": 1,
-        #             "price": "30000.00",
-        #             "side": 2,
-        #             "source": "api.v1",
-        #             "stop_id": 0,
-        #             "taker_fee": "0.00050",
-        #             "target": 0,
-        #             "type": 1,
-        #             "update_time": 1651004578.618224,
-        #             "user_id": 3620173
-        #         },
-        #         "message": "OK"
-        #     }
-        #
-        # Stop Order
-        #
-        #     {"code":0,"data":{"status":"success"},"message":"OK"}
-        #
+                    response = self.v2PrivatePostFuturesOrder(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "amount": "0.0001",
+                    #             "client_id": "x-167673045-1471b81d747080a0",
+                    #             "created_at": 1714116769986,
+                    #             "fee": "0",
+                    #             "fee_ccy": "USDT",
+                    #             "filled_amount": "0",
+                    #             "filled_value": "0",
+                    #             "last_filled_amount": "0",
+                    #             "last_filled_price": "0",
+                    #             "maker_fee_rate": "0.0003",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "order_id": 136913377780,
+                    #             "price": "61000.42",
+                    #             "realized_pnl": "0",
+                    #             "side": "buy",
+                    #             "taker_fee_rate": "0.0005",
+                    #             "type": "limit",
+                    #             "unfilled_amount": "0.0001",
+                    #             "updated_at": 1714116769986
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
         data = self.safe_dict(response, 'data', {})
         return self.parse_order(data, market)
 
-    async def create_orders(self, orders: List[OrderRequest], params={}) -> List[Order]:
+    def create_orders(self, orders: List[OrderRequest], params={}) -> List[Order]:
         """
         create a list of trade orders(all orders should be of the same symbol)
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade002_batch_limit_orders
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-multi-order
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-multi-stop-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-multi-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-multi-stop-order
         :param Array orders: list of orders to create, each object should contain the parameters required by createOrder, namely symbol, type, side, amount, price and params
         :param dict [params]: extra parameters specific to the api endpoint
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         ordersRequests = []
         symbol = None
+        reduceOnly = False
+        isTriggerOrder = False
+        isStopLossOrTakeProfitTrigger = False
         for i in range(0, len(orders)):
             rawOrder = orders[i]
             marketId = self.safe_string(rawOrder, 'symbol')
             if symbol is None:
                 symbol = marketId
             else:
                 if symbol != marketId:
@@ -2300,103 +2455,192 @@
             type = self.safe_string(rawOrder, 'type')
             side = self.safe_string(rawOrder, 'side')
             amount = self.safe_value(rawOrder, 'amount')
             price = self.safe_value(rawOrder, 'price')
             orderParams = self.safe_value(rawOrder, 'params', {})
             if type != 'limit':
                 raise NotSupported(self.id + ' createOrders() does not support ' + type + ' orders, only limit orders are accepted')
+            reduceOnly = self.safe_value(orderParams, 'reduceOnly')
+            triggerPrice = self.safe_number_2(orderParams, 'stopPrice', 'triggerPrice')
+            stopLossTriggerPrice = self.safe_number(orderParams, 'stopLossPrice')
+            takeProfitTriggerPrice = self.safe_number(orderParams, 'takeProfitPrice')
+            isTriggerOrder = triggerPrice is not None
+            isStopLossTriggerOrder = stopLossTriggerPrice is not None
+            isTakeProfitTriggerOrder = takeProfitTriggerPrice is not None
+            isStopLossOrTakeProfitTrigger = isStopLossTriggerOrder or isTakeProfitTriggerOrder
             orderRequest = self.create_order_request(marketId, type, side, amount, price, orderParams)
             ordersRequests.append(orderRequest)
         market = self.market(symbol)
-        if not market['spot']:
-            raise NotSupported(self.id + ' createOrders() does not support ' + market['type'] + ' orders, only spot orders are accepted')
         request = {
             'market': market['id'],
-            'batch_orders': self.json(ordersRequests),
+            'orders': ordersRequests,
         }
-        response = await self.v1PrivatePostOrderLimitBatch(request)
-        #
-        #     {
-        #         "code": 0,
-        #         "data": [
-        #             {
-        #                 "code": 0,
-        #                 "data": {
-        #                     "amount": "0.0005",
-        #                     "asset_fee": "0",
-        #                     "avg_price": "0.00",
-        #                     "client_id": "x-167673045-d34bfb41242d8fd1",
-        #                     "create_time": 1701229157,
-        #                     "deal_amount": "0",
-        #                     "deal_fee": "0",
-        #                     "deal_money": "0",
-        #                     "fee_asset": null,
-        #                     "fee_discount": "1",
-        #                     "finished_time": null,
-        #                     "id": 107745856676,
-        #                     "left": "0.0005",
-        #                     "maker_fee_rate": "0.002",
-        #                     "market": "BTCUSDT",
-        #                     "money_fee": "0",
-        #                     "order_type": "limit",
-        #                     "price": "23000",
-        #                     "source_id": "",
-        #                     "status": "not_deal",
-        #                     "stock_fee": "0",
-        #                     "taker_fee_rate": "0.002",
-        #                     "type": "buy"
-        #                 },
-        #                 "message": "OK"
-        #             },
-        #         ],
-        #         "message": "Success"
-        #     }
-        #
-        data = self.safe_value(response, 'data', [])
+        response = None
+        if market['spot']:
+            if isTriggerOrder:
+                response = self.v2PrivatePostSpotBatchStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": [
+                #             {
+                #                 "code": 0,
+                #                 "data": {
+                #                     "stop_id": 117186257510
+                #                 },
+                #                 "message": "OK"
+                #             },
+                #         ],
+                #         "message": "OK"
+                #     }
+                #
+            else:
+                response = self.v2PrivatePostSpotBatchOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": [
+                #             {
+                #                 "amount": "0.0001",
+                #                 "base_fee": "0",
+                #                 "ccy": "BTC",
+                #                 "client_id": "x-167673045-f3651372049dab0d",
+                #                 "created_at": 1714121403450,
+                #                 "discount_fee": "0",
+                #                 "filled_amount": "0",
+                #                 "filled_value": "0",
+                #                 "last_fill_amount": "0",
+                #                 "last_fill_price": "0",
+                #                 "maker_fee_rate": "0.002",
+                #                 "market": "BTCUSDT",
+                #                 "market_type": "SPOT",
+                #                 "order_id": 117185362233,
+                #                 "price": "61000",
+                #                 "quote_fee": "0",
+                #                 "side": "buy",
+                #                 "taker_fee_rate": "0.002",
+                #                 "type": "limit",
+                #                 "unfilled_amount": "0.0001",
+                #                 "updated_at": 1714121403450
+                #             },
+                #             {
+                #                 "code": 3109,
+                #                 "data": null,
+                #                 "message": "balance not enough"
+                #             }
+                #         ],
+                #         "message": "OK"
+                #     }
+                #
+        else:
+            if isTriggerOrder:
+                response = self.v2PrivatePostFuturesBatchStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": [
+                #             {
+                #                 "code": 0,
+                #                 "data": {
+                #                     "stop_id": 136919625994
+                #                 },
+                #                 "message": "OK"
+                #             },
+                #         ],
+                #         "message": "OK"
+                #     }
+                #
+            elif isStopLossOrTakeProfitTrigger:
+                raise NotSupported(self.id + ' createOrders() does not support stopLossPrice or takeProfitPrice orders')
+            else:
+                if reduceOnly:
+                    raise NotSupported(self.id + ' createOrders() does not support reduceOnly orders')
+                else:
+                    response = self.v2PrivatePostFuturesBatchOrder(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": [
+                    #             {
+                    #                 "code": 0,
+                    #                 "data": {
+                    #                     "amount": "0.0001",
+                    #                     "client_id": "x-167673045-2cb7436f3462a654",
+                    #                     "created_at": 1714122832493,
+                    #                     "fee": "0",
+                    #                     "fee_ccy": "USDT",
+                    #                     "filled_amount": "0",
+                    #                     "filled_value": "0",
+                    #                     "last_filled_amount": "0",
+                    #                     "last_filled_price": "0",
+                    #                     "maker_fee_rate": "0.0003",
+                    #                     "market": "BTCUSDT",
+                    #                     "market_type": "FUTURES",
+                    #                     "order_id": 136918835063,
+                    #                     "price": "61000",
+                    #                     "realized_pnl": "0",
+                    #                     "side": "buy",
+                    #                     "taker_fee_rate": "0.0005",
+                    #                     "type": "limit",
+                    #                     "unfilled_amount": "0.0001",
+                    #                     "updated_at": 1714122832493
+                    #                 },
+                    #                 "message": "OK"
+                    #             },
+                    #         ],
+                    #         "message": "OK"
+                    #     }
+                    #
+        data = self.safe_list(response, 'data', [])
         results = []
         for i in range(0, len(data)):
             entry = data[i]
             status = None
             code = self.safe_integer(entry, 'code')
             if code is not None:
                 if code != 0:
                     status = 'rejected'
                 else:
                     status = 'open'
-            item = self.safe_value(entry, 'data', {})
-            item['status'] = status
-            order = self.parse_order(item, market)
+            innerData = self.safe_dict(entry, 'data', {})
+            order = None
+            if market['spot'] and not isTriggerOrder:
+                entry['status'] = status
+                order = self.parse_order(entry, market)
+            else:
+                innerData['status'] = status
+                order = self.parse_order(innerData, market)
             results.append(order)
         return results
 
-    async def cancel_orders(self, ids, symbol: Str = None, params={}):
+    def cancel_orders(self, ids, symbol: Str = None, params={}):
         """
         cancel multiple orders
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade016_batch_cancel_order
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http021-0_cancel_order_batch
         :param str[] ids: order ids
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' cancelOrders() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
         idsString = ','.join(ids)
         response = None
         if market['spot']:
             request['batch_ids'] = idsString
-            response = await self.v1PrivateDeleteOrderPendingBatch(self.extend(request, params))
+            response = self.v1PrivateDeleteOrderPendingBatch(self.extend(request, params))
         else:
             request['order_ids'] = idsString
-            response = await self.v1PerpetualPrivatePostOrderCancelBatch(self.extend(request, params))
+            response = self.v1PerpetualPrivatePostOrderCancelBatch(self.extend(request, params))
         #
         # spot
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -2490,42 +2734,42 @@
             entry = data[i]
             dataRequest = 'data' if market['spot'] else 'order'
             item = self.safe_value(entry, dataRequest, {})
             order = self.parse_order(item, market)
             results.append(order)
         return results
 
-    async def edit_order(self, id: str, symbol: str, type: OrderType, side: OrderSide, amount: Num = None, price: Num = None, params={}):
+    def edit_order(self, id: str, symbol: str, type: OrderType, side: OrderSide, amount: Num = None, price: Num = None, params={}):
         """
         edit a trade order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade022_modify_order
         :param str id: order id
         :param str symbol: unified symbol of the market to create an order in
         :param str type: 'market' or 'limit'
         :param str side: 'buy' or 'sell'
         :param float amount: how much of the currency you want to trade in units of the base currency
         :param float [price]: the price at which the order is to be fullfilled, in units of the quote currency, ignored in market orders
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' editOrder() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if not market['spot']:
             raise NotSupported(self.id + ' editOrder() does not support ' + market['type'] + ' orders, only spot orders are accepted')
         request = {
             'market': market['id'],
             'id': int(id),
         }
         if amount is not None:
             request['amount'] = self.amount_to_precision(symbol, amount)
         if price is not None:
             request['price'] = self.price_to_precision(symbol, price)
-        response = await self.v1PrivatePostOrderModify(self.extend(request, params))
+        response = self.v1PrivatePostOrderModify(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "id": 35436205,
         #             "create_time": 1636080705,
         #             "finished_time": null,
@@ -2552,15 +2796,15 @@
         #     },
         #         "message": "Success"
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         return self.parse_order(data, market)
 
-    async def cancel_order(self, id: str, symbol: Str = None, params={}):
+    def cancel_order(self, id: str, symbol: Str = None, params={}):
         """
         cancels an open order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade018_cancle_stop_pending_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade015_cancel_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade024_cancel_order_by_client_id
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade025_cancel_stop_order_by_client_id
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http023_cancel_stop_order
@@ -2572,15 +2816,15 @@
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.clientOrderId]: client order id, defaults to id if not passed
         :param boolean [params.stop]: if stop order = True, default = False
         :returns dict: An `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' cancelOrder() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         stop = self.safe_value(params, 'stop')
         swap = market['swap']
         request = {
             'market': market['id'],
         }
         accountId = self.safe_integer(params, 'account_id')
@@ -2593,35 +2837,35 @@
             request['account_id'] = accountId
         query = self.omit(params, ['stop', 'account_id', 'clientOrderId'])
         response = None
         if clientOrderId is not None:
             request['client_id'] = clientOrderId
             if stop:
                 if swap:
-                    response = await self.v1PerpetualPrivatePostOrderCancelStopByClientId(self.extend(request, query))
+                    response = self.v1PerpetualPrivatePostOrderCancelStopByClientId(self.extend(request, query))
                 else:
-                    response = await self.v1PrivateDeleteOrderStopPendingByClientId(self.extend(request, query))
+                    response = self.v1PrivateDeleteOrderStopPendingByClientId(self.extend(request, query))
             else:
                 if swap:
-                    response = await self.v1PerpetualPrivatePostOrderCancelByClientId(self.extend(request, query))
+                    response = self.v1PerpetualPrivatePostOrderCancelByClientId(self.extend(request, query))
                 else:
-                    response = await self.v1PrivateDeleteOrderPendingByClientId(self.extend(request, query))
+                    response = self.v1PrivateDeleteOrderPendingByClientId(self.extend(request, query))
         else:
             idRequest = 'order_id' if swap else 'id'
             request[idRequest] = id
             if stop:
                 if swap:
-                    response = await self.v1PerpetualPrivatePostOrderCancelStop(self.extend(request, query))
+                    response = self.v1PerpetualPrivatePostOrderCancelStop(self.extend(request, query))
                 else:
-                    response = await self.v1PrivateDeleteOrderStopPendingId(self.extend(request, query))
+                    response = self.v1PrivateDeleteOrderStopPendingId(self.extend(request, query))
             else:
                 if swap:
-                    response = await self.v1PerpetualPrivatePostOrderCancel(self.extend(request, query))
+                    response = self.v1PerpetualPrivatePostOrderCancel(self.extend(request, query))
                 else:
-                    response = await self.v1PrivateDeleteOrderPending(self.extend(request, query))
+                    response = self.v1PrivateDeleteOrderPending(self.extend(request, query))
         #
         # Spot and Margin
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "amount": "0.0005",
@@ -2723,94 +2967,94 @@
         # Spot and Margin Stop
         #
         #     {"code":0,"data":{},"message":"Success"}
         #
         data = self.safe_dict(response, 'data')
         return self.parse_order(data, market)
 
-    async def cancel_all_orders(self, symbol: Str = None, params={}):
+    def cancel_all_orders(self, symbol: Str = None, params={}):
         """
         cancel all open orders in a market
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade018_cancle_stop_pending_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade015_cancel_order
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http024_cancel_stop_all
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http022_cancel_all
         :param str symbol: unified market symbol of the market to cancel orders in
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' cancelAllOrders() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         accountId = self.safe_integer(params, 'account_id', 0)
         request = {
             'market': marketId,
             # 'account_id': accountId,  # SPOT, main account ID: 0, margin account ID: See < Inquire Margin Account Market Info >, future account ID: See < Inquire Future Account Market Info >
             # 'side': 0,  # SWAP, 0: All, 1: Sell, 2: Buy
         }
         swap = market['swap']
         stop = self.safe_value(params, 'stop')
         params = self.omit(params, ['stop', 'account_id'])
         response = None
         if swap:
             if stop:
-                response = await self.v1PerpetualPrivatePostOrderCancelStopAll(self.extend(request, params))
+                response = self.v1PerpetualPrivatePostOrderCancelStopAll(self.extend(request, params))
             else:
-                response = await self.v1PerpetualPrivatePostOrderCancelAll(self.extend(request, params))
+                response = self.v1PerpetualPrivatePostOrderCancelAll(self.extend(request, params))
         else:
             request['account_id'] = accountId
             if stop:
-                response = await self.v1PrivateDeleteOrderStopPending(self.extend(request, params))
+                response = self.v1PrivateDeleteOrderStopPending(self.extend(request, params))
             else:
-                response = await self.v1PrivateDeleteOrderPending(self.extend(request, params))
+                response = self.v1PrivateDeleteOrderPending(self.extend(request, params))
         #
         # Spot and Margin
         #
         #     {"code": 0, "data": null, "message": "Success"}
         #
         # Swap
         #
         #     {"code": 0, "data": {"status":"success"}, "message": "OK"}
         #
         return response
 
-    async def fetch_order(self, id: str, symbol: Str = None, params={}):
+    def fetch_order(self, id: str, symbol: Str = None, params={}):
         """
         fetches information on an order made by the user
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http028_stop_status
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http026_order_status
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade007_order_status
         :param str symbol: unified symbol of the market the order was made in
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: An `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' fetchOrder() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         swap = market['swap']
         stop = self.safe_value(params, 'stop')
         params = self.omit(params, 'stop')
         request = {
             'market': market['id'],
             # 'id': id,  # SPOT
             # 'order_id': id,  # SWAP
         }
         idRequest = 'order_id' if swap else 'id'
         request[idRequest] = id
         response = None
         if swap:
             if stop:
-                response = await self.v1PerpetualPrivateGetOrderStopStatus(self.extend(request, params))
+                response = self.v1PerpetualPrivateGetOrderStopStatus(self.extend(request, params))
             else:
-                response = await self.v1PerpetualPrivateGetOrderStatus(self.extend(request, params))
+                response = self.v1PerpetualPrivateGetOrderStatus(self.extend(request, params))
         else:
-            response = await self.v1PrivateGetOrderStatus(self.extend(request, params))
+            response = self.v1PrivateGetOrderStatus(self.extend(request, params))
         #
         # Spot
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "amount": "0.1",
@@ -2904,16 +3148,16 @@
         #         },
         #         "message":"OK"
         #     }
         #
         data = self.safe_dict(response, 'data')
         return self.parse_order(data, market)
 
-    async def fetch_orders_by_status(self, status, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
-        await self.load_markets()
+    def fetch_orders_by_status(self, status, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+        self.load_markets()
         limit = 100 if (limit is None) else limit
         request = {
             'limit': limit,
             # 'page': 1,  # SPOT
             # 'offset': 0,  # SWAP
             # 'side': 0,  # SWAP, 0: All, 1: Sell, 2: Buy
         }
@@ -2939,32 +3183,32 @@
                 raise ArgumentsRequired(self.id + ' fetchOrdersByStatus() requires a symbol argument for swap markets')
             if side is not None:
                 request['side'] = side
             else:
                 request['side'] = 0
             request['offset'] = 0
             if stop:
-                response = await self.v1PerpetualPrivateGetOrderStopPending(self.extend(request, params))
+                response = self.v1PerpetualPrivateGetOrderStopPending(self.extend(request, params))
             else:
                 if status == 'finished':
-                    response = await self.v1PerpetualPrivateGetOrderFinished(self.extend(request, params))
+                    response = self.v1PerpetualPrivateGetOrderFinished(self.extend(request, params))
                 elif status == 'pending':
-                    response = await self.v1PerpetualPrivateGetOrderPending(self.extend(request, params))
+                    response = self.v1PerpetualPrivateGetOrderPending(self.extend(request, params))
         else:
             request['page'] = 1
             if status == 'finished':
                 if stop:
-                    response = await self.v1PrivateGetOrderStopFinished(self.extend(request, params))
+                    response = self.v1PrivateGetOrderStopFinished(self.extend(request, params))
                 else:
-                    response = await self.v1PrivateGetOrderFinished(self.extend(request, params))
+                    response = self.v1PrivateGetOrderFinished(self.extend(request, params))
             elif status == 'pending':
                 if stop:
-                    response = await self.v1PrivateGetOrderStopPending(self.extend(request, params))
+                    response = self.v1PrivateGetOrderStopPending(self.extend(request, params))
                 else:
-                    response = await self.v1PrivateGetOrderPending(self.extend(request, params))
+                    response = self.v1PrivateGetOrderPending(self.extend(request, params))
         #
         # Spot and Margin
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "count": 1,
@@ -3112,82 +3356,82 @@
         #     }
         #
         tradeRequest = 'records' if (marketType == 'swap') else 'data'
         data = self.safe_value(response, 'data')
         orders = self.safe_list(data, tradeRequest, [])
         return self.parse_orders(orders, market, since, limit)
 
-    async def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
+    def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
         """
         fetch all unfilled currently open orders
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http027_query_pending_stop
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http025_query_pending
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade013_stop_pending_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade011_pending_order
         :param str symbol: unified market symbol
         :param int [since]: the earliest time in ms to fetch open orders for
         :param int [limit]: the maximum number of  open orders structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Order[]: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        return await self.fetch_orders_by_status('pending', symbol, since, limit, params)
+        return self.fetch_orders_by_status('pending', symbol, since, limit, params)
 
-    async def fetch_closed_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
+    def fetch_closed_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
         """
         fetches information on multiple closed orders made by the user
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http029_query_finished
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade010_stop_finished_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade012_finished_order
         :param str symbol: unified market symbol of the market orders were made in
         :param int [since]: the earliest time in ms to fetch orders for
         :param int [limit]: the maximum number of order structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Order[]: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        return await self.fetch_orders_by_status('finished', symbol, since, limit, params)
+        return self.fetch_orders_by_status('finished', symbol, since, limit, params)
 
-    async def create_deposit_address(self, code: str, params={}):
+    def create_deposit_address(self, code: str, params={}):
         """
         create a currency deposit address
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account019_update_deposit_address
         :param str code: unified currency code of the currency for the deposit address
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `address structure <https://docs.ccxt.com/#/?id=address-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         currency = self.currency(code)
         request = {
             'coin_type': currency['id'],
         }
         if 'network' in params:
             network = self.safe_string(params, 'network')
             params = self.omit(params, 'network')
             request['smart_contract_name'] = network
-        response = await self.v1PrivatePutBalanceDepositAddressCoinType(self.extend(request, params))
+        response = self.v1PrivatePutBalanceDepositAddressCoinType(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "coin_address": "TV639dSpb9iGRtoFYkCp4AoaaDYKrK1pw5",
         #             "is_bitcoin_cash": False
         #         },
         #         "message": "Success"
         #     }
         data = self.safe_dict(response, 'data', {})
         return self.parse_deposit_address(data, currency)
 
-    async def fetch_deposit_address(self, code: str, params={}):
+    def fetch_deposit_address(self, code: str, params={}):
         """
         fetch the deposit address for a currency associated with self account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account020_query_deposit_address
         :param str code: unified currency code
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `address structure <https://docs.ccxt.com/#/?id=address-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         currency = self.currency(code)
         request = {
             'coin_type': currency['id'],
         }
         networks = self.safe_value(currency, 'networks', {})
         network = self.safe_string(params, 'network')
         params = self.omit(params, 'network')
@@ -3196,15 +3440,15 @@
         if networks is not None and numOfNetworks > 1:
             if network is None:
                 raise ArgumentsRequired(self.id + ' fetchDepositAddress() ' + code + ' requires a network parameter')
             if not (network in networks):
                 raise ExchangeError(self.id + ' fetchDepositAddress() ' + network + ' network not supported for ' + code)
         if network is not None:
             request['smart_contract_name'] = network
-        response = await self.v1PrivateGetBalanceDepositAddressCoinType(self.extend(request, params))
+        response = self.v1PrivateGetBalanceDepositAddressCoinType(self.extend(request, params))
         #
         #      {
         #          "code": 0,
         #          "data": {
         #            "coin_address": "1P1JqozxioQwaqPwgMAQdNDYNyaVSqgARq",
         #            # coin_address: "xxxxxxxxxxxxxx:yyyyyyyyy",  # with embedded tag/memo
         #            "is_bitcoin_cash": False
@@ -3256,26 +3500,26 @@
             'info': depositAddress,
             'currency': self.safe_currency_code(None, currency),
             'address': address,
             'tag': tag,
             'network': None,
         }
 
-    async def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+    def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch all trades made by the user
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http013_user_deals
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade014_user_deals
         :param str symbol: unified market symbol
         :param int [since]: the earliest time in ms to fetch trades for
         :param int [limit]: the maximum number of trades structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Trade[]: a list of `trade structures <https://docs.ccxt.com/#/?id=trade-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = None
         if limit is None:
             limit = 100
         request = {
             'limit': limit,  # SPOT and SWAP
             'offset': 0,  # SWAP, means query from a certain record
             # 'page': 1,  # SPOT
@@ -3300,18 +3544,18 @@
             request['account_id'] = accountId
             params = self.omit(params, 'account_id')
         response = None
         if swap:
             if since is not None:
                 request['start_time'] = since
             request['side'] = 0
-            response = await self.v1PerpetualPrivateGetMarketUserDeals(self.extend(request, params))
+            response = self.v1PerpetualPrivateGetMarketUserDeals(self.extend(request, params))
         else:
             request['page'] = 1
-            response = await self.v1PrivateGetOrderUserDeals(self.extend(request, params))
+            response = self.v1PrivateGetOrderUserDeals(self.extend(request, params))
         #
         # Spot and Margin
         #
         #      {
         #          "code": 0,
         #          "data": {
         #              "data": [
@@ -3381,26 +3625,26 @@
         #     }
         #
         tradeRequest = 'records' if swap else 'data'
         data = self.safe_value(response, 'data')
         trades = self.safe_list(data, tradeRequest, [])
         return self.parse_trades(trades, market, since, limit)
 
-    async def fetch_positions(self, symbols: Strings = None, params={}):
+    def fetch_positions(self, symbols: Strings = None, params={}):
         """
         fetch all open positions
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033_pending_position
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033-0_finished_position
         :param str[] [symbols]: list of unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.method]: the method to use 'perpetualPrivateGetPositionPending' or 'perpetualPrivateGetPositionFinished' default is 'perpetualPrivateGetPositionPending'
         :param int [params.side]: *history endpoint only* 0: All, 1: Sell, 2: Buy, default is 0
         :returns dict[]: a list of `position structure <https://docs.ccxt.com/#/?id=position-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         defaultMethod = None
         defaultMethod, params = self.handle_option_and_params(params, 'fetchPositions', 'method', 'v1PerpetualPrivateGetPositionPending')
         isHistory = (defaultMethod == 'v1PerpetualPrivateGetPositionFinished')
         symbols = self.market_symbols(symbols)
         request = {}
         market = None
         if symbols is not None:
@@ -3418,17 +3662,17 @@
             if isHistory:
                 raise ArgumentsRequired(self.id + ' fetchPositions() requires a symbol argument for closed positions')
         if isHistory:
             request['limit'] = 100
             request['side'] = self.safe_integer(params, 'side', 0)  # 0: All, 1: Sell, 2: Buy
         response = None
         if defaultMethod == 'v1PerpetualPrivateGetPositionPending':
-            response = await self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
+            response = self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
         else:
-            response = await self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
+            response = self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "adl_sort": 3396,
         #                 "adl_sort_val": "0.00007786",
@@ -3486,28 +3730,28 @@
         #
         position = self.safe_value(response, 'data', [])
         result = []
         for i in range(0, len(position)):
             result.append(self.parse_position(position[i], market))
         return self.filter_by_array_positions(result, 'symbol', symbols, False)
 
-    async def fetch_position(self, symbol: str, params={}):
+    def fetch_position(self, symbol: str, params={}):
         """
         fetch data on a single open contract trade position
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033_pending_position
         :param str symbol: unified market symbol of the market the position is held in, default is None
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `position structure <https://docs.ccxt.com/#/?id=position-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
-        response = await self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
+        response = self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "adl_sort": 3396,
         #                 "adl_sort_val": "0.00007786",
@@ -3702,29 +3946,29 @@
             'initialMarginPercentage': self.parse_number(initialMarginPercentage),
             'leverage': self.parse_number(leverage),
             'marginRatio': None,
             'stopLossPrice': self.omit_zero(self.safe_string(position, 'stop_loss_price')),
             'takeProfitPrice': self.omit_zero(self.safe_string(position, 'take_profit_price')),
         })
 
-    async def set_margin_mode(self, marginMode: str, symbol: Str = None, params={}):
+    def set_margin_mode(self, marginMode: str, symbol: Str = None, params={}):
         """
         set margin mode to 'cross' or 'isolated'
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http014_adjust_leverage
         :param str marginMode: 'cross' or 'isolated'
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: response from the exchange
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' setMarginMode() requires a symbol argument')
         marginMode = marginMode.lower()
         if marginMode != 'isolated' and marginMode != 'cross':
             raise BadRequest(self.id + ' setMarginMode() marginMode argument should be isolated or cross')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if market['type'] != 'swap':
             raise BadSymbol(self.id + ' setMarginMode() supports swap contracts only')
         defaultPositionType = None
         if marginMode == 'isolated':
             defaultPositionType = 1
         elif marginMode == 'cross':
@@ -3739,29 +3983,29 @@
         if (leverage < 3) or (leverage > maxLeverage):
             raise BadRequest(self.id + ' setMarginMode() leverage should be between 3 and ' + str(maxLeverage) + ' for ' + symbol)
         request = {
             'market': market['id'],
             'leverage': str(leverage),
             'position_type': positionType,  # 1: isolated, 2: cross
         }
-        return await self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
+        return self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
 
-    async def set_leverage(self, leverage: Int, symbol: Str = None, params={}):
+    def set_leverage(self, leverage: Int, symbol: Str = None, params={}):
         """
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http014_adjust_leverage
         set the level of leverage for a market
         :param float leverage: the rate of leverage
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.marginMode]: 'cross' or 'isolated'(default is 'cross')
         :returns dict: response from the exchange
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' setLeverage() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if not market['swap']:
             raise BadSymbol(self.id + ' setLeverage() supports swap contracts only')
         marginMode = None
         marginMode, params = self.handle_margin_mode_and_params('setLeverage', params, 'cross')
         positionType = None
         if marginMode == 'isolated':
@@ -3773,26 +4017,26 @@
         if (leverage < minLeverage) or (leverage > maxLeverage):
             raise BadRequest(self.id + ' setLeverage() leverage should be between ' + str(minLeverage) + ' and ' + str(maxLeverage) + ' for ' + symbol)
         request = {
             'market': market['id'],
             'leverage': str(leverage),
             'position_type': positionType,  # 1: isolated, 2: cross
         }
-        return await self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
+        return self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
 
-    async def fetch_leverage_tiers(self, symbols: Strings = None, params={}):
+    def fetch_leverage_tiers(self, symbols: Strings = None, params={}):
         """
         retrieve information on the maximum leverage, and maintenance margin for trades of varying trade sizes
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http007_market_limit
         :param str[]|None symbols: list of unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `leverage tiers structures <https://docs.ccxt.com/#/?id=leverage-tiers-structure>`, indexed by market symbols
         """
-        await self.load_markets()
-        response = await self.v1PerpetualPublicGetMarketLimitConfig(params)
+        self.load_markets()
+        response = self.v1PerpetualPublicGetMarketLimitConfig(params)
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "BTCUSD": [
         #                 ["500001", "100", "0.005"],
         #                 ["1000001", "50", "0.01"],
@@ -3823,23 +4067,23 @@
                 'maintenanceMarginRate': self.safe_number(bracket, 2),
                 'maxLeverage': self.safe_integer(bracket, 1),
                 'info': bracket,
             })
             minNotional = maxNotional
         return tiers
 
-    async def modify_margin_helper(self, symbol: str, amount, addOrReduce, params={}):
-        await self.load_markets()
+    def modify_margin_helper(self, symbol: str, amount, addOrReduce, params={}):
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'amount': self.amount_to_precision(symbol, amount),
             'type': addOrReduce,
         }
-        response = await self.v1PerpetualPrivatePostPositionAdjustMargin(self.extend(request, params))
+        response = self.v1PerpetualPrivatePostPositionAdjustMargin(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "adl_sort": 1,
         #             "adl_sort_val": "0.00004320",
         #             "amount": "0.0005",
@@ -3986,61 +4230,61 @@
             'total': self.safe_number(data, 'position_amount'),
             'code': market['quote'],
             'status': None,
             'timestamp': timestamp,
             'datetime': self.iso8601(timestamp),
         }
 
-    async def add_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
+    def add_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
         """
         add margin
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http032_adjust_position_margin
         :param str symbol: unified market symbol
         :param float amount: amount of margin to add
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `margin structure <https://docs.ccxt.com/#/?id=add-margin-structure>`
         """
-        return await self.modify_margin_helper(symbol, amount, 1, params)
+        return self.modify_margin_helper(symbol, amount, 1, params)
 
-    async def reduce_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
+    def reduce_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
         """
         remove margin from a position
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http032_adjust_position_margin
         :param str symbol: unified market symbol
         :param float amount: the amount of margin to remove
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `margin structure <https://docs.ccxt.com/#/?id=reduce-margin-structure>`
         """
-        return await self.modify_margin_helper(symbol, amount, 2, params)
+        return self.modify_margin_helper(symbol, amount, 2, params)
 
-    async def fetch_funding_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+    def fetch_funding_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch the history of funding payments paid and received on self account
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http034_funding_position
         :param str symbol: unified market symbol
         :param int [since]: the earliest time in ms to fetch funding history for
         :param int [limit]: the maximum number of funding history structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `funding history structure <https://docs.ccxt.com/#/?id=funding-history-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' fetchFundingHistory() requires a symbol argument')
         limit = 100 if (limit is None) else limit
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'limit': limit,
             # 'offset': 0,
             # 'end_time': 1638990636000,
             # 'windowtime': 1638990636000,
         }
         if since is not None:
             request['start_time'] = since
-        response = await self.v1PerpetualPrivateGetPositionFunding(self.extend(request, params))
+        response = self.v1PerpetualPrivateGetPositionFunding(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "limit": 100,
         #             "offset": 0,
         #             "records": [
@@ -4079,30 +4323,30 @@
                 'timestamp': timestamp,
                 'datetime': self.iso8601(timestamp),
                 'id': self.safe_number(entry, 'position_id'),
                 'amount': self.safe_number(entry, 'funding'),
             })
         return result
 
-    async def fetch_funding_rate(self, symbol: str, params={}):
+    def fetch_funding_rate(self, symbol: str, params={}):
         """
         fetch the current funding rate
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http008_market_ticker
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `funding rate structure <https://docs.ccxt.com/#/?id=funding-rate-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if not market['swap']:
             raise BadSymbol(self.id + ' fetchFundingRate() supports swap contracts only')
         request = {
             'market': market['id'],
         }
-        response = await self.v1PerpetualPublicGetMarketTicker(self.extend(request, params))
+        response = self.v1PerpetualPublicGetMarketTicker(self.extend(request, params))
         #
         #     {
         #          "code": 0,
         #         "data":
         #         {
         #             "date": 1650678472474,
         #             "ticker": {
@@ -4185,31 +4429,31 @@
             'nextFundingTimestamp': None,
             'nextFundingDatetime': None,
             'previousFundingRate': self.safe_number(contract, 'funding_rate_last'),
             'previousFundingTimestamp': None,
             'previousFundingDatetime': None,
         }
 
-    async def fetch_funding_rates(self, symbols: Strings = None, params={}):
+    def fetch_funding_rates(self, symbols: Strings = None, params={}):
         """
         fetch the current funding rates
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http009_market_ticker_all
         :param str[] symbols: unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of `funding rate structures <https://docs.ccxt.com/#/?id=funding-rate-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         symbols = self.market_symbols(symbols)
         market = None
         if symbols is not None:
             symbol = self.safe_value(symbols, 0)
             market = self.market(symbol)
             if not market['swap']:
                 raise BadSymbol(self.id + ' fetchFundingRates() supports swap contracts only')
-        response = await self.v1PerpetualPublicGetMarketTickerAll(params)
+        response = self.v1PerpetualPublicGetMarketTickerAll(params)
         #
         #     {
         #         "code": 0,
         #         "data":
         #         {
         #             "date": 1650678472474,
         #             "ticker": {
@@ -4249,43 +4493,43 @@
             if marketId.find('_') == -1:  # skip _signprice and _indexprice
                 marketInner = self.safe_market(marketId, None, None, 'swap')
                 ticker = tickers[marketId]
                 ticker['timestamp'] = timestamp
                 result.append(self.parse_funding_rate(ticker, marketInner))
         return self.filter_by_array(result, 'symbol', symbols)
 
-    async def withdraw(self, code: str, amount: float, address: str, tag=None, params={}):
+    def withdraw(self, code: str, amount: float, address: str, tag=None, params={}):
         """
         make a withdrawal
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account015_submit_withdraw
         :param str code: unified currency code
         :param float amount: the amount to withdraw
         :param str address: the address to withdraw to
         :param str tag:
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.network]: unified network code
         :returns dict: a `transaction structure <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         tag, params = self.handle_withdraw_tag_and_params(tag, params)
         self.check_address(address)
-        await self.load_markets()
+        self.load_markets()
         currency = self.currency(code)
         networkCode = self.safe_string_upper(params, 'network')
         params = self.omit(params, 'network')
         if tag:
             address = address + ':' + tag
         request = {
             'coin_type': currency['id'],
             'coin_address': address,  # must be authorized, inter-user transfer by a registered mobile phone number or an email address is supported
             'actual_amount': float(self.number_to_string(amount)),  # the actual amount without fees, https://www.coinex.com/fees
             'transfer_method': 'onchain',  # onchain, local
         }
         if networkCode is not None:
             request['smart_contract_name'] = self.network_code_to_id(networkCode)
-        response = await self.v1PrivatePostBalanceCoinWithdraw(self.extend(request, params))
+        response = self.v1PrivatePostBalanceCoinWithdraw(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "actual_amount": "1.00000000",
         #             "amount": "1.00000000",
         #             "coin_address": "1KAv3pazbTk2JnQ5xTo6fpKK7p1it2RzD4",
@@ -4312,46 +4556,46 @@
             'not_pass': 'failed',
             'cancel': 'canceled',
             'finish': 'ok',
             'fail': 'failed',
         }
         return self.safe_string(statuses, status, status)
 
-    async def fetch_funding_rate_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+    def fetch_funding_rate_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http038_funding_history
         fetches historical funding rate prices
         :param str symbol: unified symbol of the market to fetch the funding rate history for
         :param int [since]: timestamp in ms of the earliest funding rate to fetch
         :param int [limit]: the maximum amount of `funding rate structures <https://docs.ccxt.com/#/?id=funding-rate-history-structure>` to fetch
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param boolean [params.paginate]: default False, when True will automatically paginate by calling self endpoint multiple times. See in the docs all the [availble parameters](https://github.com/ccxt/ccxt/wiki/Manual#pagination-params)
         :param int [params.until]: timestamp in ms of the latest funding rate
         :returns dict[]: a list of `funding rate structures <https://docs.ccxt.com/#/?id=funding-rate-history-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' fetchFundingRateHistory() requires a symbol argument')
-        await self.load_markets()
+        self.load_markets()
         paginate = False
         paginate, params = self.handle_option_and_params(params, 'fetchFundingRateHistory', 'paginate')
         if paginate:
-            return await self.fetch_paginated_call_deterministic('fetchFundingRateHistory', symbol, since, limit, '8h', params, 1000)
+            return self.fetch_paginated_call_deterministic('fetchFundingRateHistory', symbol, since, limit, '8h', params, 1000)
         if limit is None:
             limit = 100
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'limit': limit,
             'offset': 0,
             # 'end_time': 1638990636,
         }
         if since is not None:
             request['start_time'] = since
         request, params = self.handle_until_option('end_time', request, params)
-        response = await self.v1PerpetualPublicGetMarketFundingHistory(self.extend(request, params))
+        response = self.v1PerpetualPublicGetMarketFundingHistory(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "offset": 0,
         #             "limit": 3,
         #             "records": [
@@ -4489,49 +4733,49 @@
             'status': status,
             'updated': None,
             'fee': fee,
             'comment': None,
             'internal': internal,
         }
 
-    async def transfer(self, code: str, amount: float, fromAccount: str, toAccount: str, params={}) -> TransferEntry:
+    def transfer(self, code: str, amount: float, fromAccount: str, toAccount: str, params={}) -> TransferEntry:
         """
         transfer currency internally between wallets on the same account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account014_balance_contract_transfer
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account013_margin_transfer
         :param str code: unified currency code
         :param float amount: amount to transfer
         :param str fromAccount: account to transfer from
         :param str toAccount: account to transfer to
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `transfer structure <https://docs.ccxt.com/#/?id=transfer-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         currency = self.currency(code)
         amountToPrecision = self.currency_to_precision(code, amount)
         request = {
             'amount': amountToPrecision,
             'coin_type': currency['id'],
         }
         response = None
         if (fromAccount == 'spot') and (toAccount == 'swap'):
             request['transfer_side'] = 'in'  # 'in' spot to swap, 'out' swap to spot
-            response = await self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
+            response = self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
         elif (fromAccount == 'swap') and (toAccount == 'spot'):
             request['transfer_side'] = 'out'  # 'in' spot to swap, 'out' swap to spot
-            response = await self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
+            response = self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
         else:
             accountsById = self.safe_value(self.options, 'accountsById', {})
             fromId = self.safe_string(accountsById, fromAccount, fromAccount)
             toId = self.safe_string(accountsById, toAccount, toAccount)
             # fromAccount and toAccount must be integers for margin transfers
             # spot is 0, use fetchBalance() to find the margin account id
             request['from_account'] = int(fromId)
             request['to_account'] = int(toId)
-            response = await self.v1PrivatePostMarginTransfer(self.extend(request, params))
+            response = self.v1PrivatePostMarginTransfer(self.extend(request, params))
         #
         #     {"code": 0, "data": null, "message": "Success"}
         #
         return self.extend(self.parse_transfer(response, currency), {
             'amount': self.parse_number(amountToPrecision),
             'fromAccount': fromAccount,
             'toAccount': toAccount,
@@ -4597,26 +4841,26 @@
             'currency': currencyCode,
             'amount': self.safe_number(transfer, 'amount'),
             'fromAccount': fromAccount,
             'toAccount': toAccount,
             'status': self.parse_transfer_status(self.safe_string_2(transfer, 'code', 'status')),
         }
 
-    async def fetch_transfers(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
+    def fetch_transfers(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch a history of internal transfers made on an account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account025_margin_transfer_history
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account024_contract_transfer_history
         :param str code: unified currency code of the currency transferred
         :param int [since]: the earliest time in ms to fetch transfers for
         :param int [limit]: the maximum number of  transfers structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `transfer structures <https://docs.ccxt.com/#/?id=transfer-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         currency = None
         request = {
             'page': 1,
             # 'limit': limit,
             # 'asset': 'USDT',
             # 'start_time': since,
             # 'end_time': 1515806440,
@@ -4635,17 +4879,17 @@
         else:
             request['limit'] = 100
         params = self.omit(params, 'page')
         marginMode = None
         marginMode, params = self.handle_margin_mode_and_params('fetchTransfers', params)
         response = None
         if marginMode is not None:
-            response = await self.v1PrivateGetMarginTransferHistory(self.extend(request, params))
+            response = self.v1PrivateGetMarginTransferHistory(self.extend(request, params))
         else:
-            response = await self.v1PrivateGetContractTransferHistory(self.extend(request, params))
+            response = self.v1PrivateGetContractTransferHistory(self.extend(request, params))
         #
         # Swap
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "records": [
@@ -4686,33 +4930,33 @@
         #         "message": "Success"
         #     }
         #
         data = self.safe_value(response, 'data', {})
         transfers = self.safe_list(data, 'records', [])
         return self.parse_transfers(transfers, currency, since, limit)
 
-    async def fetch_withdrawals(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
+    def fetch_withdrawals(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
         """
         fetch all withdrawals made from an account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account026_withdraw_list
         :param str code: unified currency code
         :param int [since]: the earliest time in ms to fetch withdrawals for
         :param int [limit]: the maximum number of withdrawals structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `transaction structures <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         request = {}
         currency = None
         if code is not None:
-            await self.load_markets()
+            self.load_markets()
             currency = self.currency(code)
             request['coin_type'] = currency['id']
         if limit is not None:
             request['Limit'] = limit
-        response = await self.v1PrivateGetBalanceCoinWithdraw(self.extend(request, params))
+        response = self.v1PrivateGetBalanceCoinWithdraw(self.extend(request, params))
         #
         #    {
         #        "code": 0,
         #        "data": {
         #            "has_next": False,
         #            "curr_page": 1,
         #            "count": 1,
@@ -4748,33 +4992,33 @@
         #    }
         #
         data = self.safe_value(response, 'data')
         if not isinstance(data, list):
             data = self.safe_value(data, 'data', [])
         return self.parse_transactions(data, currency, since, limit)
 
-    async def fetch_deposits(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
+    def fetch_deposits(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
         """
         fetch all deposits made to an account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account009_deposit_list
         :param str code: unified currency code
         :param int [since]: the earliest time in ms to fetch deposits for
         :param int [limit]: the maximum number of deposits structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `transaction structures <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         request = {}
         currency = None
         if code is not None:
-            await self.load_markets()
+            self.load_markets()
             currency = self.currency(code)
             request['coin_type'] = currency['id']
         if limit is not None:
             request['Limit'] = limit
-        response = await self.v1PrivateGetBalanceCoinDeposit(self.extend(request, params))
+        response = self.v1PrivateGetBalanceCoinDeposit(self.extend(request, params))
         #
         #    {
         #        "code": 0,
         #        "data": {
         #            "has_next": False,
         #            "curr_page": 1,
         #            "count": 1,
@@ -4843,28 +5087,28 @@
             'quoteRate': self.safe_number(quoteInfo, 'day_rate'),
             'period': 86400000,
             'timestamp': None,
             'datetime': None,
             'info': info,
         }
 
-    async def fetch_isolated_borrow_rate(self, symbol: str, params={}):
+    def fetch_isolated_borrow_rate(self, symbol: str, params={}):
         """
         fetch the rate of interest to borrow a currency for margin trading
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account007_margin_account_settings
         :param str symbol: unified symbol of the market to fetch the borrow rate for
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `isolated borrow rate structure <https://docs.ccxt.com/#/?id=isolated-borrow-rate-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
-        response = await self.v1PrivateGetMarginConfig(self.extend(request, params))
+        response = self.v1PrivateGetMarginConfig(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "market": "BTCUSDT",
         #             "leverage": 10,
         #             "BTC": {
@@ -4880,23 +5124,23 @@
         #         },
         #         "message": "Success"
         #     }
         #
         data = self.safe_value(response, 'data', {})
         return self.parse_isolated_borrow_rate(data, market)
 
-    async def fetch_isolated_borrow_rates(self, params={}):
+    def fetch_isolated_borrow_rates(self, params={}):
         """
         fetch the borrow interest rates of all currencies
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account007_margin_account_settings
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a list of `isolated borrow rate structures <https://github.com/ccxt/ccxt/wiki/Manual#isolated-borrow-rate-structure>`
         """
-        await self.load_markets()
-        response = await self.v1PrivateGetMarginConfig(params)
+        self.load_markets()
+        response = self.v1PrivateGetMarginConfig(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "market": "BTCUSDT",
         #                 "leverage": 10,
@@ -4917,24 +5161,24 @@
         #
         data = self.safe_value(response, 'data', [])
         rates = []
         for i in range(0, len(data)):
             rates.append(self.parse_isolated_borrow_rate(data[i]))
         return rates
 
-    async def fetch_borrow_interest(self, code: Str = None, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
-        await self.load_markets()
+    def fetch_borrow_interest(self, code: Str = None, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+        self.load_markets()
         request = {}
         market = None
         if symbol is not None:
             market = self.market(symbol)
             request['market'] = market['id']
         if limit is not None:
             request['limit'] = limit
-        response = await self.v1PrivateGetMarginLoanHistory(self.extend(request, params))
+        response = self.v1PrivateGetMarginLoanHistory(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "page": 1,
         #             "limit": 10,
         #             "total": 1,
@@ -5001,33 +5245,33 @@
             'interestRate': self.safe_number(info, 'day_rate'),
             'amountBorrowed': self.parse_number(loanAmount),
             'timestamp': timestamp,  # expiry time
             'datetime': self.iso8601(timestamp),
             'info': info,
         }
 
-    async def borrow_isolated_margin(self, symbol: str, code: str, amount: float, params={}):
+    def borrow_isolated_margin(self, symbol: str, code: str, amount: float, params={}):
         """
         create a loan to borrow margin
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account017_margin_loan
         :param str symbol: unified market symbol, required for coinex
         :param str code: unified currency code of the currency to borrow
         :param float amount: the amount to borrow
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `margin loan structure <https://docs.ccxt.com/#/?id=margin-loan-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         currency = self.currency(code)
         request = {
             'market': market['id'],
             'coin_type': currency['id'],
             'amount': self.currency_to_precision(code, amount),
         }
-        response = await self.v1PrivatePostMarginLoan(self.extend(request, params))
+        response = self.v1PrivatePostMarginLoan(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "loan_id": 1670
         #         },
         #         "message": "Success"
@@ -5036,34 +5280,34 @@
         data = self.safe_value(response, 'data', {})
         transaction = self.parse_margin_loan(data, currency)
         return self.extend(transaction, {
             'amount': amount,
             'symbol': symbol,
         })
 
-    async def repay_isolated_margin(self, symbol: str, code: str, amount, params={}):
+    def repay_isolated_margin(self, symbol: str, code: str, amount, params={}):
         """
         repay borrowed margin and interest
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account018_margin_flat
         :param str symbol: unified market symbol, required for coinex
         :param str code: unified currency code of the currency to repay
         :param float amount: the amount to repay
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.loan_id]: extra parameter that is not required
         :returns dict: a `margin loan structure <https://docs.ccxt.com/#/?id=margin-loan-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         currency = self.currency(code)
         request = {
             'market': market['id'],
             'coin_type': currency['id'],
             'amount': self.currency_to_precision(code, amount),
         }
-        response = await self.v1PrivatePostMarginFlat(self.extend(request, params))
+        response = self.v1PrivatePostMarginFlat(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": null,
         #         "message": "Success"
         #     }
         #
@@ -5095,29 +5339,29 @@
             'amount': None,
             'symbol': None,
             'timestamp': None,
             'datetime': None,
             'info': info,
         }
 
-    async def fetch_deposit_withdraw_fees(self, codes: Strings = None, params={}):
+    def fetch_deposit_withdraw_fees(self, codes: Strings = None, params={}):
         """
         fetch deposit and withdraw fees
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot001_market010_asset_config
         :param str[]|None codes: list of unified currency codes
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `fees structures <https://docs.ccxt.com/#/?id=fee-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         request = {}
         if codes is not None:
             codesLength = len(codes)
             if codesLength == 1:
                 request['coin_type'] = self.safe_value(codes, 0)
-        response = await self.v1PublicGetCommonAssetConfig(self.extend(request, params))
+        response = self.v1PublicGetCommonAssetConfig(self.extend(request, params))
         #
         #    {
         #        "code": 0,
         #        "data": {
         #            "CET-CSC": {
         #                "asset": "CET",
         #                "chain": "CSC",
@@ -5181,33 +5425,33 @@
         depositWithdrawCodes = list(depositWithdrawFees.keys())
         for i in range(0, len(depositWithdrawCodes)):
             code = depositWithdrawCodes[i]
             currency = self.currency(code)
             depositWithdrawFees[code] = self.assign_default_deposit_withdraw_fees(depositWithdrawFees[code], currency)
         return depositWithdrawFees
 
-    async def fetch_leverages(self, symbols: List[str] = None, params={}) -> Leverages:
+    def fetch_leverages(self, symbols: List[str] = None, params={}) -> Leverages:
         """
         fetch the set leverage for all contract and margin markets
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account007_margin_account_settings
         :param str[] [symbols]: a list of unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a list of `leverage structures <https://docs.ccxt.com/#/?id=leverage-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         symbols = self.market_symbols(symbols)
         market = None
         if symbols is not None:
             symbol = self.safe_value(symbols, 0)
             market = self.market(symbol)
         marketType = None
         marketType, params = self.handle_market_type_and_params('fetchLeverages', market, params)
         if marketType != 'spot':
             raise NotSupported(self.id + ' fetchLeverages() supports spot margin markets only')
-        response = await self.v1PrivateGetMarginConfig(params)
+        response = self.v1PrivateGetMarginConfig(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "market": "BTCUSDT",
         #                 "leverage": 10,
@@ -5236,37 +5480,37 @@
             'info': leverage,
             'symbol': self.safe_symbol(marketId, market, None, 'spot'),
             'marginMode': None,
             'longLeverage': leverageValue,
             'shortLeverage': leverageValue,
         }
 
-    async def fetch_position_history(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> Position:
+    def fetch_position_history(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> Position:
         """
         fetches historical positions
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033-0_finished_position
         :param str symbol: unified contract symbol
         :param int [since]: not used by coinex fetchPositionHistory
         :param int [limit]: the maximum amount of records to fetch, default=1000
         :param dict params: extra parameters specific to the exchange api endpoint
          *
          * EXCHANGE SPECIFIC PARAMETERS
         :param int [params.side]: 0: all 1: sell, 2: buy
         :returns dict[]: a list of `position structures <https://docs.ccxt.com/#/?id=position-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         market = self.market(symbol)
         if limit is None:
             limit = 1000
         request = {
             'market': market['id'],
             'side': 0,
             'limit': limit,
         }
-        response = await self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
+        response = self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
         #
         #    {
         #        code: '0',
         #        data: {
         #            limit: '1000',
         #            offset: '0',
         #            records: [
@@ -5400,28 +5644,29 @@
                 else:
                     body = self.json(query)
             elif version == 'v2':
                 self.check_required_credentials()
                 query = self.keysort(query)
                 urlencoded = self.rawencode(query)
                 preparedString = method + '/' + version + '/' + path
-                if urlencoded:
+                if method == 'POST':
+                    body = self.json(query)
+                    preparedString += body
+                elif urlencoded:
                     preparedString += '?' + urlencoded
                 preparedString += nonce + self.secret
                 signature = self.hash(self.encode(preparedString), 'sha256')
                 headers = {
                     'X-COINEX-KEY': self.apiKey,
                     'X-COINEX-SIGN': signature,
                     'X-COINEX-TIMESTAMP': nonce,
                 }
-                if (method == 'GET') or (method == 'DELETE') or (method == 'PUT'):
+                if method != 'POST':
                     if urlencoded:
                         url += '?' + urlencoded
-                else:
-                    body = self.json(query)
         return {'url': url, 'method': method, 'body': body, 'headers': headers}
 
     def handle_errors(self, httpCode, reason, url, method, headers, body, response, requestHeaders, requestBody):
         if response is None:
             return None
         code = self.safe_string(response, 'code')
         data = self.safe_value(response, 'data')
@@ -5429,30 +5674,30 @@
         if (code != '0') or ((message != 'Success') and (message != 'Succeeded') and (message != 'Ok') and not data):
             feedback = self.id + ' ' + message
             self.throw_broadly_matched_exception(self.exceptions['broad'], message, feedback)
             self.throw_exactly_matched_exception(self.exceptions['exact'], code, feedback)
             raise ExchangeError(feedback)
         return None
 
-    async def fetch_margin_adjustment_history(self, symbol: Str = None, type: Str = None, since: Num = None, limit: Num = None, params={}) -> List[MarginModification]:
+    def fetch_margin_adjustment_history(self, symbol: Str = None, type: Str = None, since: Num = None, limit: Num = None, params={}) -> List[MarginModification]:
         """
         fetches the history of margin added or reduced from contract isolated positions
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http046_position_margin_history
         :param str [symbol]: unified market symbol
         :param str [type]: not used by coinex fetchMarginAdjustmentHistory
         :param int [since]: timestamp in ms of the earliest change to fetch
         :param int [limit]: the maximum amount of changes to fetch, default=100, max=100
         :param dict params: extra parameters specific to the exchange api endpoint
         :param int [params.until]: timestamp in ms of the latest change to fetch
          *
          * EXCHANGE SPECIFIC PARAMETERS
         :param int [params.offset]: offset
         :returns dict[]: a list of `margin structures <https://docs.ccxt.com/#/?id=margin-loan-structure>`
         """
-        await self.load_markets()
+        self.load_markets()
         until = self.safe_integer(params, 'until')
         params = self.omit(params, 'until')
         if limit is None:
             limit = 100
         request = {
             'market': '',
             'position_id': 0,
@@ -5462,15 +5707,15 @@
         if symbol is not None:
             market = self.market(symbol)
             request['market'] = market['id']
         if since is not None:
             request['start_time'] = since
         if until is not None:
             request['end_time'] = until
-        response = await self.v1PerpetualPrivateGetPositionMarginHistory(self.extend(request, params))
+        response = self.v1PerpetualPrivateGetPositionMarginHistory(self.extend(request, params))
         #
         #    {
         #        code: '0',
         #        data: {
         #            limit: '100',
         #            offset: '0',
         #            records: [
```

### Comparing `ccxt-4.3.8/ccxt/async_support/coinlist.py` & `ccxt-4.3.9/ccxt/async_support/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinmate.py` & `ccxt-4.3.9/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinmetro.py` & `ccxt-4.3.9/ccxt/async_support/coinmetro.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
                         'exchange/book/{pair}': 3,
                         'exchange/bookUpdates/{pair}/{from}': 1,  # not unified
                     },
                 },
                 'private': {
                     'get': {
                         'users/balances': 1,
+                        'users/wallets': 1,
                         'users/wallets/history/{since}': 1.67,
                         'exchange/orders/status/{orderID}': 1,
                         'exchange/orders/active': 1,
                         'exchange/orders/history/{since}': 1.67,
                         'exchange/fills/{since}': 1.67,
                         'exchange/margin': 1,  # not unified
                     },
@@ -906,57 +907,56 @@
             'quoteVolume': None,
             'info': ticker,
         }, market)
 
     async def fetch_balance(self, params={}) -> Balances:
         """
         query for balance and get the amount of funds available for trading or funds locked in orders
-        :see: https://documenter.getpostman.com/view/3653795/SVfWN6KS#698ae067-43dd-4e19-a0ac-d9ba91381816
+        :see: https://documenter.getpostman.com/view/3653795/SVfWN6KS#741a1dcc-7307-40d0-acca-28d003d1506a
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `balance structure <https://docs.ccxt.com/#/?id=balance-structure>`
         """
         await self.load_markets()
-        response = await self.privateGetUsersBalances(params)
-        return self.parse_balance(response)
+        response = await self.privateGetUsersWallets(params)
+        list = self.safe_list(response, 'list', [])
+        return self.parse_balance(list)
 
-    def parse_balance(self, response) -> Balances:
+    def parse_balance(self, balances) -> Balances:
         #
-        #     {
-        #         "USDC": {
-        #             "USDC": 99,
-        #             "EUR": 91.16,
-        #             "BTC": 0.002334
-        #         },
-        #         "XCM": {
-        #             "XCM": 0,
-        #             "EUR": 0,
-        #             "BTC": 0
-        #         },
-        #         "TOTAL": {
-        #             "EUR": 91.16,
-        #             "BTC": 0.002334
+        #     [
+        #         {
+        #             "xcmLocks": [],
+        #             "xcmLockAmounts": [],
+        #             "refList": [],
+        #             "balanceHistory": [],
+        #             "_id": "5fecd3c998e75c2e4d63f7c3",
+        #             "currency": "BTC",
+        #             "label": "BTC",
+        #             "userId": "5fecd3c97fbfed1521db23bd",
+        #             "__v": 0,
+        #             "balance": 0.5,
+        #             "createdAt": "2020-12-30T19:23:53.646Z",
+        #             "disabled": False,
+        #             "updatedAt": "2020-12-30T19:23:53.653Z",
+        #             "reserved": 0,
+        #             "id": "5fecd3c998e75c2e4d63f7c3"
         #         },
-        #         "REF": {
-        #             "XCM": 0,
-        #             "EUR": 0,
-        #             "BTC": 0
-        #         }
-        #     }
+        #         ...
+        #     ]
         #
         result = {
-            'info': response,
+            'info': balances,
         }
-        balances = self.omit(response, ['TOTAL', 'REF'])
-        currencyIds = list(balances.keys())
-        for i in range(0, len(currencyIds)):
-            currencyId = currencyIds[i]
+        for i in range(0, len(balances)):
+            balanceEntry = self.safe_dict(balances, i, {})
+            currencyId = self.safe_string(balanceEntry, 'currency')
             code = self.safe_currency_code(currencyId)
             account = self.account()
-            currency = self.safe_value(balances, currencyId, {})
-            account['total'] = self.safe_string(currency, currencyId)
+            account['total'] = self.safe_string(balanceEntry, 'balance')
+            account['used'] = self.safe_string(balanceEntry, 'reserved')
             result[code] = account
         return self.safe_balance(result)
 
     async def fetch_ledger(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch the history of changes, actions done by the user or operations that altered balance of the user
         :see: https://documenter.getpostman.com/view/3653795/SVfWN6KS#4e7831f7-a0e7-4c3e-9336-1d0e5dcb15cf
```

### Comparing `ccxt-4.3.8/ccxt/async_support/coinone.py` & `ccxt-4.3.9/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinsph.py` & `ccxt-4.3.9/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/coinspot.py` & `ccxt-4.3.9/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/cryptocom.py` & `ccxt-4.3.9/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/currencycom.py` & `ccxt-4.3.9/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/delta.py` & `ccxt-4.3.9/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/deribit.py` & `ccxt-4.3.9/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/digifinex.py` & `ccxt-4.3.9/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/exmo.py` & `ccxt-4.3.9/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/flowbtc.py` & `ccxt-4.3.9/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/fmfwio.py` & `ccxt-4.3.9/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/gate.py` & `ccxt-4.3.9/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/gemini.py` & `ccxt-4.3.9/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/hitbtc.py` & `ccxt-4.3.9/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/hollaex.py` & `ccxt-4.3.9/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/htx.py` & `ccxt-4.3.9/ccxt/async_support/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/huobijp.py` & `ccxt-4.3.9/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/hyperliquid.py` & `ccxt-4.3.9/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/idex.py` & `ccxt-4.3.9/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/independentreserve.py` & `ccxt-4.3.9/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/indodax.py` & `ccxt-4.3.9/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/kraken.py` & `ccxt-4.3.9/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/krakenfutures.py` & `ccxt-4.3.9/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/kucoin.py` & `ccxt-4.3.9/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/kucoinfutures.py` & `ccxt-4.3.9/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/kuna.py` & `ccxt-4.3.9/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/latoken.py` & `ccxt-4.3.9/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/lbank.py` & `ccxt-4.3.9/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/luno.py` & `ccxt-4.3.9/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/lykke.py` & `ccxt-4.3.9/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/mercado.py` & `ccxt-4.3.9/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/mexc.py` & `ccxt-4.3.9/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/ndax.py` & `ccxt-4.3.9/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/novadax.py` & `ccxt-4.3.9/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/oceanex.py` & `ccxt-4.3.9/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/okcoin.py` & `ccxt-4.3.9/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/okx.py` & `ccxt-4.3.9/ccxt/async_support/okx.py`

 * *Files 2% similar despite different names*

```diff
@@ -2544,14 +2544,16 @@
         clientOrderId = self.safe_string_2(params, 'clOrdId', 'clientOrderId')
         stopLoss = self.safe_value(params, 'stopLoss')
         stopLossDefined = (stopLoss is not None)
         takeProfit = self.safe_value(params, 'takeProfit')
         takeProfitDefined = (takeProfit is not None)
         trailingPercent = self.safe_string_2(params, 'trailingPercent', 'callbackRatio')
         isTrailingPercentOrder = trailingPercent is not None
+        trigger = (triggerPrice is not None) or (type == 'trigger')
+        isReduceOnly = self.safe_value(params, 'reduceOnly', False)
         defaultMarginMode = self.safe_string_2(self.options, 'defaultMarginMode', 'marginMode', 'cross')
         marginMode = self.safe_string_2(params, 'marginMode', 'tdMode')  # cross or isolated, tdMode not ommited so be extended into the request
         margin = False
         if (marginMode is not None) and (marginMode != 'cash'):
             margin = True
         else:
             marginMode = defaultMarginMode
@@ -2565,22 +2567,35 @@
             request['tdMode'] = tradeMode
         elif contract:
             if market['swap'] or market['future']:
                 positionSide = None
                 positionSide, params = self.handle_option_and_params(params, 'createOrder', 'positionSide')
                 if positionSide is not None:
                     request['posSide'] = positionSide
+                else:
+                    hedged = None
+                    hedged, params = self.handle_option_and_params(params, 'createOrder', 'hedged')
+                    if hedged:
+                        isBuy = (side == 'buy')
+                        isProtective = (takeProfitPrice is not None) or (stopLossPrice is not None) or isReduceOnly
+                        if isProtective:
+                            # in case of protective orders, the posSide should be opposite of position side
+                            # reduceOnly is emulated and not natively supported by the exchange
+                            request['posSide'] = 'short' if isBuy else 'long'
+                            if isReduceOnly:
+                                params = self.omit(params, 'reduceOnly')
+                        else:
+                            request['posSide'] = 'long' if isBuy else 'short'
             request['tdMode'] = marginMode
         isMarketOrder = type == 'market'
         postOnly = False
         postOnly, params = self.handle_post_only(isMarketOrder, type == 'post_only', params)
         params = self.omit(params, ['currency', 'ccy', 'marginMode', 'timeInForce', 'stopPrice', 'triggerPrice', 'clientOrderId', 'stopLossPrice', 'takeProfitPrice', 'slOrdPx', 'tpOrdPx', 'margin', 'stopLoss', 'takeProfit', 'trailingPercent'])
         ioc = (timeInForce == 'IOC') or (type == 'ioc')
         fok = (timeInForce == 'FOK') or (type == 'fok')
-        trigger = (triggerPrice is not None) or (type == 'trigger')
         conditional = (stopLossPrice is not None) or (takeProfitPrice is not None) or (type == 'conditional')
         marketIOC = (isMarketOrder and ioc) or (type == 'optimal_limit_ioc')
         defaultTgtCcy = self.safe_string(self.options, 'tgtCcy', 'base_ccy')
         tgtCcy = self.safe_string(params, 'tgtCcy', defaultTgtCcy)
         if (not contract) and (not margin):
             request['tgtCcy'] = tgtCcy
         if isMarketOrder or marketIOC:
@@ -2731,14 +2746,15 @@
         :param dict [params.stopLoss]: *stopLoss object in params* containing the triggerPrice at which the attached stop loss order will be triggered(perpetual swap markets only)
         :param float [params.stopLoss.triggerPrice]: stop loss trigger price
         :param float [params.stopLoss.price]: used for stop loss limit orders, not used for stop loss market price orders
         :param str [params.stopLoss.type]: 'market' or 'limit' used to specify the stop loss price type
         :param str [params.positionSide]: if position mode is one-way: set to 'net', if position mode is hedge-mode: set to 'long' or 'short'
         :param str [params.trailingPercent]: the percent to trail away from the current market price
         :param str [params.tpOrdKind]: 'condition' or 'limit', the default is 'condition'
+        :param str [params.hedged]: True/false, to automatically set exchange-specific params needed when trading in hedge mode
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         await self.load_markets()
         market = self.market(symbol)
         request = self.create_order_request(symbol, type, side, amount, price, params)
         method = self.safe_string(self.options, 'createOrder', 'privatePostTradeBatchOrders')
         requestOrdType = self.safe_string(request, 'ordType')
@@ -5848,14 +5864,44 @@
         #         }
         #       ],
         #       "msg": ""
         #     }
         #
         return response
 
+    async def fetch_position_mode(self, symbol: Str = None, params={}):
+        """
+        :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-get-account-configuration
+        fetchs the position mode, hedged or one way, hedged for binance is set identically for all linear markets or all inverse markets
+        :param str symbol: unified symbol of the market to fetch the order book for
+        :param dict [params]: extra parameters specific to the exchange API endpoint
+        :param str [param.accountId]: if you have multiple accounts, you must specify the account id to fetch the position mode
+        :returns dict: an object detailing whether the market is in hedged or one-way mode
+        """
+        accounts = await self.fetch_accounts()
+        length = len(accounts)
+        selectedAccount = None
+        if length > 1:
+            accountId = self.safe_string(params, 'accountId')
+            if accountId is None:
+                accountIds = self.get_list_from_object_values(accounts, 'id')
+                raise ExchangeError(self.id + ' fetchPositionMode() can not detect position mode, because you have multiple accounts. Set params["accountId"] to desired id from: ' + ', '.join(accountIds))
+            else:
+                accountsById = self.index_by(accounts, 'id')
+                selectedAccount = self.safe_dict(accountsById, accountId)
+        else:
+            selectedAccount = accounts[0]
+        mainAccount = selectedAccount['info']
+        posMode = self.safe_string(mainAccount, 'posMode')  # long_short_mode, net_mode
+        isHedged = posMode == 'long_short_mode'
+        return {
+            'info': mainAccount,
+            'hedged': isHedged,
+        }
+
     async def set_position_mode(self, hedged: bool, symbol: Str = None, params={}):
         """
         set hedged to True or False for a market
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-set-position-mode
         :param bool hedged: set to True to use long_short_mode, False for net_mode
         :param str symbol: not used by okx setPositionMode
         :param dict [params]: extra parameters specific to the exchange API endpoint
```

### Comparing `ccxt-4.3.8/ccxt/async_support/onetrading.py` & `ccxt-4.3.9/ccxt/async_support/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/p2b.py` & `ccxt-4.3.9/ccxt/async_support/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/paymium.py` & `ccxt-4.3.9/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/phemex.py` & `ccxt-4.3.9/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/poloniex.py` & `ccxt-4.3.9/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/poloniexfutures.py` & `ccxt-4.3.9/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/probit.py` & `ccxt-4.3.9/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/timex.py` & `ccxt-4.3.9/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/tokocrypto.py` & `ccxt-4.3.9/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/tradeogre.py` & `ccxt-4.3.9/ccxt/async_support/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/upbit.py` & `ccxt-4.3.9/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/wavesexchange.py` & `ccxt-4.3.9/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/wazirx.py` & `ccxt-4.3.9/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/whitebit.py` & `ccxt-4.3.9/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/woo.py` & `ccxt-4.3.9/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/yobit.py` & `ccxt-4.3.9/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/zaif.py` & `ccxt-4.3.9/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/async_support/zonda.py` & `ccxt-4.3.9/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/base/__init__.py` & `ccxt-4.3.9/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/base/decimal_to_precision.py` & `ccxt-4.3.9/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/base/errors.py` & `ccxt-4.3.9/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/base/exchange.py` & `ccxt-4.3.9/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.3.8'
+__version__ = '4.3.9'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-4.3.8/ccxt/base/precise.py` & `ccxt-4.3.9/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/base/types.py` & `ccxt-4.3.9/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bequant.py` & `ccxt-4.3.9/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bigone.py` & `ccxt-4.3.9/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/binance.py` & `ccxt-4.3.9/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/binancecoinm.py` & `ccxt-4.3.9/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/binanceus.py` & `ccxt-4.3.9/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/binanceusdm.py` & `ccxt-4.3.9/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bingx.py` & `ccxt-4.3.9/ccxt/bingx.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,14 @@
                 },
                 'subAccount': {
                     'v1': {
                         'private': {
                             'get': {
                                 'list': 3,
                                 'assets': 3,
-                                'apiKey/query': 1,
                             },
                             'post': {
                                 'create': 3,
                                 'apiKey/create': 3,
                                 'apiKey/edit': 3,
                                 'apiKey/del': 3,
                                 'updateStatus': 3,
@@ -316,14 +315,15 @@
                     },
                 },
                 'account': {
                     'v1': {
                         'private': {
                             'get': {
                                 'uid': 1,
+                                'apiKey/query': 1,
                             },
                             'post': {
                                 'innerTransfer/authorizeSubAccount': 3,
                             },
                         },
                     },
                 },
@@ -1751,27 +1751,32 @@
         request: dict = {
             'symbol': market['id'],
             'type': type,
             'side': side.upper(),
         }
         isMarketOrder = type == 'MARKET'
         isSpot = marketType == 'spot'
+        stopLossPrice = self.safe_string(params, 'stopLossPrice')
+        takeProfitPrice = self.safe_string(params, 'takeProfitPrice')
+        triggerPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
+        isTriggerOrder = triggerPrice is not None
+        isStopLossPriceOrder = stopLossPrice is not None
+        isTakeProfitPriceOrder = takeProfitPrice is not None
         exchangeClientOrderId = 'newClientOrderId' if isSpot else 'clientOrderID'
         clientOrderId = self.safe_string_2(params, exchangeClientOrderId, 'clientOrderId')
         if clientOrderId is not None:
             request[exchangeClientOrderId] = clientOrderId
         timeInForce = self.safe_string_upper(params, 'timeInForce')
         postOnly, params = self.handle_post_only(isMarketOrder, timeInForce == 'PostOnly', params)
         if postOnly or (timeInForce == 'PostOnly'):
             request['timeInForce'] = 'PostOnly'
         elif timeInForce == 'IOC':
             request['timeInForce'] = 'IOC'
         elif timeInForce == 'GTC':
             request['timeInForce'] = 'GTC'
-        triggerPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
         if isSpot:
             cost = self.safe_number_2(params, 'cost', 'quoteOrderQty')
             params = self.omit(params, 'cost')
             if cost is not None:
                 request['quoteOrderQty'] = self.parse_to_numeric(self.cost_to_precision(symbol, cost))
             else:
                 if isMarketOrder and (price is not None):
@@ -1786,25 +1791,27 @@
                 if isMarketOrder and self.safe_string(request, 'quoteOrderQty') is None:
                     raise ArgumentsRequired(self.id + ' createOrder() requires the cost parameter(or the amount + price) for placing spot market-buy trigger orders')
                 request['stopPrice'] = self.price_to_precision(symbol, triggerPrice)
                 if type == 'LIMIT':
                     request['type'] = 'TRIGGER_LIMIT'
                 elif type == 'MARKET':
                     request['type'] = 'TRIGGER_MARKET'
+            elif (stopLossPrice is not None) or (takeProfitPrice is not None):
+                stopTakePrice = stopLossPrice if (stopLossPrice is not None) else takeProfitPrice
+                if type == 'LIMIT':
+                    request['type'] = 'TAKE_STOP_LIMIT'
+                elif type == 'MARKET':
+                    request['type'] = 'TAKE_STOP_MARKET'
+                request['stopPrice'] = self.parse_to_numeric(self.price_to_precision(symbol, stopTakePrice))
         else:
             if timeInForce == 'FOK':
                 request['timeInForce'] = 'FOK'
-            stopLossPrice = self.safe_string(params, 'stopLossPrice')
-            takeProfitPrice = self.safe_string(params, 'takeProfitPrice')
             trailingAmount = self.safe_string(params, 'trailingAmount')
             trailingPercent = self.safe_string_2(params, 'trailingPercent', 'priceRate')
             trailingType = self.safe_string(params, 'trailingType', 'TRAILING_STOP_MARKET')
-            isTriggerOrder = triggerPrice is not None
-            isStopLossPriceOrder = stopLossPrice is not None
-            isTakeProfitPriceOrder = takeProfitPrice is not None
             isTrailingAmountOrder = trailingAmount is not None
             isTrailingPercentOrder = trailingPercent is not None
             isTrailing = isTrailingAmountOrder or isTrailingPercentOrder
             stopLoss = self.safe_value(params, 'stopLoss')
             takeProfit = self.safe_value(params, 'takeProfit')
             isStopLoss = stopLoss is not None
             isTakeProfit = takeProfit is not None
@@ -1874,15 +1881,15 @@
             positionSide = None
             if reduceOnly:
                 positionSide = 'SHORT' if (side == 'buy') else 'LONG'
             else:
                 positionSide = 'LONG' if (side == 'buy') else 'SHORT'
             request['positionSide'] = positionSide
             request['quantity'] = self.parse_to_numeric(self.amount_to_precision(symbol, amount))
-            params = self.omit(params, ['reduceOnly', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice', 'trailingAmount', 'trailingPercent', 'trailingType', 'takeProfit', 'stopLoss', 'clientOrderId'])
+        params = self.omit(params, ['reduceOnly', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice', 'trailingAmount', 'trailingPercent', 'trailingType', 'takeProfit', 'stopLoss', 'clientOrderId'])
         return self.extend(request, params)
 
     def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
         """
         create a trade order
         :see: https://bingx-api.github.io/docs/#/en-us/swapV2/trade-api.html#Trade%20order
         :see: https://bingx-api.github.io/docs/#/en-us/spot/trade-api.html#Create%20an%20Order
@@ -1892,17 +1899,17 @@
         :param float amount: how much you want to trade in units of the base currency
         :param float [price]: the price at which the order is to be fullfilled, in units of the quote currency, ignored in market orders
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.clientOrderId]: a unique id for the order
         :param bool [params.postOnly]: True to place a post only order
         :param str [params.timeInForce]: spot supports 'PO', 'GTC' and 'IOC', swap supports 'PO', 'GTC', 'IOC' and 'FOK'
         :param bool [params.reduceOnly]: *swap only* True or False whether the order is reduce only
-        :param float [params.triggerPrice]: *swap only* triggerPrice at which the attached take profit / stop loss order will be triggered
-        :param float [params.stopLossPrice]: *swap only* stop loss trigger price
-        :param float [params.takeProfitPrice]: *swap only* take profit trigger price
+        :param float [params.triggerPrice]: triggerPrice at which the attached take profit / stop loss order will be triggered
+        :param float [params.stopLossPrice]: stop loss trigger price
+        :param float [params.takeProfitPrice]: take profit trigger price
         :param float [params.cost]: the quote quantity that can be used alternative for the amount
         :param float [params.trailingAmount]: *swap only* the quote amount to trail away from the current market price
         :param float [params.trailingPercent]: *swap only* the percent to trail away from the current market price
         :param dict [params.takeProfit]: *takeProfit object in params* containing the triggerPrice at which the attached take profit order will be triggered
         :param float [params.takeProfit.triggerPrice]: take profit trigger price
         :param dict [params.stopLoss]: *stopLoss object in params* containing the triggerPrice at which the attached stop loss order will be triggered
         :param float [params.stopLoss.triggerPrice]: stop loss trigger price
```

### Comparing `ccxt-4.3.8/ccxt/bit2c.py` & `ccxt-4.3.9/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitbank.py` & `ccxt-4.3.9/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitbns.py` & `ccxt-4.3.9/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitfinex.py` & `ccxt-4.3.9/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitfinex2.py` & `ccxt-4.3.9/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitflyer.py` & `ccxt-4.3.9/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitget.py` & `ccxt-4.3.9/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bithumb.py` & `ccxt-4.3.9/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitmart.py` & `ccxt-4.3.9/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitmex.py` & `ccxt-4.3.9/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitopro.py` & `ccxt-4.3.9/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitrue.py` & `ccxt-4.3.9/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitso.py` & `ccxt-4.3.9/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitstamp.py` & `ccxt-4.3.9/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitteam.py` & `ccxt-4.3.9/ccxt/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bitvavo.py` & `ccxt-4.3.9/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bl3p.py` & `ccxt-4.3.9/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/blockchaincom.py` & `ccxt-4.3.9/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/blofin.py` & `ccxt-4.3.9/ccxt/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/btcalpha.py` & `ccxt-4.3.9/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/btcbox.py` & `ccxt-4.3.9/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/btcmarkets.py` & `ccxt-4.3.9/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/btcturk.py` & `ccxt-4.3.9/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/bybit.py` & `ccxt-4.3.9/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/cex.py` & `ccxt-4.3.9/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinbase.py` & `ccxt-4.3.9/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinbaseinternational.py` & `ccxt-4.3.9/ccxt/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinbasepro.py` & `ccxt-4.3.9/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coincheck.py` & `ccxt-4.3.9/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinex.py` & `ccxt-4.3.9/ccxt/async_support/coinex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
-from ccxt.base.exchange import Exchange
+from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.coinex import ImplicitAPI
+import asyncio
 from ccxt.base.types import Balances, Currencies, Currency, Int, Leverage, Leverages, MarginModification, Market, Num, Order, OrderRequest, OrderSide, OrderType, Position, Str, Strings, Ticker, Tickers, Trade, TradingFeeInterface, TradingFees, Transaction, TransferEntry
 from typing import List
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
@@ -488,16 +489,16 @@
                 'broad': {
                     'ip not allow visit': PermissionDenied,
                     'service too busy': ExchangeNotAvailable,
                 },
             },
         })
 
-    def fetch_currencies(self, params={}) -> Currencies:
-        response = self.v1PublicGetCommonAssetConfig(params)
+    async def fetch_currencies(self, params={}) -> Currencies:
+        response = await self.v1PublicGetCommonAssetConfig(params)
         #     {
         #         "code": 0,
         #         "data": {
         #             "USDT-ERC20": {
         #                  "asset": "USDT",
         #                  "chain": "ERC20",
         #                  "withdrawal_precision": 6,
@@ -611,33 +612,33 @@
             result[code]['info'] = info
             result[code]['fee'] = self.parse_number(minFeeString)
             result[code]['precision'] = self.parse_number(minPrecisionString)
             result[code]['limits']['deposit']['min'] = self.parse_number(minDepositString)
             result[code]['limits']['withdraw']['min'] = self.parse_number(minWithdrawString)
         return result
 
-    def fetch_markets(self, params={}) -> List[Market]:
+    async def fetch_markets(self, params={}) -> List[Market]:
         """
         retrieves data on all markets for coinex
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of objects representing market data
         """
         promisesUnresolved = [
             self.fetch_spot_markets(params),
             self.fetch_contract_markets(params),
         ]
-        promises = promisesUnresolved
+        promises = await asyncio.gather(*promisesUnresolved)
         spotMarkets = promises[0]
         swapMarkets = promises[1]
         return self.array_concat(spotMarkets, swapMarkets)
 
-    def fetch_spot_markets(self, params):
-        response = self.v2PublicGetSpotMarket(params)
+    async def fetch_spot_markets(self, params):
+        response = await self.v2PublicGetSpotMarket(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "base_ccy": "SORA",
         #                 "base_ccy_precision": 8,
@@ -713,16 +714,16 @@
                     },
                 },
                 'created': None,
                 'info': market,
             })
         return result
 
-    def fetch_contract_markets(self, params):
-        response = self.v2PublicGetFuturesMarket(params)
+    async def fetch_contract_markets(self, params):
+        response = await self.v2PublicGetFuturesMarket(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "base_ccy": "BTC",
         #                 "base_ccy_precision": 8,
@@ -869,33 +870,33 @@
             'percentage': None,
             'average': None,
             'baseVolume': self.safe_string(ticker, 'volume'),
             'quoteVolume': None,
             'info': ticker,
         }, market)
 
-    def fetch_ticker(self, symbol: str, params={}) -> Ticker:
+    async def fetch_ticker(self, symbol: str, params={}) -> Ticker:
         """
         fetches a price ticker, a statistical calculation with the information calculated over the past 24 hours for a specific market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-ticker
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-ticker
         :param str symbol: unified symbol of the market to fetch the ticker for
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `ticker structure <https://docs.ccxt.com/#/?id=ticker-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
         response = None
         if market['swap']:
-            response = self.v2PublicGetFuturesTicker(self.extend(request, params))
+            response = await self.v2PublicGetFuturesTicker(self.extend(request, params))
         else:
-            response = self.v2PublicGetSpotTicker(self.extend(request, params))
+            response = await self.v2PublicGetSpotTicker(self.extend(request, params))
         #
         # Spot
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -939,35 +940,35 @@
         #         "message": "OK"
         #     }
         #
         data = self.safe_list(response, 'data', [])
         result = self.safe_dict(data, 0, {})
         return self.parse_ticker(result, market)
 
-    def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
+    async def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
         """
         fetches price tickers for multiple markets, statistical information calculated over the past 24 hours for each market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-ticker
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-ticker
         :param str[]|None symbols: unified symbols of the markets to fetch the ticker for, all market tickers are returned if not assigned
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `ticker structures <https://docs.ccxt.com/#/?id=ticker-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         symbols = self.market_symbols(symbols)
         market = None
         if symbols is not None:
             symbol = self.safe_value(symbols, 0)
             market = self.market(symbol)
         marketType, query = self.handle_market_type_and_params('fetchTickers', market, params)
         response = None
         if marketType == 'swap':
-            response = self.v2PublicGetFuturesTicker(query)
+            response = await self.v2PublicGetFuturesTicker(query)
         else:
-            response = self.v2PublicGetSpotTicker(query)
+            response = await self.v2PublicGetSpotTicker(query)
         #
         # Spot
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -1010,56 +1011,56 @@
         #         ],
         #         "message": "OK"
         #     }
         #
         data = self.safe_list(response, 'data', [])
         return self.parse_tickers(data, symbols)
 
-    def fetch_time(self, params={}):
+    async def fetch_time(self, params={}):
         """
         fetches the current integer timestamp in milliseconds from the exchange server
         :see: https://docs.coinex.com/api/v2/common/http/time
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns int: the current integer timestamp in milliseconds from the exchange server
         """
-        response = self.v2PublicGetTime(params)
+        response = await self.v2PublicGetTime(params)
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "timestamp": 1711699867777
         #         },
         #         "message": "OK"
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         return self.safe_integer(data, 'timestamp')
 
-    def fetch_order_book(self, symbol: str, limit: Int = 20, params={}):
+    async def fetch_order_book(self, symbol: str, limit: Int = 20, params={}):
         """
         fetches information on open orders with bid(buy) and ask(sell) prices, volumes and other data
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-depth
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-depth
         :param str symbol: unified symbol of the market to fetch the order book for
         :param int [limit]: the maximum amount of order book entries to return
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: A dictionary of `order book structures <https://docs.ccxt.com/#/?id=order-book-structure>` indexed by market symbols
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if limit is None:
             limit = 20  # default
         request = {
             'market': market['id'],
             'limit': limit,
             'interval': '0',
         }
         response = None
         if market['swap']:
-            response = self.v2PublicGetFuturesDepth(self.extend(request, params))
+            response = await self.v2PublicGetFuturesDepth(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": {
             #             "depth": {
             #                 "asks": [
             #                     ["70851.94", "0.2119"],
@@ -1078,15 +1079,15 @@
             #             "is_full": True,
             #             "market": "BTCUSDT"
             #         },
             #         "message": "OK"
             #     }
             #
         else:
-            response = self.v2PublicGetSpotDepth(self.extend(request, params))
+            response = await self.v2PublicGetSpotDepth(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": {
             #             "depth": {
             #                 "asks": [
             #                     ["70875.31", "0.28670282"],
@@ -1225,38 +1226,38 @@
             'takerOrMaker': takerOrMaker,
             'price': priceString,
             'amount': amountString,
             'cost': costString,
             'fee': fee,
         }, market)
 
-    def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
+    async def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
         """
         get the list of the most recent trades for a particular symbol
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-deals
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-deals
         :param str symbol: unified symbol of the market to fetch trades for
         :param int [since]: timestamp in ms of the earliest trade to fetch
         :param int [limit]: the maximum amount of trades to fetch
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Trade[]: a list of `trade structures <https://docs.ccxt.com/#/?id=public-trades>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             # 'last_id': 0,
         }
         if limit is not None:
             request['limit'] = limit
         response = None
         if market['swap']:
-            response = self.v2PublicGetFuturesDeals(self.extend(request, params))
+            response = await self.v2PublicGetFuturesDeals(self.extend(request, params))
         else:
-            response = self.v2PublicGetSpotDeals(self.extend(request, params))
+            response = await self.v2PublicGetSpotDeals(self.extend(request, params))
         #
         # Spot and Swap
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -1268,31 +1269,31 @@
         #             },
         #         ],
         #         "message": "OK"
         #     }
         #
         return self.parse_trades(response['data'], market, since, limit)
 
-    def fetch_trading_fee(self, symbol: str, params={}) -> TradingFeeInterface:
+    async def fetch_trading_fee(self, symbol: str, params={}) -> TradingFeeInterface:
         """
         fetch the trading fees for a market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `fee structure <https://docs.ccxt.com/#/?id=fee-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
         response = None
         if market['spot']:
-            response = self.v2PublicGetSpotMarket(self.extend(request, params))
+            response = await self.v2PublicGetSpotMarket(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1306,15 +1307,15 @@
             #                 "taker_fee_rate": "0.002"
             #             }
             #         ],
             #         "message": "OK"
             #     }
             #
         else:
-            response = self.v2PublicGetFuturesMarket(self.extend(request, params))
+            response = await self.v2PublicGetFuturesMarket(self.extend(request, params))
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1332,28 +1333,28 @@
             #         "message": "OK"
             #     }
             #
         data = self.safe_list(response, 'data', [])
         result = self.safe_dict(data, 0, {})
         return self.parse_trading_fee(result, market)
 
-    def fetch_trading_fees(self, params={}) -> TradingFees:
+    async def fetch_trading_fees(self, params={}) -> TradingFees:
         """
         fetch the trading fees for multiple markets
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `fee structures <https://docs.ccxt.com/#/?id=fee-structure>` indexed by market symbols
         """
-        self.load_markets()
+        await self.load_markets()
         type = None
         type, params = self.handle_market_type_and_params('fetchTradingFees', None, params)
         response = None
         if type == 'swap':
-            response = self.v2PublicGetFuturesMarket(params)
+            response = await self.v2PublicGetFuturesMarket(params)
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1368,15 +1369,15 @@
             #                 "taker_fee_rate": "0"
             #             }
             #         ],
             #         "message": "OK"
             #     }
             #
         else:
-            response = self.v2PublicGetSpotMarket(params)
+            response = await self.v2PublicGetSpotMarket(params)
             #
             #     {
             #         "code": 0,
             #         "data": [
             #             {
             #                 "base_ccy": "BTC",
             #                 "base_ccy_precision": 8,
@@ -1433,39 +1434,39 @@
             self.safe_number(ohlcv, 'open'),
             self.safe_number(ohlcv, 'high'),
             self.safe_number(ohlcv, 'low'),
             self.safe_number(ohlcv, 'close'),
             self.safe_number(ohlcv, 'value'),
         ]
 
-    def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
+    async def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
         """
         fetches historical candlestick data containing the open, high, low, and close price, and the volume of a market
         :see: https://docs.coinex.com/api/v2/spot/market/http/list-market-kline
         :see: https://docs.coinex.com/api/v2/futures/market/http/list-market-kline
         :param str symbol: unified symbol of the market to fetch OHLCV data for
         :param str timeframe: the length of time each candle represents
         :param int [since]: timestamp in ms of the earliest candle to fetch
         :param int [limit]: the maximum amount of candles to fetch
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns int[][]: A list of candles ordered, open, high, low, close, volume
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'period': self.safe_string(self.timeframes, timeframe, timeframe),
         }
         if limit is not None:
             request['limit'] = limit
         response = None
         if market['swap']:
-            response = self.v2PublicGetFuturesKline(self.extend(request, params))
+            response = await self.v2PublicGetFuturesKline(self.extend(request, params))
         else:
-            response = self.v2PublicGetSpotKline(self.extend(request, params))
+            response = await self.v2PublicGetSpotKline(self.extend(request, params))
         #
         # Spot and Swap
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -1481,17 +1482,17 @@
         #         ],
         #         "message": "OK"
         #     }
         #
         data = self.safe_list(response, 'data', [])
         return self.parse_ohlcvs(data, market, timeframe, since, limit)
 
-    def fetch_margin_balance(self, params={}):
-        self.load_markets()
-        response = self.v2PrivateGetAssetsMarginBalance(params)
+    async def fetch_margin_balance(self, params={}):
+        await self.load_markets()
+        response = await self.v2PrivateGetAssetsMarginBalance(params)
         #
         #     {
         #         "data": [
         #             {
         #                 "margin_account": "BTCUSDT",
         #                 "base_ccy": "BTC",
         #                 "quote_ccy": "USDT",
@@ -1534,17 +1535,17 @@
             baseAccount['used'] = self.safe_string(used, 'base_ccy')
             baseDebt = self.safe_string(loan, 'base_ccy')
             baseInterest = self.safe_string(interest, 'base_ccy')
             baseAccount['debt'] = Precise.string_add(baseDebt, baseInterest)
             result[baseCurrencyCode] = baseAccount
         return self.safe_balance(result)
 
-    def fetch_spot_balance(self, params={}):
-        self.load_markets()
-        response = self.v2PrivateGetAssetsSpotBalance(params)
+    async def fetch_spot_balance(self, params={}):
+        await self.load_markets()
+        response = await self.v2PrivateGetAssetsSpotBalance(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "available": "0.00000046",
         #                 "ccy": "USDT",
@@ -1562,17 +1563,17 @@
             code = self.safe_currency_code(currencyId)
             account = self.account()
             account['free'] = self.safe_string(entry, 'available')
             account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
-    def fetch_swap_balance(self, params={}):
-        self.load_markets()
-        response = self.v2PrivateGetAssetsFuturesBalance(params)
+    async def fetch_swap_balance(self, params={}):
+        await self.load_markets()
+        response = await self.v2PrivateGetAssetsFuturesBalance(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "available": "0.00000046",
         #                 "ccy": "USDT",
@@ -1593,17 +1594,17 @@
             code = self.safe_currency_code(currencyId)
             account = self.account()
             account['free'] = self.safe_string(entry, 'available')
             account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
-    def fetch_financial_balance(self, params={}):
-        self.load_markets()
-        response = self.v2PrivateGetAssetsFinancialBalance(params)
+    async def fetch_financial_balance(self, params={}):
+        await self.load_markets()
+        response = await self.v2PrivateGetAssetsFinancialBalance(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "available": "0.00000046",
         #                 "ccy": "USDT",
@@ -1621,15 +1622,15 @@
             code = self.safe_currency_code(currencyId)
             account = self.account()
             account['free'] = self.safe_string(entry, 'available')
             account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
-    def fetch_balance(self, params={}) -> Balances:
+    async def fetch_balance(self, params={}) -> Balances:
         """
         query for balance and get the amount of funds available for trading or funds locked in orders
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-spot-balance         # spot
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-futures-balance      # swap
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-marigin-balance      # margin
         :see: https://docs.coinex.com/api/v2/assets/balance/http/get-financial-balance    # financial
         :param dict [params]: extra parameters specific to the exchange API endpoint
@@ -1639,21 +1640,21 @@
         marketType = None
         marketType, params = self.handle_market_type_and_params('fetchBalance', None, params)
         marginMode = None
         marginMode, params = self.handle_margin_mode_and_params('fetchBalance', params)
         marketType = 'margin' if (marginMode is not None) else marketType
         params = self.omit(params, 'margin')
         if marketType == 'margin':
-            return self.fetch_margin_balance(params)
+            return await self.fetch_margin_balance(params)
         elif marketType == 'swap':
-            return self.fetch_swap_balance(params)
+            return await self.fetch_swap_balance(params)
         elif marketType == 'financial':
-            return self.fetch_financial_balance(params)
+            return await self.fetch_financial_balance(params)
         else:
-            return self.fetch_spot_balance(params)
+            return await self.fetch_spot_balance(params)
 
     def parse_order_status(self, status):
         statuses = {
             'rejected': 'rejected',
             'open': 'open',
             'not_deal': 'open',
             'part_deal': 'open',
@@ -1684,15 +1685,15 @@
         #         "price": "170.00000000",
         #         "status": "done",
         #         "taker_fee_rate": "0.0005",
         #         "type": "sell",
         #         "client_id": "",
         #     }
         #
-        # Spot and Margin createOrder, createOrders, cancelOrder, cancelOrders, fetchOrder
+        # Spot and Margin cancelOrder, cancelOrders, fetchOrder
         #
         #      {
         #          "amount":"1.5",
         #          "asset_fee":"0",
         #          "avg_price":"0.14208538",
         #          "client_id":"",
         #          "create_time":1650993819,
@@ -1712,15 +1713,15 @@
         #          "status":"done",
         #          "stock_fee":"0",
         #          "taker_fee_rate":"0.002",
         #          "type":"buy"
         #          "client_id": "",
         #      }
         #
-        # Swap createOrder, cancelOrder, fetchOrder
+        # Swap cancelOrder, fetchOrder
         #
         #     {
         #         "amount": "0.0005",
         #         "client_id": "",
         #         "create_time": 1651004578.618224,
         #         "deal_asset_fee": "0.00000000000000000000",
         #         "deal_fee": "0.00000000000000000000",
@@ -1749,18 +1750,14 @@
         #         "taker_fee": "0.00050",
         #         "target": 0,
         #         "type": 1,
         #         "update_time": 1651004578.618224,
         #         "user_id": 3620173
         #     }
         #
-        # Stop order createOrder
-        #
-        #     {"status":"success"}
-        #
         # Swap Stop cancelOrder, fetchOrder
         #
         #     {
         #         "amount": "0.0005",
         #         "client_id": "",
         #         "create_time": 1651034023.008771,
         #         "effect_type": 1,
@@ -1925,166 +1922,257 @@
         #         "taker_fee": "0.00050",
         #         "target": 0,
         #         "type": 1,
         #         "update_time": 1701233721.718884,
         #         "user_id": 3620173
         #     }
         #
+        # Spot and Margin createOrder, createOrders v2
+        #
+        #     {
+        #         "amount": "0.0001",
+        #         "base_fee": "0",
+        #         "ccy": "BTC",
+        #         "client_id": "x-167673045-a0a3c6461459a801",
+        #         "created_at": 1714114386250,
+        #         "discount_fee": "0",
+        #         "filled_amount": "0",
+        #         "filled_value": "0",
+        #         "last_fill_amount": "0",
+        #         "last_fill_price": "0",
+        #         "maker_fee_rate": "0.002",
+        #         "market": "BTCUSDT",
+        #         "market_type": "SPOT",
+        #         "order_id": 117178743547,
+        #         "price": "61000",
+        #         "quote_fee": "0",
+        #         "side": "buy",
+        #         "taker_fee_rate": "0.002",
+        #         "type": "limit",
+        #         "unfilled_amount": "0.0001",
+        #         "updated_at": 1714114386250
+        #     }
+        #
+        # Spot, Margin and Swap trigger createOrder, createOrders v2
+        #
+        #     {
+        #         "stop_id": 117180138153
+        #     }
+        #
+        # Swap createOrder, createOrders v2
+        #
+        #     {
+        #         "amount": "0.0001",
+        #         "client_id": "x-167673045-1471b81d747080a0",
+        #         "created_at": 1714116769986,
+        #         "fee": "0",
+        #         "fee_ccy": "USDT",
+        #         "filled_amount": "0",
+        #         "filled_value": "0",
+        #         "last_filled_amount": "0",
+        #         "last_filled_price": "0",
+        #         "maker_fee_rate": "0.0003",
+        #         "market": "BTCUSDT",
+        #         "market_type": "FUTURES",
+        #         "order_id": 136913377780,
+        #         "price": "61000.42",
+        #         "realized_pnl": "0",
+        #         "side": "buy",
+        #         "taker_fee_rate": "0.0005",
+        #         "type": "limit",
+        #         "unfilled_amount": "0.0001",
+        #         "updated_at": 1714116769986
+        #     }
+        #
+        # Swap stopLossPrice and takeProfitPrice createOrder v2
+        #
+        #     {
+        #         "adl_level": 1,
+        #         "ath_margin_size": "2.14586666",
+        #         "ath_position_amount": "0.0001",
+        #         "avg_entry_price": "64376",
+        #         "bkr_price": "0",
+        #         "close_avbl": "0.0001",
+        #         "cml_position_value": "6.4376",
+        #         "created_at": 1714119054558,
+        #         "leverage": "3",
+        #         "liq_price": "0",
+        #         "maintenance_margin_rate": "0.005",
+        #         "maintenance_margin_value": "0.03218632",
+        #         "margin_avbl": "2.14586666",
+        #         "margin_mode": "cross",
+        #         "market": "BTCUSDT",
+        #         "market_type": "FUTURES",
+        #         "max_position_value": "6.4376",
+        #         "open_interest": "0.0001",
+        #         "position_id": 303884204,
+        #         "position_margin_rate": "3.10624785634397912265",
+        #         "realized_pnl": "-0.0032188",
+        #         "settle_price": "64376",
+        #         "settle_value": "6.4376",
+        #         "side": "long",
+        #         "stop_loss_price": "62000",
+        #         "stop_loss_type": "latest_price",
+        #         "take_profit_price": "0",
+        #         "take_profit_type": "",
+        #         "unrealized_pnl": "0",
+        #         "updated_at": 1714119054559
+        #     }
+        #
         rawStatus = self.safe_string(order, 'status')
         timestamp = self.safe_timestamp(order, 'create_time')
+        if timestamp is None:
+            timestamp = self.safe_integer(order, 'created_at')
+        update = self.safe_timestamp(order, 'update_time')
+        if update is None:
+            update = self.safe_integer(order, 'updated_at')
         marketId = self.safe_string(order, 'market')
         defaultType = self.safe_string(self.options, 'defaultType')
         orderType = 'swap' if ('source' in order) else defaultType
         market = self.safe_market(marketId, market, None, orderType)
-        feeCurrencyId = self.safe_string(order, 'fee_asset')
+        feeCurrencyId = self.safe_string_2(order, 'fee_asset', 'fee_ccy')
         feeCurrency = self.safe_currency_code(feeCurrencyId)
         if feeCurrency is None:
             feeCurrency = market['quote']
-        rawSide = self.safe_integer(order, 'side')
+        rawIntegerSide = self.safe_integer(order, 'side')
+        rawStringSide = self.safe_string(order, 'side')
         side: Str = None
-        if rawSide == 1:
+        if rawIntegerSide == 1:
             side = 'sell'
-        elif rawSide == 2:
+        elif rawIntegerSide == 2:
             side = 'buy'
+        elif (rawStringSide == 'buy') or (rawStringSide == 'sell'):
+            side = rawStringSide
         else:
             side = self.safe_string(order, 'type')
         rawType = self.safe_string(order, 'order_type')
         type: Str = None
         if rawType is None:
             typeInteger = self.safe_integer(order, 'type')
+            typeString = self.safe_string(order, 'type')
             if typeInteger == 1:
                 type = 'limit'
             elif typeInteger == 2:
                 type = 'market'
+            elif (typeString == 'limit') or (typeString == 'market'):
+                type = typeString
+            elif typeString == 'maker_only':
+                type = 'limit'
         else:
             type = rawType
         clientOrderId = self.safe_string(order, 'client_id')
         if clientOrderId == '':
             clientOrderId = None
         return self.safe_order({
-            'id': self.safe_string_2(order, 'id', 'order_id'),
+            'id': self.safe_string_n(order, ['id', 'order_id', 'stop_id']),
             'clientOrderId': clientOrderId,
             'datetime': self.iso8601(timestamp),
             'timestamp': timestamp,
-            'lastTradeTimestamp': self.safe_timestamp(order, 'update_time'),
+            'lastTradeTimestamp': update,
             'status': self.parse_order_status(rawStatus),
             'symbol': market['symbol'],
             'type': type,
             'timeInForce': None,
             'postOnly': None,
             'reduceOnly': None,
             'side': side,
             'price': self.safe_string(order, 'price'),
             'stopPrice': self.safe_string(order, 'stop_price'),
             'triggerPrice': self.safe_string(order, 'stop_price'),
             'takeProfitPrice': self.safe_number(order, 'take_profit_price'),
             'stopLossPrice': self.safe_number(order, 'stop_loss_price'),
-            'cost': self.safe_string(order, 'deal_money'),
-            'average': self.safe_string(order, 'avg_price'),
+            'cost': self.safe_string_2(order, 'deal_money', 'filled_value'),
+            'average': self.safe_string_2(order, 'avg_price', 'avg_entry_price'),
             'amount': self.safe_string(order, 'amount'),
-            'filled': self.safe_string(order, 'deal_amount'),
-            'remaining': self.safe_string(order, 'left'),
+            'filled': self.safe_string_2(order, 'deal_amount', 'filled_amount'),
+            'remaining': self.safe_string_2(order, 'left', 'unfilled_amount'),
             'trades': None,
             'fee': {
                 'currency': feeCurrency,
-                'cost': self.safe_string(order, 'deal_fee'),
+                'cost': self.safe_string_n(order, ['deal_fee', 'quote_fee', 'fee']),
             },
             'info': order,
         }, market)
 
-    def create_market_buy_order_with_cost(self, symbol: str, cost: float, params={}):
+    async def create_market_buy_order_with_cost(self, symbol: str, cost: float, params={}):
         """
         create a market buy order by providing the symbol and cost
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade003_market_order
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-order
         :param str symbol: unified symbol of the market to create an order in
         :param float cost: how much you want to trade in units of the quote currency
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if not market['spot']:
             raise NotSupported(self.id + ' createMarketBuyOrderWithCost() supports spot orders only')
         params['createMarketBuyOrderRequiresPrice'] = False
-        return self.create_order(symbol, 'market', 'buy', cost, None, params)
+        return await self.create_order(symbol, 'market', 'buy', cost, None, params)
 
     def create_order_request(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
         market = self.market(symbol)
         swap = market['swap']
         clientOrderId = self.safe_string_2(params, 'client_id', 'clientOrderId')
-        stopPrice = self.safe_value_2(params, 'stopPrice', 'triggerPrice')
-        stopLossPrice = self.safe_value(params, 'stopLossPrice')
-        takeProfitPrice = self.safe_value(params, 'takeProfitPrice')
+        stopPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
+        stopLossPrice = self.safe_string(params, 'stopLossPrice')
+        takeProfitPrice = self.safe_string(params, 'takeProfitPrice')
         option = self.safe_string(params, 'option')
         isMarketOrder = type == 'market'
-        postOnly = self.is_post_only(isMarketOrder, option == 'MAKER_ONLY', params)
-        positionId = self.safe_integer_2(params, 'position_id', 'positionId')  # Required for closing swap positions
-        timeInForceRaw = self.safe_string(params, 'timeInForce')  # Spot: IOC, FOK, PO, GTC, ... NORMAL(default), MAKER_ONLY
-        reduceOnly = self.safe_value(params, 'reduceOnly')
+        postOnly = self.is_post_only(isMarketOrder, option == 'maker_only', params)
+        timeInForceRaw = self.safe_string_upper(params, 'timeInForce')
+        reduceOnly = self.safe_bool(params, 'reduceOnly')
         if reduceOnly:
             if not market['swap']:
                 raise InvalidOrder(self.id + ' createOrder() does not support reduceOnly for ' + market['type'] + ' orders, reduceOnly orders are supported for swap markets only')
-            if positionId is None:
-                raise ArgumentsRequired(self.id + ' createOrder() requires a position_id/positionId parameter for reduceOnly orders')
         request = {
             'market': market['id'],
         }
         if clientOrderId is None:
             defaultId = 'x-167673045'
             brokerId = self.safe_string(self.options, 'brokerId', defaultId)
             request['client_id'] = brokerId + '-' + self.uuid16()
         else:
             request['client_id'] = clientOrderId
+        if (stopLossPrice is None) and (takeProfitPrice is None):
+            if not reduceOnly:
+                request['side'] = side
+            requestType = type
+            if postOnly:
+                requestType = 'maker_only'
+            elif timeInForceRaw is not None:
+                if timeInForceRaw == 'IOC':
+                    requestType = 'ioc'
+                elif timeInForceRaw == 'FOK':
+                    requestType = 'fok'
+            if not isMarketOrder:
+                request['price'] = self.price_to_precision(symbol, price)
+            request['type'] = requestType
         if swap:
+            request['market_type'] = 'FUTURES'
             if stopLossPrice or takeProfitPrice:
-                request['stop_type'] = self.safe_integer(params, 'stop_type', 1)  # 1: triggered by the latest transaction, 2: mark price, 3: index price
-                if positionId is None:
-                    raise ArgumentsRequired(self.id + ' createOrder() requires a position_id parameter for stop loss and take profit orders')
-                request['position_id'] = positionId
                 if stopLossPrice:
                     request['stop_loss_price'] = self.price_to_precision(symbol, stopLossPrice)
+                    request['stop_loss_type'] = self.safe_string(params, 'stop_type', 'latest_price')
                 elif takeProfitPrice:
                     request['take_profit_price'] = self.price_to_precision(symbol, takeProfitPrice)
+                    request['take_profit_type'] = self.safe_string(params, 'stop_type', 'latest_price')
             else:
-                requestSide = 2 if (side == 'buy') else 1
+                request['amount'] = self.amount_to_precision(symbol, amount)
                 if stopPrice is not None:
-                    request['stop_price'] = self.price_to_precision(symbol, stopPrice)
-                    request['stop_type'] = self.safe_integer(params, 'stop_type', 1)  # 1: triggered by the latest transaction, 2: mark price, 3: index price
-                    request['amount'] = self.amount_to_precision(symbol, amount)
-                    request['side'] = requestSide
-                    if type == 'limit':
-                        request['price'] = self.price_to_precision(symbol, price)
-                    request['amount'] = self.amount_to_precision(symbol, amount)
-                timeInForce = None
-                if (type != 'market') or (stopPrice is not None):
-                    if postOnly:
-                        request['option'] = 1
-                    elif timeInForceRaw is not None:
-                        if timeInForceRaw == 'IOC':
-                            timeInForce = 2
-                        elif timeInForceRaw == 'FOK':
-                            timeInForce = 3
-                        else:
-                            timeInForce = 1
-                        request['effect_type'] = timeInForce  # exchange takes 'IOC' and 'FOK'
-                if type == 'limit' and stopPrice is None:
-                    if reduceOnly:
-                        request['position_id'] = positionId
-                    else:
-                        request['side'] = requestSide
-                    request['price'] = self.price_to_precision(symbol, price)
-                    request['amount'] = self.amount_to_precision(symbol, amount)
-                elif type == 'market' and stopPrice is None:
-                    if reduceOnly:
-                        request['position_id'] = positionId
-                    else:
-                        request['side'] = requestSide
-                        request['amount'] = self.amount_to_precision(symbol, amount)
+                    request['trigger_price'] = self.price_to_precision(symbol, stopPrice)
+                    request['trigger_price_type'] = self.safe_string(params, 'stop_type', 'latest_price')
         else:
-            request['type'] = side
+            marginMode = None
+            marginMode, params = self.handle_margin_mode_and_params('createOrder', params)
+            if marginMode is not None:
+                request['market_type'] = 'MARGIN'
+            else:
+                request['market_type'] = 'SPOT'
             if (type == 'market') and (side == 'buy'):
                 createMarketBuyOrderRequiresPrice = True
                 createMarketBuyOrderRequiresPrice, params = self.handle_option_and_params(params, 'createOrder', 'createMarketBuyOrderRequiresPrice', True)
                 cost = self.safe_number(params, 'cost')
                 params = self.omit(params, 'cost')
                 if createMarketBuyOrderRequiresPrice:
                     if (price is None) and (cost is None):
@@ -2095,203 +2183,272 @@
                         quoteAmount = self.parse_to_numeric(Precise.string_mul(amountString, priceString))
                         costRequest = cost if (cost is not None) else quoteAmount
                         request['amount'] = self.cost_to_precision(symbol, costRequest)
                 else:
                     request['amount'] = self.cost_to_precision(symbol, amount)
             else:
                 request['amount'] = self.amount_to_precision(symbol, amount)
-            if (type == 'limit') or (type == 'ioc'):
-                request['price'] = self.price_to_precision(symbol, price)
             if stopPrice is not None:
-                request['stop_price'] = self.price_to_precision(symbol, stopPrice)
-            if (type != 'market') or (stopPrice is not None):
-                # following options cannot be applied to vanilla market orders(but can be applied to stop-market orders)
-                if (timeInForceRaw is not None) or postOnly:
-                    if (postOnly or (timeInForceRaw != 'IOC')) and ((type == 'limit') and (stopPrice is not None)):
-                        raise InvalidOrder(self.id + ' createOrder() only supports the IOC option for stop-limit orders')
-                    if postOnly:
-                        request['option'] = 'MAKER_ONLY'
-                    else:
-                        if timeInForceRaw is not None:
-                            request['option'] = timeInForceRaw  # exchange takes 'IOC' and 'FOK'
-        accountId = self.safe_integer(params, 'account_id')
-        marginMode = None
-        marginMode, params = self.handle_margin_mode_and_params('createOrder', params)
-        if marginMode is not None:
-            if accountId is None:
-                raise BadRequest(self.id + ' createOrder() requires an account_id parameter for margin orders')
-            request['account_id'] = accountId
-        params = self.omit(params, ['reduceOnly', 'positionId', 'timeInForce', 'postOnly', 'stopPrice', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice'])
+                request['trigger_price'] = self.price_to_precision(symbol, stopPrice)
+        params = self.omit(params, ['reduceOnly', 'timeInForce', 'postOnly', 'stopPrice', 'triggerPrice', 'stopLossPrice', 'takeProfitPrice'])
         return self.extend(request, params)
 
-    def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
+    async def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}):
         """
         create a trade order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade001_limit_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade003_market_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade004_IOC_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade005_stop_limit_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade006_stop_market_order
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http017_put_limit
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http018_put_market
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http019_put_limit_stop
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http020_put_market_stop
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http031_market_close
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http030_limit_close
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-order
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-stop-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-stop-order
+        :see: https://docs.coinex.com/api/v2/futures/position/http/close-position
+        :see: https://docs.coinex.com/api/v2/futures/position/http/set-position-stop-loss
+        :see: https://docs.coinex.com/api/v2/futures/position/http/set-position-take-profit
         :param str symbol: unified symbol of the market to create an order in
         :param str type: 'market' or 'limit'
         :param str side: 'buy' or 'sell'
         :param float amount: how much you want to trade in units of the base currency
         :param float [price]: the price at which the order is to be fullfilled, in units of the quote currency, ignored in market orders
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param float [params.triggerPrice]: price to trigger stop orders
         :param float [params.stopLossPrice]: price to trigger stop loss orders
         :param float [params.takeProfitPrice]: price to trigger take profit orders
         :param str [params.timeInForce]: 'GTC', 'IOC', 'FOK', 'PO'
         :param boolean [params.postOnly]: set to True if you wish to make a post only order
         :param boolean [params.reduceOnly]: *contract only* indicates if self order is to reduce the size of a position
-        :param int [params.position_id]: *required for reduce only orders* the position id to reduce
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
-        reduceOnly = self.safe_value(params, 'reduceOnly')
-        triggerPrice = self.safe_number_2(params, 'stopPrice', 'triggerPrice')
-        stopLossTriggerPrice = self.safe_number(params, 'stopLossPrice')
-        takeProfitTriggerPrice = self.safe_number(params, 'takeProfitPrice')
+        reduceOnly = self.safe_bool(params, 'reduceOnly')
+        triggerPrice = self.safe_string_2(params, 'stopPrice', 'triggerPrice')
+        stopLossTriggerPrice = self.safe_string(params, 'stopLossPrice')
+        takeProfitTriggerPrice = self.safe_string(params, 'takeProfitPrice')
         isTriggerOrder = triggerPrice is not None
         isStopLossTriggerOrder = stopLossTriggerPrice is not None
         isTakeProfitTriggerOrder = takeProfitTriggerPrice is not None
         isStopLossOrTakeProfitTrigger = isStopLossTriggerOrder or isTakeProfitTriggerOrder
         request = self.create_order_request(symbol, type, side, amount, price, params)
         response = None
         if market['spot']:
             if isTriggerOrder:
-                if type == 'limit':
-                    response = self.v1PrivatePostOrderStopLimit(request)
-                else:
-                    response = self.v1PrivatePostOrderStopMarket(request)
+                response = await self.v2PrivatePostSpotStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": {
+                #             "stop_id": 117180138153
+                #         },
+                #         "message": "OK"
+                #     }
+                #
             else:
-                if type == 'limit':
-                    response = self.v1PrivatePostOrderLimit(request)
-                else:
-                    response = self.v1PrivatePostOrderMarket(request)
+                response = await self.v2PrivatePostSpotOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": {
+                #             "amount": "0.0001",
+                #             "base_fee": "0",
+                #             "ccy": "BTC",
+                #             "client_id": "x-167673045-a0a3c6461459a801",
+                #             "created_at": 1714114386250,
+                #             "discount_fee": "0",
+                #             "filled_amount": "0",
+                #             "filled_value": "0",
+                #             "last_fill_amount": "0",
+                #             "last_fill_price": "0",
+                #             "maker_fee_rate": "0.002",
+                #             "market": "BTCUSDT",
+                #             "market_type": "SPOT",
+                #             "order_id": 117178743547,
+                #             "price": "61000",
+                #             "quote_fee": "0",
+                #             "side": "buy",
+                #             "taker_fee_rate": "0.002",
+                #             "type": "limit",
+                #             "unfilled_amount": "0.0001",
+                #             "updated_at": 1714114386250
+                #         },
+                #         "message": "OK"
+                #     }
+                #
         else:
             if isTriggerOrder:
-                if type == 'limit':
-                    response = self.v1PerpetualPrivatePostOrderPutStopLimit(request)
-                else:
-                    response = self.v1PerpetualPrivatePostOrderPutStopMarket(request)
+                response = await self.v2PrivatePostFuturesStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": {
+                #             "stop_id": 136915460994
+                #         },
+                #         "message": "OK"
+                #     }
+                #
             elif isStopLossOrTakeProfitTrigger:
                 if isStopLossTriggerOrder:
-                    response = self.v1PerpetualPrivatePostPositionStopLoss(request)
+                    response = await self.v2PrivatePostFuturesSetPositionStopLoss(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "adl_level": 1,
+                    #             "ath_margin_size": "2.14586666",
+                    #             "ath_position_amount": "0.0001",
+                    #             "avg_entry_price": "64376",
+                    #             "bkr_price": "0",
+                    #             "close_avbl": "0.0001",
+                    #             "cml_position_value": "6.4376",
+                    #             "created_at": 1714119054558,
+                    #             "leverage": "3",
+                    #             "liq_price": "0",
+                    #             "maintenance_margin_rate": "0.005",
+                    #             "maintenance_margin_value": "0.03218632",
+                    #             "margin_avbl": "2.14586666",
+                    #             "margin_mode": "cross",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "max_position_value": "6.4376",
+                    #             "open_interest": "0.0001",
+                    #             "position_id": 303884204,
+                    #             "position_margin_rate": "3.10624785634397912265",
+                    #             "realized_pnl": "-0.0032188",
+                    #             "settle_price": "64376",
+                    #             "settle_value": "6.4376",
+                    #             "side": "long",
+                    #             "stop_loss_price": "62000",
+                    #             "stop_loss_type": "latest_price",
+                    #             "take_profit_price": "0",
+                    #             "take_profit_type": "",
+                    #             "unrealized_pnl": "0",
+                    #             "updated_at": 1714119054559
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
                 elif isTakeProfitTriggerOrder:
-                    response = self.v1PerpetualPrivatePostPositionTakeProfit(request)
+                    response = await self.v2PrivatePostFuturesSetPositionTakeProfit(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "adl_level": 1,
+                    #             "ath_margin_size": "2.14586666",
+                    #             "ath_position_amount": "0.0001",
+                    #             "avg_entry_price": "64376",
+                    #             "bkr_price": "0",
+                    #             "close_avbl": "0.0001",
+                    #             "cml_position_value": "6.4376",
+                    #             "created_at": 1714119054558,
+                    #             "leverage": "3",
+                    #             "liq_price": "0",
+                    #             "maintenance_margin_rate": "0.005",
+                    #             "maintenance_margin_value": "0.03218632",
+                    #             "margin_avbl": "2.14586666",
+                    #             "margin_mode": "cross",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "max_position_value": "6.4376",
+                    #             "open_interest": "0.0001",
+                    #             "position_id": 303884204,
+                    #             "position_margin_rate": "3.10624785634397912265",
+                    #             "realized_pnl": "-0.0032188",
+                    #             "settle_price": "64376",
+                    #             "settle_value": "6.4376",
+                    #             "side": "long",
+                    #             "stop_loss_price": "62000",
+                    #             "stop_loss_type": "latest_price",
+                    #             "take_profit_price": "70000",
+                    #             "take_profit_type": "latest_price",
+                    #             "unrealized_pnl": "0",
+                    #             "updated_at": 1714119054559
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
             else:
                 if reduceOnly:
-                    if type == 'limit':
-                        response = self.v1PerpetualPrivatePostOrderCloseLimit(request)
-                    else:
-                        response = self.v1PerpetualPrivatePostOrderCloseMarket(request)
+                    response = await self.v2PrivatePostFuturesClosePosition(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "amount": "0.0001",
+                    #             "client_id": "x-167673045-4f264600c432ac06",
+                    #             "created_at": 1714119323764,
+                    #             "fee": "0.003221",
+                    #             "fee_ccy": "USDT",
+                    #             "filled_amount": "0.0001",
+                    #             "filled_value": "6.442017",
+                    #             "last_filled_amount": "0.0001",
+                    #             "last_filled_price": "64420.17",
+                    #             "maker_fee_rate": "0",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "order_id": 136915813578,
+                    #             "price": "0",
+                    #             "realized_pnl": "0.004417",
+                    #             "side": "sell",
+                    #             "taker_fee_rate": "0.0005",
+                    #             "type": "market",
+                    #             "unfilled_amount": "0",
+                    #             "updated_at": 1714119323764
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
                 else:
-                    if type == 'limit':
-                        response = self.v1PerpetualPrivatePostOrderPutLimit(request)
-                    else:
-                        response = self.v1PerpetualPrivatePostOrderPutMarket(request)
-        #
-        # Spot and Margin
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "amount": "0.0005",
-        #             "asset_fee": "0",
-        #             "avg_price": "0.00",
-        #             "client_id": "",
-        #             "create_time": 1650951627,
-        #             "deal_amount": "0",
-        #             "deal_fee": "0",
-        #             "deal_money": "0",
-        #             "fee_asset": null,
-        #             "fee_discount": "1",
-        #             "finished_time": null,
-        #             "id": 74510932594,
-        #             "left": "0.0005",
-        #             "maker_fee_rate": "0.002",
-        #             "market": "BTCUSDT",
-        #             "money_fee": "0",
-        #             "order_type": "limit",
-        #             "price": "30000",
-        #             "status": "not_deal",
-        #             "stock_fee": "0",
-        #             "taker_fee_rate": "0.002",
-        #             "type": "buy"
-        #         },
-        #         "message": "Success"
-        #     }
-        #
-        # Swap
-        #
-        #     {
-        #         "code": 0,
-        #         "data": {
-        #             "amount": "0.0005",
-        #             "client_id": "",
-        #             "create_time": 1651004578.618224,
-        #             "deal_asset_fee": "0.00000000000000000000",
-        #             "deal_fee": "0.00000000000000000000",
-        #             "deal_profit": "0.00000000000000000000",
-        #             "deal_stock": "0.00000000000000000000",
-        #             "effect_type": 1,
-        #             "fee_asset": "",
-        #             "fee_discount": "0.00000000000000000000",
-        #             "last_deal_amount": "0.00000000000000000000",
-        #             "last_deal_id": 0,
-        #             "last_deal_price": "0.00000000000000000000",
-        #             "last_deal_role": 0,
-        #             "last_deal_time": 0,
-        #             "last_deal_type": 0,
-        #             "left": "0.0005",
-        #             "leverage": "3",
-        #             "maker_fee": "0.00030",
-        #             "market": "BTCUSDT",
-        #             "order_id": 18221659097,
-        #             "position_id": 0,
-        #             "position_type": 1,
-        #             "price": "30000.00",
-        #             "side": 2,
-        #             "source": "api.v1",
-        #             "stop_id": 0,
-        #             "taker_fee": "0.00050",
-        #             "target": 0,
-        #             "type": 1,
-        #             "update_time": 1651004578.618224,
-        #             "user_id": 3620173
-        #         },
-        #         "message": "OK"
-        #     }
-        #
-        # Stop Order
-        #
-        #     {"code":0,"data":{"status":"success"},"message":"OK"}
-        #
+                    response = await self.v2PrivatePostFuturesOrder(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": {
+                    #             "amount": "0.0001",
+                    #             "client_id": "x-167673045-1471b81d747080a0",
+                    #             "created_at": 1714116769986,
+                    #             "fee": "0",
+                    #             "fee_ccy": "USDT",
+                    #             "filled_amount": "0",
+                    #             "filled_value": "0",
+                    #             "last_filled_amount": "0",
+                    #             "last_filled_price": "0",
+                    #             "maker_fee_rate": "0.0003",
+                    #             "market": "BTCUSDT",
+                    #             "market_type": "FUTURES",
+                    #             "order_id": 136913377780,
+                    #             "price": "61000.42",
+                    #             "realized_pnl": "0",
+                    #             "side": "buy",
+                    #             "taker_fee_rate": "0.0005",
+                    #             "type": "limit",
+                    #             "unfilled_amount": "0.0001",
+                    #             "updated_at": 1714116769986
+                    #         },
+                    #         "message": "OK"
+                    #     }
+                    #
         data = self.safe_dict(response, 'data', {})
         return self.parse_order(data, market)
 
-    def create_orders(self, orders: List[OrderRequest], params={}) -> List[Order]:
+    async def create_orders(self, orders: List[OrderRequest], params={}) -> List[Order]:
         """
         create a list of trade orders(all orders should be of the same symbol)
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade002_batch_limit_orders
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-multi-order
+        :see: https://docs.coinex.com/api/v2/spot/order/http/put-multi-stop-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-multi-order
+        :see: https://docs.coinex.com/api/v2/futures/order/http/put-multi-stop-order
         :param Array orders: list of orders to create, each object should contain the parameters required by createOrder, namely symbol, type, side, amount, price and params
         :param dict [params]: extra parameters specific to the api endpoint
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         ordersRequests = []
         symbol = None
+        reduceOnly = False
+        isTriggerOrder = False
+        isStopLossOrTakeProfitTrigger = False
         for i in range(0, len(orders)):
             rawOrder = orders[i]
             marketId = self.safe_string(rawOrder, 'symbol')
             if symbol is None:
                 symbol = marketId
             else:
                 if symbol != marketId:
@@ -2299,103 +2456,192 @@
             type = self.safe_string(rawOrder, 'type')
             side = self.safe_string(rawOrder, 'side')
             amount = self.safe_value(rawOrder, 'amount')
             price = self.safe_value(rawOrder, 'price')
             orderParams = self.safe_value(rawOrder, 'params', {})
             if type != 'limit':
                 raise NotSupported(self.id + ' createOrders() does not support ' + type + ' orders, only limit orders are accepted')
+            reduceOnly = self.safe_value(orderParams, 'reduceOnly')
+            triggerPrice = self.safe_number_2(orderParams, 'stopPrice', 'triggerPrice')
+            stopLossTriggerPrice = self.safe_number(orderParams, 'stopLossPrice')
+            takeProfitTriggerPrice = self.safe_number(orderParams, 'takeProfitPrice')
+            isTriggerOrder = triggerPrice is not None
+            isStopLossTriggerOrder = stopLossTriggerPrice is not None
+            isTakeProfitTriggerOrder = takeProfitTriggerPrice is not None
+            isStopLossOrTakeProfitTrigger = isStopLossTriggerOrder or isTakeProfitTriggerOrder
             orderRequest = self.create_order_request(marketId, type, side, amount, price, orderParams)
             ordersRequests.append(orderRequest)
         market = self.market(symbol)
-        if not market['spot']:
-            raise NotSupported(self.id + ' createOrders() does not support ' + market['type'] + ' orders, only spot orders are accepted')
         request = {
             'market': market['id'],
-            'batch_orders': self.json(ordersRequests),
+            'orders': ordersRequests,
         }
-        response = self.v1PrivatePostOrderLimitBatch(request)
-        #
-        #     {
-        #         "code": 0,
-        #         "data": [
-        #             {
-        #                 "code": 0,
-        #                 "data": {
-        #                     "amount": "0.0005",
-        #                     "asset_fee": "0",
-        #                     "avg_price": "0.00",
-        #                     "client_id": "x-167673045-d34bfb41242d8fd1",
-        #                     "create_time": 1701229157,
-        #                     "deal_amount": "0",
-        #                     "deal_fee": "0",
-        #                     "deal_money": "0",
-        #                     "fee_asset": null,
-        #                     "fee_discount": "1",
-        #                     "finished_time": null,
-        #                     "id": 107745856676,
-        #                     "left": "0.0005",
-        #                     "maker_fee_rate": "0.002",
-        #                     "market": "BTCUSDT",
-        #                     "money_fee": "0",
-        #                     "order_type": "limit",
-        #                     "price": "23000",
-        #                     "source_id": "",
-        #                     "status": "not_deal",
-        #                     "stock_fee": "0",
-        #                     "taker_fee_rate": "0.002",
-        #                     "type": "buy"
-        #                 },
-        #                 "message": "OK"
-        #             },
-        #         ],
-        #         "message": "Success"
-        #     }
-        #
-        data = self.safe_value(response, 'data', [])
+        response = None
+        if market['spot']:
+            if isTriggerOrder:
+                response = await self.v2PrivatePostSpotBatchStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": [
+                #             {
+                #                 "code": 0,
+                #                 "data": {
+                #                     "stop_id": 117186257510
+                #                 },
+                #                 "message": "OK"
+                #             },
+                #         ],
+                #         "message": "OK"
+                #     }
+                #
+            else:
+                response = await self.v2PrivatePostSpotBatchOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": [
+                #             {
+                #                 "amount": "0.0001",
+                #                 "base_fee": "0",
+                #                 "ccy": "BTC",
+                #                 "client_id": "x-167673045-f3651372049dab0d",
+                #                 "created_at": 1714121403450,
+                #                 "discount_fee": "0",
+                #                 "filled_amount": "0",
+                #                 "filled_value": "0",
+                #                 "last_fill_amount": "0",
+                #                 "last_fill_price": "0",
+                #                 "maker_fee_rate": "0.002",
+                #                 "market": "BTCUSDT",
+                #                 "market_type": "SPOT",
+                #                 "order_id": 117185362233,
+                #                 "price": "61000",
+                #                 "quote_fee": "0",
+                #                 "side": "buy",
+                #                 "taker_fee_rate": "0.002",
+                #                 "type": "limit",
+                #                 "unfilled_amount": "0.0001",
+                #                 "updated_at": 1714121403450
+                #             },
+                #             {
+                #                 "code": 3109,
+                #                 "data": null,
+                #                 "message": "balance not enough"
+                #             }
+                #         ],
+                #         "message": "OK"
+                #     }
+                #
+        else:
+            if isTriggerOrder:
+                response = await self.v2PrivatePostFuturesBatchStopOrder(request)
+                #
+                #     {
+                #         "code": 0,
+                #         "data": [
+                #             {
+                #                 "code": 0,
+                #                 "data": {
+                #                     "stop_id": 136919625994
+                #                 },
+                #                 "message": "OK"
+                #             },
+                #         ],
+                #         "message": "OK"
+                #     }
+                #
+            elif isStopLossOrTakeProfitTrigger:
+                raise NotSupported(self.id + ' createOrders() does not support stopLossPrice or takeProfitPrice orders')
+            else:
+                if reduceOnly:
+                    raise NotSupported(self.id + ' createOrders() does not support reduceOnly orders')
+                else:
+                    response = await self.v2PrivatePostFuturesBatchOrder(request)
+                    #
+                    #     {
+                    #         "code": 0,
+                    #         "data": [
+                    #             {
+                    #                 "code": 0,
+                    #                 "data": {
+                    #                     "amount": "0.0001",
+                    #                     "client_id": "x-167673045-2cb7436f3462a654",
+                    #                     "created_at": 1714122832493,
+                    #                     "fee": "0",
+                    #                     "fee_ccy": "USDT",
+                    #                     "filled_amount": "0",
+                    #                     "filled_value": "0",
+                    #                     "last_filled_amount": "0",
+                    #                     "last_filled_price": "0",
+                    #                     "maker_fee_rate": "0.0003",
+                    #                     "market": "BTCUSDT",
+                    #                     "market_type": "FUTURES",
+                    #                     "order_id": 136918835063,
+                    #                     "price": "61000",
+                    #                     "realized_pnl": "0",
+                    #                     "side": "buy",
+                    #                     "taker_fee_rate": "0.0005",
+                    #                     "type": "limit",
+                    #                     "unfilled_amount": "0.0001",
+                    #                     "updated_at": 1714122832493
+                    #                 },
+                    #                 "message": "OK"
+                    #             },
+                    #         ],
+                    #         "message": "OK"
+                    #     }
+                    #
+        data = self.safe_list(response, 'data', [])
         results = []
         for i in range(0, len(data)):
             entry = data[i]
             status = None
             code = self.safe_integer(entry, 'code')
             if code is not None:
                 if code != 0:
                     status = 'rejected'
                 else:
                     status = 'open'
-            item = self.safe_value(entry, 'data', {})
-            item['status'] = status
-            order = self.parse_order(item, market)
+            innerData = self.safe_dict(entry, 'data', {})
+            order = None
+            if market['spot'] and not isTriggerOrder:
+                entry['status'] = status
+                order = self.parse_order(entry, market)
+            else:
+                innerData['status'] = status
+                order = self.parse_order(innerData, market)
             results.append(order)
         return results
 
-    def cancel_orders(self, ids, symbol: Str = None, params={}):
+    async def cancel_orders(self, ids, symbol: Str = None, params={}):
         """
         cancel multiple orders
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade016_batch_cancel_order
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http021-0_cancel_order_batch
         :param str[] ids: order ids
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' cancelOrders() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
         idsString = ','.join(ids)
         response = None
         if market['spot']:
             request['batch_ids'] = idsString
-            response = self.v1PrivateDeleteOrderPendingBatch(self.extend(request, params))
+            response = await self.v1PrivateDeleteOrderPendingBatch(self.extend(request, params))
         else:
             request['order_ids'] = idsString
-            response = self.v1PerpetualPrivatePostOrderCancelBatch(self.extend(request, params))
+            response = await self.v1PerpetualPrivatePostOrderCancelBatch(self.extend(request, params))
         #
         # spot
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
@@ -2489,42 +2735,42 @@
             entry = data[i]
             dataRequest = 'data' if market['spot'] else 'order'
             item = self.safe_value(entry, dataRequest, {})
             order = self.parse_order(item, market)
             results.append(order)
         return results
 
-    def edit_order(self, id: str, symbol: str, type: OrderType, side: OrderSide, amount: Num = None, price: Num = None, params={}):
+    async def edit_order(self, id: str, symbol: str, type: OrderType, side: OrderSide, amount: Num = None, price: Num = None, params={}):
         """
         edit a trade order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade022_modify_order
         :param str id: order id
         :param str symbol: unified symbol of the market to create an order in
         :param str type: 'market' or 'limit'
         :param str side: 'buy' or 'sell'
         :param float amount: how much of the currency you want to trade in units of the base currency
         :param float [price]: the price at which the order is to be fullfilled, in units of the quote currency, ignored in market orders
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' editOrder() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if not market['spot']:
             raise NotSupported(self.id + ' editOrder() does not support ' + market['type'] + ' orders, only spot orders are accepted')
         request = {
             'market': market['id'],
             'id': int(id),
         }
         if amount is not None:
             request['amount'] = self.amount_to_precision(symbol, amount)
         if price is not None:
             request['price'] = self.price_to_precision(symbol, price)
-        response = self.v1PrivatePostOrderModify(self.extend(request, params))
+        response = await self.v1PrivatePostOrderModify(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "id": 35436205,
         #             "create_time": 1636080705,
         #             "finished_time": null,
@@ -2551,15 +2797,15 @@
         #     },
         #         "message": "Success"
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         return self.parse_order(data, market)
 
-    def cancel_order(self, id: str, symbol: Str = None, params={}):
+    async def cancel_order(self, id: str, symbol: Str = None, params={}):
         """
         cancels an open order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade018_cancle_stop_pending_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade015_cancel_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade024_cancel_order_by_client_id
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade025_cancel_stop_order_by_client_id
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http023_cancel_stop_order
@@ -2571,15 +2817,15 @@
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.clientOrderId]: client order id, defaults to id if not passed
         :param boolean [params.stop]: if stop order = True, default = False
         :returns dict: An `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' cancelOrder() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         stop = self.safe_value(params, 'stop')
         swap = market['swap']
         request = {
             'market': market['id'],
         }
         accountId = self.safe_integer(params, 'account_id')
@@ -2592,35 +2838,35 @@
             request['account_id'] = accountId
         query = self.omit(params, ['stop', 'account_id', 'clientOrderId'])
         response = None
         if clientOrderId is not None:
             request['client_id'] = clientOrderId
             if stop:
                 if swap:
-                    response = self.v1PerpetualPrivatePostOrderCancelStopByClientId(self.extend(request, query))
+                    response = await self.v1PerpetualPrivatePostOrderCancelStopByClientId(self.extend(request, query))
                 else:
-                    response = self.v1PrivateDeleteOrderStopPendingByClientId(self.extend(request, query))
+                    response = await self.v1PrivateDeleteOrderStopPendingByClientId(self.extend(request, query))
             else:
                 if swap:
-                    response = self.v1PerpetualPrivatePostOrderCancelByClientId(self.extend(request, query))
+                    response = await self.v1PerpetualPrivatePostOrderCancelByClientId(self.extend(request, query))
                 else:
-                    response = self.v1PrivateDeleteOrderPendingByClientId(self.extend(request, query))
+                    response = await self.v1PrivateDeleteOrderPendingByClientId(self.extend(request, query))
         else:
             idRequest = 'order_id' if swap else 'id'
             request[idRequest] = id
             if stop:
                 if swap:
-                    response = self.v1PerpetualPrivatePostOrderCancelStop(self.extend(request, query))
+                    response = await self.v1PerpetualPrivatePostOrderCancelStop(self.extend(request, query))
                 else:
-                    response = self.v1PrivateDeleteOrderStopPendingId(self.extend(request, query))
+                    response = await self.v1PrivateDeleteOrderStopPendingId(self.extend(request, query))
             else:
                 if swap:
-                    response = self.v1PerpetualPrivatePostOrderCancel(self.extend(request, query))
+                    response = await self.v1PerpetualPrivatePostOrderCancel(self.extend(request, query))
                 else:
-                    response = self.v1PrivateDeleteOrderPending(self.extend(request, query))
+                    response = await self.v1PrivateDeleteOrderPending(self.extend(request, query))
         #
         # Spot and Margin
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "amount": "0.0005",
@@ -2722,94 +2968,94 @@
         # Spot and Margin Stop
         #
         #     {"code":0,"data":{},"message":"Success"}
         #
         data = self.safe_dict(response, 'data')
         return self.parse_order(data, market)
 
-    def cancel_all_orders(self, symbol: Str = None, params={}):
+    async def cancel_all_orders(self, symbol: Str = None, params={}):
         """
         cancel all open orders in a market
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade018_cancle_stop_pending_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade015_cancel_order
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http024_cancel_stop_all
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http022_cancel_all
         :param str symbol: unified market symbol of the market to cancel orders in
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' cancelAllOrders() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         accountId = self.safe_integer(params, 'account_id', 0)
         request = {
             'market': marketId,
             # 'account_id': accountId,  # SPOT, main account ID: 0, margin account ID: See < Inquire Margin Account Market Info >, future account ID: See < Inquire Future Account Market Info >
             # 'side': 0,  # SWAP, 0: All, 1: Sell, 2: Buy
         }
         swap = market['swap']
         stop = self.safe_value(params, 'stop')
         params = self.omit(params, ['stop', 'account_id'])
         response = None
         if swap:
             if stop:
-                response = self.v1PerpetualPrivatePostOrderCancelStopAll(self.extend(request, params))
+                response = await self.v1PerpetualPrivatePostOrderCancelStopAll(self.extend(request, params))
             else:
-                response = self.v1PerpetualPrivatePostOrderCancelAll(self.extend(request, params))
+                response = await self.v1PerpetualPrivatePostOrderCancelAll(self.extend(request, params))
         else:
             request['account_id'] = accountId
             if stop:
-                response = self.v1PrivateDeleteOrderStopPending(self.extend(request, params))
+                response = await self.v1PrivateDeleteOrderStopPending(self.extend(request, params))
             else:
-                response = self.v1PrivateDeleteOrderPending(self.extend(request, params))
+                response = await self.v1PrivateDeleteOrderPending(self.extend(request, params))
         #
         # Spot and Margin
         #
         #     {"code": 0, "data": null, "message": "Success"}
         #
         # Swap
         #
         #     {"code": 0, "data": {"status":"success"}, "message": "OK"}
         #
         return response
 
-    def fetch_order(self, id: str, symbol: Str = None, params={}):
+    async def fetch_order(self, id: str, symbol: Str = None, params={}):
         """
         fetches information on an order made by the user
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http028_stop_status
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http026_order_status
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade007_order_status
         :param str symbol: unified symbol of the market the order was made in
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: An `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' fetchOrder() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         swap = market['swap']
         stop = self.safe_value(params, 'stop')
         params = self.omit(params, 'stop')
         request = {
             'market': market['id'],
             # 'id': id,  # SPOT
             # 'order_id': id,  # SWAP
         }
         idRequest = 'order_id' if swap else 'id'
         request[idRequest] = id
         response = None
         if swap:
             if stop:
-                response = self.v1PerpetualPrivateGetOrderStopStatus(self.extend(request, params))
+                response = await self.v1PerpetualPrivateGetOrderStopStatus(self.extend(request, params))
             else:
-                response = self.v1PerpetualPrivateGetOrderStatus(self.extend(request, params))
+                response = await self.v1PerpetualPrivateGetOrderStatus(self.extend(request, params))
         else:
-            response = self.v1PrivateGetOrderStatus(self.extend(request, params))
+            response = await self.v1PrivateGetOrderStatus(self.extend(request, params))
         #
         # Spot
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "amount": "0.1",
@@ -2903,16 +3149,16 @@
         #         },
         #         "message":"OK"
         #     }
         #
         data = self.safe_dict(response, 'data')
         return self.parse_order(data, market)
 
-    def fetch_orders_by_status(self, status, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
-        self.load_markets()
+    async def fetch_orders_by_status(self, status, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+        await self.load_markets()
         limit = 100 if (limit is None) else limit
         request = {
             'limit': limit,
             # 'page': 1,  # SPOT
             # 'offset': 0,  # SWAP
             # 'side': 0,  # SWAP, 0: All, 1: Sell, 2: Buy
         }
@@ -2938,32 +3184,32 @@
                 raise ArgumentsRequired(self.id + ' fetchOrdersByStatus() requires a symbol argument for swap markets')
             if side is not None:
                 request['side'] = side
             else:
                 request['side'] = 0
             request['offset'] = 0
             if stop:
-                response = self.v1PerpetualPrivateGetOrderStopPending(self.extend(request, params))
+                response = await self.v1PerpetualPrivateGetOrderStopPending(self.extend(request, params))
             else:
                 if status == 'finished':
-                    response = self.v1PerpetualPrivateGetOrderFinished(self.extend(request, params))
+                    response = await self.v1PerpetualPrivateGetOrderFinished(self.extend(request, params))
                 elif status == 'pending':
-                    response = self.v1PerpetualPrivateGetOrderPending(self.extend(request, params))
+                    response = await self.v1PerpetualPrivateGetOrderPending(self.extend(request, params))
         else:
             request['page'] = 1
             if status == 'finished':
                 if stop:
-                    response = self.v1PrivateGetOrderStopFinished(self.extend(request, params))
+                    response = await self.v1PrivateGetOrderStopFinished(self.extend(request, params))
                 else:
-                    response = self.v1PrivateGetOrderFinished(self.extend(request, params))
+                    response = await self.v1PrivateGetOrderFinished(self.extend(request, params))
             elif status == 'pending':
                 if stop:
-                    response = self.v1PrivateGetOrderStopPending(self.extend(request, params))
+                    response = await self.v1PrivateGetOrderStopPending(self.extend(request, params))
                 else:
-                    response = self.v1PrivateGetOrderPending(self.extend(request, params))
+                    response = await self.v1PrivateGetOrderPending(self.extend(request, params))
         #
         # Spot and Margin
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "count": 1,
@@ -3111,82 +3357,82 @@
         #     }
         #
         tradeRequest = 'records' if (marketType == 'swap') else 'data'
         data = self.safe_value(response, 'data')
         orders = self.safe_list(data, tradeRequest, [])
         return self.parse_orders(orders, market, since, limit)
 
-    def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
+    async def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
         """
         fetch all unfilled currently open orders
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http027_query_pending_stop
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http025_query_pending
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade013_stop_pending_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade011_pending_order
         :param str symbol: unified market symbol
         :param int [since]: the earliest time in ms to fetch open orders for
         :param int [limit]: the maximum number of  open orders structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Order[]: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        return self.fetch_orders_by_status('pending', symbol, since, limit, params)
+        return await self.fetch_orders_by_status('pending', symbol, since, limit, params)
 
-    def fetch_closed_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
+    async def fetch_closed_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
         """
         fetches information on multiple closed orders made by the user
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http029_query_finished
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade010_stop_finished_order
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade012_finished_order
         :param str symbol: unified market symbol of the market orders were made in
         :param int [since]: the earliest time in ms to fetch orders for
         :param int [limit]: the maximum number of order structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Order[]: a list of `order structures <https://docs.ccxt.com/#/?id=order-structure>`
         """
-        return self.fetch_orders_by_status('finished', symbol, since, limit, params)
+        return await self.fetch_orders_by_status('finished', symbol, since, limit, params)
 
-    def create_deposit_address(self, code: str, params={}):
+    async def create_deposit_address(self, code: str, params={}):
         """
         create a currency deposit address
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account019_update_deposit_address
         :param str code: unified currency code of the currency for the deposit address
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `address structure <https://docs.ccxt.com/#/?id=address-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         currency = self.currency(code)
         request = {
             'coin_type': currency['id'],
         }
         if 'network' in params:
             network = self.safe_string(params, 'network')
             params = self.omit(params, 'network')
             request['smart_contract_name'] = network
-        response = self.v1PrivatePutBalanceDepositAddressCoinType(self.extend(request, params))
+        response = await self.v1PrivatePutBalanceDepositAddressCoinType(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "coin_address": "TV639dSpb9iGRtoFYkCp4AoaaDYKrK1pw5",
         #             "is_bitcoin_cash": False
         #         },
         #         "message": "Success"
         #     }
         data = self.safe_dict(response, 'data', {})
         return self.parse_deposit_address(data, currency)
 
-    def fetch_deposit_address(self, code: str, params={}):
+    async def fetch_deposit_address(self, code: str, params={}):
         """
         fetch the deposit address for a currency associated with self account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account020_query_deposit_address
         :param str code: unified currency code
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `address structure <https://docs.ccxt.com/#/?id=address-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         currency = self.currency(code)
         request = {
             'coin_type': currency['id'],
         }
         networks = self.safe_value(currency, 'networks', {})
         network = self.safe_string(params, 'network')
         params = self.omit(params, 'network')
@@ -3195,15 +3441,15 @@
         if networks is not None and numOfNetworks > 1:
             if network is None:
                 raise ArgumentsRequired(self.id + ' fetchDepositAddress() ' + code + ' requires a network parameter')
             if not (network in networks):
                 raise ExchangeError(self.id + ' fetchDepositAddress() ' + network + ' network not supported for ' + code)
         if network is not None:
             request['smart_contract_name'] = network
-        response = self.v1PrivateGetBalanceDepositAddressCoinType(self.extend(request, params))
+        response = await self.v1PrivateGetBalanceDepositAddressCoinType(self.extend(request, params))
         #
         #      {
         #          "code": 0,
         #          "data": {
         #            "coin_address": "1P1JqozxioQwaqPwgMAQdNDYNyaVSqgARq",
         #            # coin_address: "xxxxxxxxxxxxxx:yyyyyyyyy",  # with embedded tag/memo
         #            "is_bitcoin_cash": False
@@ -3255,26 +3501,26 @@
             'info': depositAddress,
             'currency': self.safe_currency_code(None, currency),
             'address': address,
             'tag': tag,
             'network': None,
         }
 
-    def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+    async def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch all trades made by the user
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http013_user_deals
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot003_trade014_user_deals
         :param str symbol: unified market symbol
         :param int [since]: the earliest time in ms to fetch trades for
         :param int [limit]: the maximum number of trades structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns Trade[]: a list of `trade structures <https://docs.ccxt.com/#/?id=trade-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = None
         if limit is None:
             limit = 100
         request = {
             'limit': limit,  # SPOT and SWAP
             'offset': 0,  # SWAP, means query from a certain record
             # 'page': 1,  # SPOT
@@ -3299,18 +3545,18 @@
             request['account_id'] = accountId
             params = self.omit(params, 'account_id')
         response = None
         if swap:
             if since is not None:
                 request['start_time'] = since
             request['side'] = 0
-            response = self.v1PerpetualPrivateGetMarketUserDeals(self.extend(request, params))
+            response = await self.v1PerpetualPrivateGetMarketUserDeals(self.extend(request, params))
         else:
             request['page'] = 1
-            response = self.v1PrivateGetOrderUserDeals(self.extend(request, params))
+            response = await self.v1PrivateGetOrderUserDeals(self.extend(request, params))
         #
         # Spot and Margin
         #
         #      {
         #          "code": 0,
         #          "data": {
         #              "data": [
@@ -3380,26 +3626,26 @@
         #     }
         #
         tradeRequest = 'records' if swap else 'data'
         data = self.safe_value(response, 'data')
         trades = self.safe_list(data, tradeRequest, [])
         return self.parse_trades(trades, market, since, limit)
 
-    def fetch_positions(self, symbols: Strings = None, params={}):
+    async def fetch_positions(self, symbols: Strings = None, params={}):
         """
         fetch all open positions
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033_pending_position
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033-0_finished_position
         :param str[] [symbols]: list of unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.method]: the method to use 'perpetualPrivateGetPositionPending' or 'perpetualPrivateGetPositionFinished' default is 'perpetualPrivateGetPositionPending'
         :param int [params.side]: *history endpoint only* 0: All, 1: Sell, 2: Buy, default is 0
         :returns dict[]: a list of `position structure <https://docs.ccxt.com/#/?id=position-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         defaultMethod = None
         defaultMethod, params = self.handle_option_and_params(params, 'fetchPositions', 'method', 'v1PerpetualPrivateGetPositionPending')
         isHistory = (defaultMethod == 'v1PerpetualPrivateGetPositionFinished')
         symbols = self.market_symbols(symbols)
         request = {}
         market = None
         if symbols is not None:
@@ -3417,17 +3663,17 @@
             if isHistory:
                 raise ArgumentsRequired(self.id + ' fetchPositions() requires a symbol argument for closed positions')
         if isHistory:
             request['limit'] = 100
             request['side'] = self.safe_integer(params, 'side', 0)  # 0: All, 1: Sell, 2: Buy
         response = None
         if defaultMethod == 'v1PerpetualPrivateGetPositionPending':
-            response = self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
+            response = await self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
         else:
-            response = self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
+            response = await self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "adl_sort": 3396,
         #                 "adl_sort_val": "0.00007786",
@@ -3485,28 +3731,28 @@
         #
         position = self.safe_value(response, 'data', [])
         result = []
         for i in range(0, len(position)):
             result.append(self.parse_position(position[i], market))
         return self.filter_by_array_positions(result, 'symbol', symbols, False)
 
-    def fetch_position(self, symbol: str, params={}):
+    async def fetch_position(self, symbol: str, params={}):
         """
         fetch data on a single open contract trade position
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033_pending_position
         :param str symbol: unified market symbol of the market the position is held in, default is None
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `position structure <https://docs.ccxt.com/#/?id=position-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
-        response = self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
+        response = await self.v1PerpetualPrivateGetPositionPending(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "adl_sort": 3396,
         #                 "adl_sort_val": "0.00007786",
@@ -3701,29 +3947,29 @@
             'initialMarginPercentage': self.parse_number(initialMarginPercentage),
             'leverage': self.parse_number(leverage),
             'marginRatio': None,
             'stopLossPrice': self.omit_zero(self.safe_string(position, 'stop_loss_price')),
             'takeProfitPrice': self.omit_zero(self.safe_string(position, 'take_profit_price')),
         })
 
-    def set_margin_mode(self, marginMode: str, symbol: Str = None, params={}):
+    async def set_margin_mode(self, marginMode: str, symbol: Str = None, params={}):
         """
         set margin mode to 'cross' or 'isolated'
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http014_adjust_leverage
         :param str marginMode: 'cross' or 'isolated'
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: response from the exchange
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' setMarginMode() requires a symbol argument')
         marginMode = marginMode.lower()
         if marginMode != 'isolated' and marginMode != 'cross':
             raise BadRequest(self.id + ' setMarginMode() marginMode argument should be isolated or cross')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if market['type'] != 'swap':
             raise BadSymbol(self.id + ' setMarginMode() supports swap contracts only')
         defaultPositionType = None
         if marginMode == 'isolated':
             defaultPositionType = 1
         elif marginMode == 'cross':
@@ -3738,29 +3984,29 @@
         if (leverage < 3) or (leverage > maxLeverage):
             raise BadRequest(self.id + ' setMarginMode() leverage should be between 3 and ' + str(maxLeverage) + ' for ' + symbol)
         request = {
             'market': market['id'],
             'leverage': str(leverage),
             'position_type': positionType,  # 1: isolated, 2: cross
         }
-        return self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
+        return await self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
 
-    def set_leverage(self, leverage: Int, symbol: Str = None, params={}):
+    async def set_leverage(self, leverage: Int, symbol: Str = None, params={}):
         """
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http014_adjust_leverage
         set the level of leverage for a market
         :param float leverage: the rate of leverage
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.marginMode]: 'cross' or 'isolated'(default is 'cross')
         :returns dict: response from the exchange
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' setLeverage() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if not market['swap']:
             raise BadSymbol(self.id + ' setLeverage() supports swap contracts only')
         marginMode = None
         marginMode, params = self.handle_margin_mode_and_params('setLeverage', params, 'cross')
         positionType = None
         if marginMode == 'isolated':
@@ -3772,26 +4018,26 @@
         if (leverage < minLeverage) or (leverage > maxLeverage):
             raise BadRequest(self.id + ' setLeverage() leverage should be between ' + str(minLeverage) + ' and ' + str(maxLeverage) + ' for ' + symbol)
         request = {
             'market': market['id'],
             'leverage': str(leverage),
             'position_type': positionType,  # 1: isolated, 2: cross
         }
-        return self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
+        return await self.v1PerpetualPrivatePostMarketAdjustLeverage(self.extend(request, params))
 
-    def fetch_leverage_tiers(self, symbols: Strings = None, params={}):
+    async def fetch_leverage_tiers(self, symbols: Strings = None, params={}):
         """
         retrieve information on the maximum leverage, and maintenance margin for trades of varying trade sizes
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http007_market_limit
         :param str[]|None symbols: list of unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a dictionary of `leverage tiers structures <https://docs.ccxt.com/#/?id=leverage-tiers-structure>`, indexed by market symbols
         """
-        self.load_markets()
-        response = self.v1PerpetualPublicGetMarketLimitConfig(params)
+        await self.load_markets()
+        response = await self.v1PerpetualPublicGetMarketLimitConfig(params)
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "BTCUSD": [
         #                 ["500001", "100", "0.005"],
         #                 ["1000001", "50", "0.01"],
@@ -3822,23 +4068,23 @@
                 'maintenanceMarginRate': self.safe_number(bracket, 2),
                 'maxLeverage': self.safe_integer(bracket, 1),
                 'info': bracket,
             })
             minNotional = maxNotional
         return tiers
 
-    def modify_margin_helper(self, symbol: str, amount, addOrReduce, params={}):
-        self.load_markets()
+    async def modify_margin_helper(self, symbol: str, amount, addOrReduce, params={}):
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'amount': self.amount_to_precision(symbol, amount),
             'type': addOrReduce,
         }
-        response = self.v1PerpetualPrivatePostPositionAdjustMargin(self.extend(request, params))
+        response = await self.v1PerpetualPrivatePostPositionAdjustMargin(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "adl_sort": 1,
         #             "adl_sort_val": "0.00004320",
         #             "amount": "0.0005",
@@ -3985,61 +4231,61 @@
             'total': self.safe_number(data, 'position_amount'),
             'code': market['quote'],
             'status': None,
             'timestamp': timestamp,
             'datetime': self.iso8601(timestamp),
         }
 
-    def add_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
+    async def add_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
         """
         add margin
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http032_adjust_position_margin
         :param str symbol: unified market symbol
         :param float amount: amount of margin to add
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `margin structure <https://docs.ccxt.com/#/?id=add-margin-structure>`
         """
-        return self.modify_margin_helper(symbol, amount, 1, params)
+        return await self.modify_margin_helper(symbol, amount, 1, params)
 
-    def reduce_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
+    async def reduce_margin(self, symbol: str, amount: float, params={}) -> MarginModification:
         """
         remove margin from a position
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http032_adjust_position_margin
         :param str symbol: unified market symbol
         :param float amount: the amount of margin to remove
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `margin structure <https://docs.ccxt.com/#/?id=reduce-margin-structure>`
         """
-        return self.modify_margin_helper(symbol, amount, 2, params)
+        return await self.modify_margin_helper(symbol, amount, 2, params)
 
-    def fetch_funding_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+    async def fetch_funding_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch the history of funding payments paid and received on self account
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http034_funding_position
         :param str symbol: unified market symbol
         :param int [since]: the earliest time in ms to fetch funding history for
         :param int [limit]: the maximum number of funding history structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `funding history structure <https://docs.ccxt.com/#/?id=funding-history-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' fetchFundingHistory() requires a symbol argument')
         limit = 100 if (limit is None) else limit
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'limit': limit,
             # 'offset': 0,
             # 'end_time': 1638990636000,
             # 'windowtime': 1638990636000,
         }
         if since is not None:
             request['start_time'] = since
-        response = self.v1PerpetualPrivateGetPositionFunding(self.extend(request, params))
+        response = await self.v1PerpetualPrivateGetPositionFunding(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "limit": 100,
         #             "offset": 0,
         #             "records": [
@@ -4078,30 +4324,30 @@
                 'timestamp': timestamp,
                 'datetime': self.iso8601(timestamp),
                 'id': self.safe_number(entry, 'position_id'),
                 'amount': self.safe_number(entry, 'funding'),
             })
         return result
 
-    def fetch_funding_rate(self, symbol: str, params={}):
+    async def fetch_funding_rate(self, symbol: str, params={}):
         """
         fetch the current funding rate
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http008_market_ticker
         :param str symbol: unified market symbol
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `funding rate structure <https://docs.ccxt.com/#/?id=funding-rate-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if not market['swap']:
             raise BadSymbol(self.id + ' fetchFundingRate() supports swap contracts only')
         request = {
             'market': market['id'],
         }
-        response = self.v1PerpetualPublicGetMarketTicker(self.extend(request, params))
+        response = await self.v1PerpetualPublicGetMarketTicker(self.extend(request, params))
         #
         #     {
         #          "code": 0,
         #         "data":
         #         {
         #             "date": 1650678472474,
         #             "ticker": {
@@ -4184,31 +4430,31 @@
             'nextFundingTimestamp': None,
             'nextFundingDatetime': None,
             'previousFundingRate': self.safe_number(contract, 'funding_rate_last'),
             'previousFundingTimestamp': None,
             'previousFundingDatetime': None,
         }
 
-    def fetch_funding_rates(self, symbols: Strings = None, params={}):
+    async def fetch_funding_rates(self, symbols: Strings = None, params={}):
         """
         fetch the current funding rates
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http009_market_ticker_all
         :param str[] symbols: unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: an array of `funding rate structures <https://docs.ccxt.com/#/?id=funding-rate-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         symbols = self.market_symbols(symbols)
         market = None
         if symbols is not None:
             symbol = self.safe_value(symbols, 0)
             market = self.market(symbol)
             if not market['swap']:
                 raise BadSymbol(self.id + ' fetchFundingRates() supports swap contracts only')
-        response = self.v1PerpetualPublicGetMarketTickerAll(params)
+        response = await self.v1PerpetualPublicGetMarketTickerAll(params)
         #
         #     {
         #         "code": 0,
         #         "data":
         #         {
         #             "date": 1650678472474,
         #             "ticker": {
@@ -4248,43 +4494,43 @@
             if marketId.find('_') == -1:  # skip _signprice and _indexprice
                 marketInner = self.safe_market(marketId, None, None, 'swap')
                 ticker = tickers[marketId]
                 ticker['timestamp'] = timestamp
                 result.append(self.parse_funding_rate(ticker, marketInner))
         return self.filter_by_array(result, 'symbol', symbols)
 
-    def withdraw(self, code: str, amount: float, address: str, tag=None, params={}):
+    async def withdraw(self, code: str, amount: float, address: str, tag=None, params={}):
         """
         make a withdrawal
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account015_submit_withdraw
         :param str code: unified currency code
         :param float amount: the amount to withdraw
         :param str address: the address to withdraw to
         :param str tag:
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.network]: unified network code
         :returns dict: a `transaction structure <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         tag, params = self.handle_withdraw_tag_and_params(tag, params)
         self.check_address(address)
-        self.load_markets()
+        await self.load_markets()
         currency = self.currency(code)
         networkCode = self.safe_string_upper(params, 'network')
         params = self.omit(params, 'network')
         if tag:
             address = address + ':' + tag
         request = {
             'coin_type': currency['id'],
             'coin_address': address,  # must be authorized, inter-user transfer by a registered mobile phone number or an email address is supported
             'actual_amount': float(self.number_to_string(amount)),  # the actual amount without fees, https://www.coinex.com/fees
             'transfer_method': 'onchain',  # onchain, local
         }
         if networkCode is not None:
             request['smart_contract_name'] = self.network_code_to_id(networkCode)
-        response = self.v1PrivatePostBalanceCoinWithdraw(self.extend(request, params))
+        response = await self.v1PrivatePostBalanceCoinWithdraw(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "actual_amount": "1.00000000",
         #             "amount": "1.00000000",
         #             "coin_address": "1KAv3pazbTk2JnQ5xTo6fpKK7p1it2RzD4",
@@ -4311,46 +4557,46 @@
             'not_pass': 'failed',
             'cancel': 'canceled',
             'finish': 'ok',
             'fail': 'failed',
         }
         return self.safe_string(statuses, status, status)
 
-    def fetch_funding_rate_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+    async def fetch_funding_rate_history(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http038_funding_history
         fetches historical funding rate prices
         :param str symbol: unified symbol of the market to fetch the funding rate history for
         :param int [since]: timestamp in ms of the earliest funding rate to fetch
         :param int [limit]: the maximum amount of `funding rate structures <https://docs.ccxt.com/#/?id=funding-rate-history-structure>` to fetch
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param boolean [params.paginate]: default False, when True will automatically paginate by calling self endpoint multiple times. See in the docs all the [availble parameters](https://github.com/ccxt/ccxt/wiki/Manual#pagination-params)
         :param int [params.until]: timestamp in ms of the latest funding rate
         :returns dict[]: a list of `funding rate structures <https://docs.ccxt.com/#/?id=funding-rate-history-structure>`
         """
         if symbol is None:
             raise ArgumentsRequired(self.id + ' fetchFundingRateHistory() requires a symbol argument')
-        self.load_markets()
+        await self.load_markets()
         paginate = False
         paginate, params = self.handle_option_and_params(params, 'fetchFundingRateHistory', 'paginate')
         if paginate:
-            return self.fetch_paginated_call_deterministic('fetchFundingRateHistory', symbol, since, limit, '8h', params, 1000)
+            return await self.fetch_paginated_call_deterministic('fetchFundingRateHistory', symbol, since, limit, '8h', params, 1000)
         if limit is None:
             limit = 100
         market = self.market(symbol)
         request = {
             'market': market['id'],
             'limit': limit,
             'offset': 0,
             # 'end_time': 1638990636,
         }
         if since is not None:
             request['start_time'] = since
         request, params = self.handle_until_option('end_time', request, params)
-        response = self.v1PerpetualPublicGetMarketFundingHistory(self.extend(request, params))
+        response = await self.v1PerpetualPublicGetMarketFundingHistory(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "offset": 0,
         #             "limit": 3,
         #             "records": [
@@ -4488,49 +4734,49 @@
             'status': status,
             'updated': None,
             'fee': fee,
             'comment': None,
             'internal': internal,
         }
 
-    def transfer(self, code: str, amount: float, fromAccount: str, toAccount: str, params={}) -> TransferEntry:
+    async def transfer(self, code: str, amount: float, fromAccount: str, toAccount: str, params={}) -> TransferEntry:
         """
         transfer currency internally between wallets on the same account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account014_balance_contract_transfer
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account013_margin_transfer
         :param str code: unified currency code
         :param float amount: amount to transfer
         :param str fromAccount: account to transfer from
         :param str toAccount: account to transfer to
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `transfer structure <https://docs.ccxt.com/#/?id=transfer-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         currency = self.currency(code)
         amountToPrecision = self.currency_to_precision(code, amount)
         request = {
             'amount': amountToPrecision,
             'coin_type': currency['id'],
         }
         response = None
         if (fromAccount == 'spot') and (toAccount == 'swap'):
             request['transfer_side'] = 'in'  # 'in' spot to swap, 'out' swap to spot
-            response = self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
+            response = await self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
         elif (fromAccount == 'swap') and (toAccount == 'spot'):
             request['transfer_side'] = 'out'  # 'in' spot to swap, 'out' swap to spot
-            response = self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
+            response = await self.v1PrivatePostContractBalanceTransfer(self.extend(request, params))
         else:
             accountsById = self.safe_value(self.options, 'accountsById', {})
             fromId = self.safe_string(accountsById, fromAccount, fromAccount)
             toId = self.safe_string(accountsById, toAccount, toAccount)
             # fromAccount and toAccount must be integers for margin transfers
             # spot is 0, use fetchBalance() to find the margin account id
             request['from_account'] = int(fromId)
             request['to_account'] = int(toId)
-            response = self.v1PrivatePostMarginTransfer(self.extend(request, params))
+            response = await self.v1PrivatePostMarginTransfer(self.extend(request, params))
         #
         #     {"code": 0, "data": null, "message": "Success"}
         #
         return self.extend(self.parse_transfer(response, currency), {
             'amount': self.parse_number(amountToPrecision),
             'fromAccount': fromAccount,
             'toAccount': toAccount,
@@ -4596,26 +4842,26 @@
             'currency': currencyCode,
             'amount': self.safe_number(transfer, 'amount'),
             'fromAccount': fromAccount,
             'toAccount': toAccount,
             'status': self.parse_transfer_status(self.safe_string_2(transfer, 'code', 'status')),
         }
 
-    def fetch_transfers(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
+    async def fetch_transfers(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch a history of internal transfers made on an account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account025_margin_transfer_history
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account024_contract_transfer_history
         :param str code: unified currency code of the currency transferred
         :param int [since]: the earliest time in ms to fetch transfers for
         :param int [limit]: the maximum number of  transfers structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `transfer structures <https://docs.ccxt.com/#/?id=transfer-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         currency = None
         request = {
             'page': 1,
             # 'limit': limit,
             # 'asset': 'USDT',
             # 'start_time': since,
             # 'end_time': 1515806440,
@@ -4634,17 +4880,17 @@
         else:
             request['limit'] = 100
         params = self.omit(params, 'page')
         marginMode = None
         marginMode, params = self.handle_margin_mode_and_params('fetchTransfers', params)
         response = None
         if marginMode is not None:
-            response = self.v1PrivateGetMarginTransferHistory(self.extend(request, params))
+            response = await self.v1PrivateGetMarginTransferHistory(self.extend(request, params))
         else:
-            response = self.v1PrivateGetContractTransferHistory(self.extend(request, params))
+            response = await self.v1PrivateGetContractTransferHistory(self.extend(request, params))
         #
         # Swap
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "records": [
@@ -4685,33 +4931,33 @@
         #         "message": "Success"
         #     }
         #
         data = self.safe_value(response, 'data', {})
         transfers = self.safe_list(data, 'records', [])
         return self.parse_transfers(transfers, currency, since, limit)
 
-    def fetch_withdrawals(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
+    async def fetch_withdrawals(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
         """
         fetch all withdrawals made from an account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account026_withdraw_list
         :param str code: unified currency code
         :param int [since]: the earliest time in ms to fetch withdrawals for
         :param int [limit]: the maximum number of withdrawals structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `transaction structures <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         request = {}
         currency = None
         if code is not None:
-            self.load_markets()
+            await self.load_markets()
             currency = self.currency(code)
             request['coin_type'] = currency['id']
         if limit is not None:
             request['Limit'] = limit
-        response = self.v1PrivateGetBalanceCoinWithdraw(self.extend(request, params))
+        response = await self.v1PrivateGetBalanceCoinWithdraw(self.extend(request, params))
         #
         #    {
         #        "code": 0,
         #        "data": {
         #            "has_next": False,
         #            "curr_page": 1,
         #            "count": 1,
@@ -4747,33 +4993,33 @@
         #    }
         #
         data = self.safe_value(response, 'data')
         if not isinstance(data, list):
             data = self.safe_value(data, 'data', [])
         return self.parse_transactions(data, currency, since, limit)
 
-    def fetch_deposits(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
+    async def fetch_deposits(self, code: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Transaction]:
         """
         fetch all deposits made to an account
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account009_deposit_list
         :param str code: unified currency code
         :param int [since]: the earliest time in ms to fetch deposits for
         :param int [limit]: the maximum number of deposits structures to retrieve
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `transaction structures <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         request = {}
         currency = None
         if code is not None:
-            self.load_markets()
+            await self.load_markets()
             currency = self.currency(code)
             request['coin_type'] = currency['id']
         if limit is not None:
             request['Limit'] = limit
-        response = self.v1PrivateGetBalanceCoinDeposit(self.extend(request, params))
+        response = await self.v1PrivateGetBalanceCoinDeposit(self.extend(request, params))
         #
         #    {
         #        "code": 0,
         #        "data": {
         #            "has_next": False,
         #            "curr_page": 1,
         #            "count": 1,
@@ -4842,28 +5088,28 @@
             'quoteRate': self.safe_number(quoteInfo, 'day_rate'),
             'period': 86400000,
             'timestamp': None,
             'datetime': None,
             'info': info,
         }
 
-    def fetch_isolated_borrow_rate(self, symbol: str, params={}):
+    async def fetch_isolated_borrow_rate(self, symbol: str, params={}):
         """
         fetch the rate of interest to borrow a currency for margin trading
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account007_margin_account_settings
         :param str symbol: unified symbol of the market to fetch the borrow rate for
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: an `isolated borrow rate structure <https://docs.ccxt.com/#/?id=isolated-borrow-rate-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         request = {
             'market': market['id'],
         }
-        response = self.v1PrivateGetMarginConfig(self.extend(request, params))
+        response = await self.v1PrivateGetMarginConfig(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "market": "BTCUSDT",
         #             "leverage": 10,
         #             "BTC": {
@@ -4879,23 +5125,23 @@
         #         },
         #         "message": "Success"
         #     }
         #
         data = self.safe_value(response, 'data', {})
         return self.parse_isolated_borrow_rate(data, market)
 
-    def fetch_isolated_borrow_rates(self, params={}):
+    async def fetch_isolated_borrow_rates(self, params={}):
         """
         fetch the borrow interest rates of all currencies
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account007_margin_account_settings
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a list of `isolated borrow rate structures <https://github.com/ccxt/ccxt/wiki/Manual#isolated-borrow-rate-structure>`
         """
-        self.load_markets()
-        response = self.v1PrivateGetMarginConfig(params)
+        await self.load_markets()
+        response = await self.v1PrivateGetMarginConfig(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "market": "BTCUSDT",
         #                 "leverage": 10,
@@ -4916,24 +5162,24 @@
         #
         data = self.safe_value(response, 'data', [])
         rates = []
         for i in range(0, len(data)):
             rates.append(self.parse_isolated_borrow_rate(data[i]))
         return rates
 
-    def fetch_borrow_interest(self, code: Str = None, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
-        self.load_markets()
+    async def fetch_borrow_interest(self, code: Str = None, symbol: Str = None, since: Int = None, limit: Int = None, params={}):
+        await self.load_markets()
         request = {}
         market = None
         if symbol is not None:
             market = self.market(symbol)
             request['market'] = market['id']
         if limit is not None:
             request['limit'] = limit
-        response = self.v1PrivateGetMarginLoanHistory(self.extend(request, params))
+        response = await self.v1PrivateGetMarginLoanHistory(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "page": 1,
         #             "limit": 10,
         #             "total": 1,
@@ -5000,33 +5246,33 @@
             'interestRate': self.safe_number(info, 'day_rate'),
             'amountBorrowed': self.parse_number(loanAmount),
             'timestamp': timestamp,  # expiry time
             'datetime': self.iso8601(timestamp),
             'info': info,
         }
 
-    def borrow_isolated_margin(self, symbol: str, code: str, amount: float, params={}):
+    async def borrow_isolated_margin(self, symbol: str, code: str, amount: float, params={}):
         """
         create a loan to borrow margin
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account017_margin_loan
         :param str symbol: unified market symbol, required for coinex
         :param str code: unified currency code of the currency to borrow
         :param float amount: the amount to borrow
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `margin loan structure <https://docs.ccxt.com/#/?id=margin-loan-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         currency = self.currency(code)
         request = {
             'market': market['id'],
             'coin_type': currency['id'],
             'amount': self.currency_to_precision(code, amount),
         }
-        response = self.v1PrivatePostMarginLoan(self.extend(request, params))
+        response = await self.v1PrivatePostMarginLoan(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": {
         #             "loan_id": 1670
         #         },
         #         "message": "Success"
@@ -5035,34 +5281,34 @@
         data = self.safe_value(response, 'data', {})
         transaction = self.parse_margin_loan(data, currency)
         return self.extend(transaction, {
             'amount': amount,
             'symbol': symbol,
         })
 
-    def repay_isolated_margin(self, symbol: str, code: str, amount, params={}):
+    async def repay_isolated_margin(self, symbol: str, code: str, amount, params={}):
         """
         repay borrowed margin and interest
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account018_margin_flat
         :param str symbol: unified market symbol, required for coinex
         :param str code: unified currency code of the currency to repay
         :param float amount: the amount to repay
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.loan_id]: extra parameter that is not required
         :returns dict: a `margin loan structure <https://docs.ccxt.com/#/?id=margin-loan-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         currency = self.currency(code)
         request = {
             'market': market['id'],
             'coin_type': currency['id'],
             'amount': self.currency_to_precision(code, amount),
         }
-        response = self.v1PrivatePostMarginFlat(self.extend(request, params))
+        response = await self.v1PrivatePostMarginFlat(self.extend(request, params))
         #
         #     {
         #         "code": 0,
         #         "data": null,
         #         "message": "Success"
         #     }
         #
@@ -5094,29 +5340,29 @@
             'amount': None,
             'symbol': None,
             'timestamp': None,
             'datetime': None,
             'info': info,
         }
 
-    def fetch_deposit_withdraw_fees(self, codes: Strings = None, params={}):
+    async def fetch_deposit_withdraw_fees(self, codes: Strings = None, params={}):
         """
         fetch deposit and withdraw fees
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot001_market010_asset_config
         :param str[]|None codes: list of unified currency codes
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict[]: a list of `fees structures <https://docs.ccxt.com/#/?id=fee-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         request = {}
         if codes is not None:
             codesLength = len(codes)
             if codesLength == 1:
                 request['coin_type'] = self.safe_value(codes, 0)
-        response = self.v1PublicGetCommonAssetConfig(self.extend(request, params))
+        response = await self.v1PublicGetCommonAssetConfig(self.extend(request, params))
         #
         #    {
         #        "code": 0,
         #        "data": {
         #            "CET-CSC": {
         #                "asset": "CET",
         #                "chain": "CSC",
@@ -5180,33 +5426,33 @@
         depositWithdrawCodes = list(depositWithdrawFees.keys())
         for i in range(0, len(depositWithdrawCodes)):
             code = depositWithdrawCodes[i]
             currency = self.currency(code)
             depositWithdrawFees[code] = self.assign_default_deposit_withdraw_fees(depositWithdrawFees[code], currency)
         return depositWithdrawFees
 
-    def fetch_leverages(self, symbols: List[str] = None, params={}) -> Leverages:
+    async def fetch_leverages(self, symbols: List[str] = None, params={}) -> Leverages:
         """
         fetch the set leverage for all contract and margin markets
         :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account007_margin_account_settings
         :param str[] [symbols]: a list of unified market symbols
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a list of `leverage structures <https://docs.ccxt.com/#/?id=leverage-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         symbols = self.market_symbols(symbols)
         market = None
         if symbols is not None:
             symbol = self.safe_value(symbols, 0)
             market = self.market(symbol)
         marketType = None
         marketType, params = self.handle_market_type_and_params('fetchLeverages', market, params)
         if marketType != 'spot':
             raise NotSupported(self.id + ' fetchLeverages() supports spot margin markets only')
-        response = self.v1PrivateGetMarginConfig(params)
+        response = await self.v1PrivateGetMarginConfig(params)
         #
         #     {
         #         "code": 0,
         #         "data": [
         #             {
         #                 "market": "BTCUSDT",
         #                 "leverage": 10,
@@ -5235,37 +5481,37 @@
             'info': leverage,
             'symbol': self.safe_symbol(marketId, market, None, 'spot'),
             'marginMode': None,
             'longLeverage': leverageValue,
             'shortLeverage': leverageValue,
         }
 
-    def fetch_position_history(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> Position:
+    async def fetch_position_history(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> Position:
         """
         fetches historical positions
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http033-0_finished_position
         :param str symbol: unified contract symbol
         :param int [since]: not used by coinex fetchPositionHistory
         :param int [limit]: the maximum amount of records to fetch, default=1000
         :param dict params: extra parameters specific to the exchange api endpoint
          *
          * EXCHANGE SPECIFIC PARAMETERS
         :param int [params.side]: 0: all 1: sell, 2: buy
         :returns dict[]: a list of `position structures <https://docs.ccxt.com/#/?id=position-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         market = self.market(symbol)
         if limit is None:
             limit = 1000
         request = {
             'market': market['id'],
             'side': 0,
             'limit': limit,
         }
-        response = self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
+        response = await self.v1PerpetualPrivateGetPositionFinished(self.extend(request, params))
         #
         #    {
         #        code: '0',
         #        data: {
         #            limit: '1000',
         #            offset: '0',
         #            records: [
@@ -5399,28 +5645,29 @@
                 else:
                     body = self.json(query)
             elif version == 'v2':
                 self.check_required_credentials()
                 query = self.keysort(query)
                 urlencoded = self.rawencode(query)
                 preparedString = method + '/' + version + '/' + path
-                if urlencoded:
+                if method == 'POST':
+                    body = self.json(query)
+                    preparedString += body
+                elif urlencoded:
                     preparedString += '?' + urlencoded
                 preparedString += nonce + self.secret
                 signature = self.hash(self.encode(preparedString), 'sha256')
                 headers = {
                     'X-COINEX-KEY': self.apiKey,
                     'X-COINEX-SIGN': signature,
                     'X-COINEX-TIMESTAMP': nonce,
                 }
-                if (method == 'GET') or (method == 'DELETE') or (method == 'PUT'):
+                if method != 'POST':
                     if urlencoded:
                         url += '?' + urlencoded
-                else:
-                    body = self.json(query)
         return {'url': url, 'method': method, 'body': body, 'headers': headers}
 
     def handle_errors(self, httpCode, reason, url, method, headers, body, response, requestHeaders, requestBody):
         if response is None:
             return None
         code = self.safe_string(response, 'code')
         data = self.safe_value(response, 'data')
@@ -5428,30 +5675,30 @@
         if (code != '0') or ((message != 'Success') and (message != 'Succeeded') and (message != 'Ok') and not data):
             feedback = self.id + ' ' + message
             self.throw_broadly_matched_exception(self.exceptions['broad'], message, feedback)
             self.throw_exactly_matched_exception(self.exceptions['exact'], code, feedback)
             raise ExchangeError(feedback)
         return None
 
-    def fetch_margin_adjustment_history(self, symbol: Str = None, type: Str = None, since: Num = None, limit: Num = None, params={}) -> List[MarginModification]:
+    async def fetch_margin_adjustment_history(self, symbol: Str = None, type: Str = None, since: Num = None, limit: Num = None, params={}) -> List[MarginModification]:
         """
         fetches the history of margin added or reduced from contract isolated positions
         :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http046_position_margin_history
         :param str [symbol]: unified market symbol
         :param str [type]: not used by coinex fetchMarginAdjustmentHistory
         :param int [since]: timestamp in ms of the earliest change to fetch
         :param int [limit]: the maximum amount of changes to fetch, default=100, max=100
         :param dict params: extra parameters specific to the exchange api endpoint
         :param int [params.until]: timestamp in ms of the latest change to fetch
          *
          * EXCHANGE SPECIFIC PARAMETERS
         :param int [params.offset]: offset
         :returns dict[]: a list of `margin structures <https://docs.ccxt.com/#/?id=margin-loan-structure>`
         """
-        self.load_markets()
+        await self.load_markets()
         until = self.safe_integer(params, 'until')
         params = self.omit(params, 'until')
         if limit is None:
             limit = 100
         request = {
             'market': '',
             'position_id': 0,
@@ -5461,15 +5708,15 @@
         if symbol is not None:
             market = self.market(symbol)
             request['market'] = market['id']
         if since is not None:
             request['start_time'] = since
         if until is not None:
             request['end_time'] = until
-        response = self.v1PerpetualPrivateGetPositionMarginHistory(self.extend(request, params))
+        response = await self.v1PerpetualPrivateGetPositionMarginHistory(self.extend(request, params))
         #
         #    {
         #        code: '0',
         #        data: {
         #            limit: '100',
         #            offset: '0',
         #            records: [
```

### Comparing `ccxt-4.3.8/ccxt/coinlist.py` & `ccxt-4.3.9/ccxt/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinmate.py` & `ccxt-4.3.9/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinmetro.py` & `ccxt-4.3.9/ccxt/coinmetro.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
                         'exchange/book/{pair}': 3,
                         'exchange/bookUpdates/{pair}/{from}': 1,  # not unified
                     },
                 },
                 'private': {
                     'get': {
                         'users/balances': 1,
+                        'users/wallets': 1,
                         'users/wallets/history/{since}': 1.67,
                         'exchange/orders/status/{orderID}': 1,
                         'exchange/orders/active': 1,
                         'exchange/orders/history/{since}': 1.67,
                         'exchange/fills/{since}': 1.67,
                         'exchange/margin': 1,  # not unified
                     },
@@ -906,57 +907,56 @@
             'quoteVolume': None,
             'info': ticker,
         }, market)
 
     def fetch_balance(self, params={}) -> Balances:
         """
         query for balance and get the amount of funds available for trading or funds locked in orders
-        :see: https://documenter.getpostman.com/view/3653795/SVfWN6KS#698ae067-43dd-4e19-a0ac-d9ba91381816
+        :see: https://documenter.getpostman.com/view/3653795/SVfWN6KS#741a1dcc-7307-40d0-acca-28d003d1506a
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :returns dict: a `balance structure <https://docs.ccxt.com/#/?id=balance-structure>`
         """
         self.load_markets()
-        response = self.privateGetUsersBalances(params)
-        return self.parse_balance(response)
+        response = self.privateGetUsersWallets(params)
+        list = self.safe_list(response, 'list', [])
+        return self.parse_balance(list)
 
-    def parse_balance(self, response) -> Balances:
+    def parse_balance(self, balances) -> Balances:
         #
-        #     {
-        #         "USDC": {
-        #             "USDC": 99,
-        #             "EUR": 91.16,
-        #             "BTC": 0.002334
-        #         },
-        #         "XCM": {
-        #             "XCM": 0,
-        #             "EUR": 0,
-        #             "BTC": 0
-        #         },
-        #         "TOTAL": {
-        #             "EUR": 91.16,
-        #             "BTC": 0.002334
+        #     [
+        #         {
+        #             "xcmLocks": [],
+        #             "xcmLockAmounts": [],
+        #             "refList": [],
+        #             "balanceHistory": [],
+        #             "_id": "5fecd3c998e75c2e4d63f7c3",
+        #             "currency": "BTC",
+        #             "label": "BTC",
+        #             "userId": "5fecd3c97fbfed1521db23bd",
+        #             "__v": 0,
+        #             "balance": 0.5,
+        #             "createdAt": "2020-12-30T19:23:53.646Z",
+        #             "disabled": False,
+        #             "updatedAt": "2020-12-30T19:23:53.653Z",
+        #             "reserved": 0,
+        #             "id": "5fecd3c998e75c2e4d63f7c3"
         #         },
-        #         "REF": {
-        #             "XCM": 0,
-        #             "EUR": 0,
-        #             "BTC": 0
-        #         }
-        #     }
+        #         ...
+        #     ]
         #
         result = {
-            'info': response,
+            'info': balances,
         }
-        balances = self.omit(response, ['TOTAL', 'REF'])
-        currencyIds = list(balances.keys())
-        for i in range(0, len(currencyIds)):
-            currencyId = currencyIds[i]
+        for i in range(0, len(balances)):
+            balanceEntry = self.safe_dict(balances, i, {})
+            currencyId = self.safe_string(balanceEntry, 'currency')
             code = self.safe_currency_code(currencyId)
             account = self.account()
-            currency = self.safe_value(balances, currencyId, {})
-            account['total'] = self.safe_string(currency, currencyId)
+            account['total'] = self.safe_string(balanceEntry, 'balance')
+            account['used'] = self.safe_string(balanceEntry, 'reserved')
             result[code] = account
         return self.safe_balance(result)
 
     def fetch_ledger(self, code: Str = None, since: Int = None, limit: Int = None, params={}):
         """
         fetch the history of changes, actions done by the user or operations that altered balance of the user
         :see: https://documenter.getpostman.com/view/3653795/SVfWN6KS#4e7831f7-a0e7-4c3e-9336-1d0e5dcb15cf
```

### Comparing `ccxt-4.3.8/ccxt/coinone.py` & `ccxt-4.3.9/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinsph.py` & `ccxt-4.3.9/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/coinspot.py` & `ccxt-4.3.9/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/cryptocom.py` & `ccxt-4.3.9/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/currencycom.py` & `ccxt-4.3.9/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/delta.py` & `ccxt-4.3.9/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/deribit.py` & `ccxt-4.3.9/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/digifinex.py` & `ccxt-4.3.9/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/exmo.py` & `ccxt-4.3.9/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/flowbtc.py` & `ccxt-4.3.9/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/fmfwio.py` & `ccxt-4.3.9/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/gate.py` & `ccxt-4.3.9/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/gemini.py` & `ccxt-4.3.9/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/hitbtc.py` & `ccxt-4.3.9/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/hollaex.py` & `ccxt-4.3.9/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/htx.py` & `ccxt-4.3.9/ccxt/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/huobijp.py` & `ccxt-4.3.9/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/hyperliquid.py` & `ccxt-4.3.9/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/idex.py` & `ccxt-4.3.9/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/independentreserve.py` & `ccxt-4.3.9/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/indodax.py` & `ccxt-4.3.9/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/kraken.py` & `ccxt-4.3.9/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/krakenfutures.py` & `ccxt-4.3.9/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/kucoin.py` & `ccxt-4.3.9/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/kucoinfutures.py` & `ccxt-4.3.9/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/kuna.py` & `ccxt-4.3.9/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/latoken.py` & `ccxt-4.3.9/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/lbank.py` & `ccxt-4.3.9/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/luno.py` & `ccxt-4.3.9/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/lykke.py` & `ccxt-4.3.9/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/mercado.py` & `ccxt-4.3.9/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/mexc.py` & `ccxt-4.3.9/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/ndax.py` & `ccxt-4.3.9/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/novadax.py` & `ccxt-4.3.9/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/oceanex.py` & `ccxt-4.3.9/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/okcoin.py` & `ccxt-4.3.9/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/okx.py` & `ccxt-4.3.9/ccxt/okx.py`

 * *Files 0% similar despite different names*

```diff
@@ -2543,14 +2543,16 @@
         clientOrderId = self.safe_string_2(params, 'clOrdId', 'clientOrderId')
         stopLoss = self.safe_value(params, 'stopLoss')
         stopLossDefined = (stopLoss is not None)
         takeProfit = self.safe_value(params, 'takeProfit')
         takeProfitDefined = (takeProfit is not None)
         trailingPercent = self.safe_string_2(params, 'trailingPercent', 'callbackRatio')
         isTrailingPercentOrder = trailingPercent is not None
+        trigger = (triggerPrice is not None) or (type == 'trigger')
+        isReduceOnly = self.safe_value(params, 'reduceOnly', False)
         defaultMarginMode = self.safe_string_2(self.options, 'defaultMarginMode', 'marginMode', 'cross')
         marginMode = self.safe_string_2(params, 'marginMode', 'tdMode')  # cross or isolated, tdMode not ommited so be extended into the request
         margin = False
         if (marginMode is not None) and (marginMode != 'cash'):
             margin = True
         else:
             marginMode = defaultMarginMode
@@ -2564,22 +2566,35 @@
             request['tdMode'] = tradeMode
         elif contract:
             if market['swap'] or market['future']:
                 positionSide = None
                 positionSide, params = self.handle_option_and_params(params, 'createOrder', 'positionSide')
                 if positionSide is not None:
                     request['posSide'] = positionSide
+                else:
+                    hedged = None
+                    hedged, params = self.handle_option_and_params(params, 'createOrder', 'hedged')
+                    if hedged:
+                        isBuy = (side == 'buy')
+                        isProtective = (takeProfitPrice is not None) or (stopLossPrice is not None) or isReduceOnly
+                        if isProtective:
+                            # in case of protective orders, the posSide should be opposite of position side
+                            # reduceOnly is emulated and not natively supported by the exchange
+                            request['posSide'] = 'short' if isBuy else 'long'
+                            if isReduceOnly:
+                                params = self.omit(params, 'reduceOnly')
+                        else:
+                            request['posSide'] = 'long' if isBuy else 'short'
             request['tdMode'] = marginMode
         isMarketOrder = type == 'market'
         postOnly = False
         postOnly, params = self.handle_post_only(isMarketOrder, type == 'post_only', params)
         params = self.omit(params, ['currency', 'ccy', 'marginMode', 'timeInForce', 'stopPrice', 'triggerPrice', 'clientOrderId', 'stopLossPrice', 'takeProfitPrice', 'slOrdPx', 'tpOrdPx', 'margin', 'stopLoss', 'takeProfit', 'trailingPercent'])
         ioc = (timeInForce == 'IOC') or (type == 'ioc')
         fok = (timeInForce == 'FOK') or (type == 'fok')
-        trigger = (triggerPrice is not None) or (type == 'trigger')
         conditional = (stopLossPrice is not None) or (takeProfitPrice is not None) or (type == 'conditional')
         marketIOC = (isMarketOrder and ioc) or (type == 'optimal_limit_ioc')
         defaultTgtCcy = self.safe_string(self.options, 'tgtCcy', 'base_ccy')
         tgtCcy = self.safe_string(params, 'tgtCcy', defaultTgtCcy)
         if (not contract) and (not margin):
             request['tgtCcy'] = tgtCcy
         if isMarketOrder or marketIOC:
@@ -2730,14 +2745,15 @@
         :param dict [params.stopLoss]: *stopLoss object in params* containing the triggerPrice at which the attached stop loss order will be triggered(perpetual swap markets only)
         :param float [params.stopLoss.triggerPrice]: stop loss trigger price
         :param float [params.stopLoss.price]: used for stop loss limit orders, not used for stop loss market price orders
         :param str [params.stopLoss.type]: 'market' or 'limit' used to specify the stop loss price type
         :param str [params.positionSide]: if position mode is one-way: set to 'net', if position mode is hedge-mode: set to 'long' or 'short'
         :param str [params.trailingPercent]: the percent to trail away from the current market price
         :param str [params.tpOrdKind]: 'condition' or 'limit', the default is 'condition'
+        :param str [params.hedged]: True/false, to automatically set exchange-specific params needed when trading in hedge mode
         :returns dict: an `order structure <https://docs.ccxt.com/#/?id=order-structure>`
         """
         self.load_markets()
         market = self.market(symbol)
         request = self.create_order_request(symbol, type, side, amount, price, params)
         method = self.safe_string(self.options, 'createOrder', 'privatePostTradeBatchOrders')
         requestOrdType = self.safe_string(request, 'ordType')
@@ -5847,14 +5863,44 @@
         #         }
         #       ],
         #       "msg": ""
         #     }
         #
         return response
 
+    def fetch_position_mode(self, symbol: Str = None, params={}):
+        """
+        :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-get-account-configuration
+        fetchs the position mode, hedged or one way, hedged for binance is set identically for all linear markets or all inverse markets
+        :param str symbol: unified symbol of the market to fetch the order book for
+        :param dict [params]: extra parameters specific to the exchange API endpoint
+        :param str [param.accountId]: if you have multiple accounts, you must specify the account id to fetch the position mode
+        :returns dict: an object detailing whether the market is in hedged or one-way mode
+        """
+        accounts = self.fetch_accounts()
+        length = len(accounts)
+        selectedAccount = None
+        if length > 1:
+            accountId = self.safe_string(params, 'accountId')
+            if accountId is None:
+                accountIds = self.get_list_from_object_values(accounts, 'id')
+                raise ExchangeError(self.id + ' fetchPositionMode() can not detect position mode, because you have multiple accounts. Set params["accountId"] to desired id from: ' + ', '.join(accountIds))
+            else:
+                accountsById = self.index_by(accounts, 'id')
+                selectedAccount = self.safe_dict(accountsById, accountId)
+        else:
+            selectedAccount = accounts[0]
+        mainAccount = selectedAccount['info']
+        posMode = self.safe_string(mainAccount, 'posMode')  # long_short_mode, net_mode
+        isHedged = posMode == 'long_short_mode'
+        return {
+            'info': mainAccount,
+            'hedged': isHedged,
+        }
+
     def set_position_mode(self, hedged: bool, symbol: Str = None, params={}):
         """
         set hedged to True or False for a market
         :see: https://www.okx.com/docs-v5/en/#trading-account-rest-api-set-position-mode
         :param bool hedged: set to True to use long_short_mode, False for net_mode
         :param str symbol: not used by okx setPositionMode
         :param dict [params]: extra parameters specific to the exchange API endpoint
```

### Comparing `ccxt-4.3.8/ccxt/onetrading.py` & `ccxt-4.3.9/ccxt/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/p2b.py` & `ccxt-4.3.9/ccxt/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/paymium.py` & `ccxt-4.3.9/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/phemex.py` & `ccxt-4.3.9/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/poloniex.py` & `ccxt-4.3.9/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/poloniexfutures.py` & `ccxt-4.3.9/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/__init__.py` & `ccxt-4.3.9/ccxt/pro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.3.8'
+__version__ = '4.3.9'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-4.3.8/ccxt/pro/alpaca.py` & `ccxt-4.3.9/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/ascendex.py` & `ccxt-4.3.9/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bequant.py` & `ccxt-4.3.9/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/binance.py` & `ccxt-4.3.9/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/binancecoinm.py` & `ccxt-4.3.9/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/binanceus.py` & `ccxt-4.3.9/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/binanceusdm.py` & `ccxt-4.3.9/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bingx.py` & `ccxt-4.3.9/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitcoincom.py` & `ccxt-4.3.9/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitfinex.py` & `ccxt-4.3.9/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitfinex2.py` & `ccxt-4.3.9/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitget.py` & `ccxt-4.3.9/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bithumb.py` & `ccxt-4.3.9/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitmart.py` & `ccxt-4.3.9/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitmex.py` & `ccxt-4.3.9/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitopro.py` & `ccxt-4.3.9/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitrue.py` & `ccxt-4.3.9/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitstamp.py` & `ccxt-4.3.9/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bitvavo.py` & `ccxt-4.3.9/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/blockchaincom.py` & `ccxt-4.3.9/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/bybit.py` & `ccxt-4.3.9/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/cex.py` & `ccxt-4.3.9/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/coinbase.py` & `ccxt-4.3.9/ccxt/pro/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/coinbaseinternational.py` & `ccxt-4.3.9/ccxt/pro/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/coinbasepro.py` & `ccxt-4.3.9/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/coincheck.py` & `ccxt-4.3.9/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/coinex.py` & `ccxt-4.3.9/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/coinone.py` & `ccxt-4.3.9/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/cryptocom.py` & `ccxt-4.3.9/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/currencycom.py` & `ccxt-4.3.9/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/deribit.py` & `ccxt-4.3.9/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/exmo.py` & `ccxt-4.3.9/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/gate.py` & `ccxt-4.3.9/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/gemini.py` & `ccxt-4.3.9/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/hitbtc.py` & `ccxt-4.3.9/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/hollaex.py` & `ccxt-4.3.9/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/htx.py` & `ccxt-4.3.9/ccxt/pro/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/huobijp.py` & `ccxt-4.3.9/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/hyperliquid.py` & `ccxt-4.3.9/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/idex.py` & `ccxt-4.3.9/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/independentreserve.py` & `ccxt-4.3.9/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/kraken.py` & `ccxt-4.3.9/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/krakenfutures.py` & `ccxt-4.3.9/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/kucoin.py` & `ccxt-4.3.9/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/kucoinfutures.py` & `ccxt-4.3.9/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/lbank.py` & `ccxt-4.3.9/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/luno.py` & `ccxt-4.3.9/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/mexc.py` & `ccxt-4.3.9/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/ndax.py` & `ccxt-4.3.9/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/okcoin.py` & `ccxt-4.3.9/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/okx.py` & `ccxt-4.3.9/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/onetrading.py` & `ccxt-4.3.9/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/p2b.py` & `ccxt-4.3.9/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/phemex.py` & `ccxt-4.3.9/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/poloniex.py` & `ccxt-4.3.9/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/poloniexfutures.py` & `ccxt-4.3.9/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/probit.py` & `ccxt-4.3.9/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/upbit.py` & `ccxt-4.3.9/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/wazirx.py` & `ccxt-4.3.9/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/whitebit.py` & `ccxt-4.3.9/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/pro/woo.py` & `ccxt-4.3.9/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/probit.py` & `ccxt-4.3.9/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-4.3.9/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-4.3.9/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-4.3.9/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-4.3.9/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-4.3.9/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-4.3.9/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-4.3.9/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-4.3.9/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-4.3.9/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-4.3.9/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-4.3.9/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-4.3.9/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/_version.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-4.3.9/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/__init__.py` & `ccxt-4.3.9/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_account.py` & `ccxt-4.3.9/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_balance.py` & `ccxt-4.3.9/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_borrow_interest.py` & `ccxt-4.3.9/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_borrow_rate.py` & `ccxt-4.3.9/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_calculate_fee.py` & `ccxt-4.3.9/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_crypto.py` & `ccxt-4.3.9/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_currency.py` & `ccxt-4.3.9/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_datetime.py` & `ccxt-4.3.9/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-4.3.9/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_deep_extend.py` & `ccxt-4.3.9/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-4.3.9/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-4.3.9/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_funding_rate_history.py` & `ccxt-4.3.9/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_last_price.py` & `ccxt-4.3.9/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_ledger_entry.py` & `ccxt-4.3.9/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_ledger_item.py` & `ccxt-4.3.9/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_leverage_tier.py` & `ccxt-4.3.9/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_margin_mode.py` & `ccxt-4.3.9/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_margin_modification.py` & `ccxt-4.3.9/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_market.py` & `ccxt-4.3.9/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_number.py` & `ccxt-4.3.9/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_ohlcv.py` & `ccxt-4.3.9/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_open_interest.py` & `ccxt-4.3.9/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_order.py` & `ccxt-4.3.9/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_order_book.py` & `ccxt-4.3.9/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_position.py` & `ccxt-4.3.9/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_shared_methods.py` & `ccxt-4.3.9/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_status.py` & `ccxt-4.3.9/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_throttle.py` & `ccxt-4.3.9/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_ticker.py` & `ccxt-4.3.9/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_trade.py` & `ccxt-4.3.9/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_trading_fee.py` & `ccxt-4.3.9/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/base/test_transaction.py` & `ccxt-4.3.9/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/test_async.py` & `ccxt-4.3.9/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/test/test_sync.py` & `ccxt-4.3.9/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/timex.py` & `ccxt-4.3.9/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/tokocrypto.py` & `ccxt-4.3.9/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/tradeogre.py` & `ccxt-4.3.9/ccxt/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/upbit.py` & `ccxt-4.3.9/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/wavesexchange.py` & `ccxt-4.3.9/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/wazirx.py` & `ccxt-4.3.9/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/whitebit.py` & `ccxt-4.3.9/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/woo.py` & `ccxt-4.3.9/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/yobit.py` & `ccxt-4.3.9/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/zaif.py` & `ccxt-4.3.9/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt/zonda.py` & `ccxt-4.3.9/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/ccxt.egg-info/PKG-INFO` & `ccxt-4.3.9/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.3.8
+Version: 4.3.9
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -222,21 +222,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.3.8/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.9/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.3.9/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.9/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.3.8/ccxt.egg-info/SOURCES.txt` & `ccxt-4.3.9/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.8/package.json` & `ccxt-4.3.9/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975308046509235%*

 * *Differences: {"'devDependencies'": "{'tsx': '^4.7.2', delete: ['ts-node']}",*

 * * "'scripts'": "{'transpileCS': 'tsx build/csharpTranspiler.ts --multi', 'transpileCSWs': 'tsx "*

 * *              "build/csharpTranspiler.ts --ws', 'cli.ts': 'tsx examples/ts/cli.ts', "*

 * *              "'validate-types': 'tsx build/validate-types.ts', 'benchmark': 'tsx "*

 * *              "examples/ts/benchmark.ts'}",*

 * * "'version'": "'4.3.9'"}*

```diff
@@ -42,15 +42,15 @@
         "ololog": "1.1.155",
         "piscina": "^3.2.0",
         "replace-in-file": "^6.3.5",
         "rollup": "^2.70.1",
         "rollup-plugin-execute": "1.1.1",
         "terser-webpack-plugin": "^5.3.9",
         "ts-loader": "^9.4.2",
-        "ts-node": "^10.9.1",
+        "tsx": "^4.7.2",
         "typescript": "4.7.4",
         "webpack": "^5.76.2",
         "webpack-cli": "^5.0.1"
     },
     "engines": {
         "node": ">=15.0.0"
     },
@@ -148,15 +148,15 @@
     },
     "readme": "README.md",
     "repository": {
         "type": "git",
         "url": "https://github.com/ccxt/ccxt.git"
     },
     "scripts": {
-        "benchmark": "node --loader ts-node/esm examples/ts/benchmark.ts",
+        "benchmark": "tsx examples/ts/benchmark.ts",
         "build": "npm run pre-transpile && npm run transpile && npm run post-transpile && npm run update-badges && npm run build-docs",
         "build-docs": "node jsdoc2md.js && node examples2md.js",
         "buildCS": "dotnet build cs/ccxt.sln",
         "buildCSRelease": "dotnet build cs --configuration Release",
         "bundle": "npm run bundle-cjs && npm run bundle-browser",
         "bundle-browser": "webpack build -c webpack.config.js && webpack build -c webpack.config.js --optimization-minimize --output-filename ccxt.browser.min.js",
         "bundle-cjs": "rollup -c rollup.config.js",
@@ -168,15 +168,15 @@
         "check-rest-php-syntax": "php -f php/test/custom/syntax.php",
         "check-syntax": "npm run transpile && npm run check-js-syntax && npm run check-python-syntax && npm run check-php-syntax",
         "check-ws-php-syntax": "php -f php/pro/test/custom/syntax.php",
         "cli.cs": "dotnet run --project \"./cs/cli/cli.csproj\"",
         "cli.js": "node ./examples/js/cli.js",
         "cli.php": "php ./examples/php/cli.php",
         "cli.py": "python3 ./examples/py/cli.py",
-        "cli.ts": "node --loader ts-node/esm examples/ts/cli.ts",
+        "cli.ts": "tsx examples/ts/cli.ts",
         "commonjs-test": "node test-commonjs.cjs",
         "copy-python-files": "npm run copy-python-package && npm run copy-python-license && npm run copy-python-keys && npm run copy-python-readme",
         "copy-python-keys": "node build/copy keys.json python/keys.json",
         "copy-python-license": "node build/copy LICENSE.txt python/LICENSE.txt",
         "copy-python-package": "node build/copy package.json python/package.json",
         "copy-python-readme": "node build/copy README.md python/README.md",
         "coverage-js": "npm run instrument && npm run nyc-coverage && rm -rf jsInstrumented",
@@ -251,24 +251,24 @@
         "test-python-base-ws": "npm run test-python-cache && npm run test-python-orderbook",
         "test-python-cache": "python python/ccxt/pro/test/base/test_cache.py",
         "test-python-orderbook": "python python/ccxt/pro/test/base/test_order_book.py",
         "test-ws": "npm run build && node run-tests --ws --useProxy",
         "test-ws-cs-base": "npm run test-cs-cache && npm run test-cs-orderbook",
         "test-ws-php-base": "npm run test-php-cache && npm run test-php-orderbook",
         "transpile": "npm run transpileRest && npm run transpileWs",
-        "transpileCS": "node --no-warnings --loader ts-node/esm build/csharpTranspiler.ts --multi",
-        "transpileCSWs": "node --no-warnings --loader ts-node/esm build/csharpTranspiler.ts --ws",
+        "transpileCS": "tsx build/csharpTranspiler.ts --multi",
+        "transpileCSWs": "tsx build/csharpTranspiler.ts --ws",
         "transpileRest": "node build/transpile",
         "transpileWs": "node build/transpileWS",
         "tsBuild": "tsc || echo \"\"",
         "tsBuildExamples": "tsc -p ./examples/tsconfig.json",
         "tsBuildFile": "tsc --skipLibCheck --strictNullChecks false --strict --noImplicitAny false --esModuleInterop --isolatedModules false --forceConsistentCasingInFileNames --removeComments false --target ES2020 --declaration --allowJs --checkJs false --moduleResolution Node --module ES2022 --outDir ./js/src --lib ES2020.BigInt --lib dom ",
         "update-badges": "node build/update-badges",
         "update-links": "node build/update-links",
-        "validate-types": "node --loader ts-node/esm build/validate-types.ts",
+        "validate-types": "tsx build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.3.8"
+    "version": "4.3.9"
 }
```

### Comparing `ccxt-4.3.8/setup.py` & `ccxt-4.3.9/setup.py`

 * *Files identical despite different names*

