# forked tomk79/node-php-bin

## 変更箇所
- php5.6.18に変更
- phpのエクステンション追加
	- curl
	- tidy

### for Win
zipのバイナリからphp.iniを変更

### for Mac & Linux
- darwin版はソースからコンパイル

再コンパイルは（以前コンパイルしたものからオプションを変更してmakeする。）

```
$ cd src/php-5.6.18
$ ./config.nice
$ make && make install
```

備考：  
- "PDO および PDO_SQLITE ドライバは、PHP 5.1.0 以降デフォルトで有効"なので指定しない
- makeする時は、tidy-html5が入っている環境で実行する。
