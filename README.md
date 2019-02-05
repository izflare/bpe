# bpe text generator

### Description

BPE による単語分割テキスト生成器  
暫定版

### Download

```
git clone https://github.com/izflare/bpe.git
```

### Compile

tested under Linux compiling with rust (cargo) ver 1.32.0

```
cd bpe
cargo build --release
```

### Run

```
cd target/release
./bpe [OPTIONS] --input <input> 

OPTIONS:
	--size <size>
```

`<input>` は分かち書き＋前処理済みデータファイル（true）  
`<size>` は連結ペア数（指定なしの場合，デフォルト値の16000で回る）  
bpeテキストは `<input>.bpe` ファイルとして出力  
（分割された単語は abc → ab@@ c のように表記）


