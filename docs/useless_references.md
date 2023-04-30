# 役に立たなかった参照

# nmake

* `nmake` がほしい（XLAモジュールのインストール時に要求される）
  * Visual Studio 2022 をインストールする
  * そのフォルダー内を `nmake` で検索する
  * `nmake` が入っている `bin` フォルダーを、環境変数の `PATH` に追加する
  * Visual Studio Code を再起動すると、ターミナルで `nmake` コマンドが認識される

```plaintext
# Visual C++ Build Tools を AMD のCPUで使うための設定
"C:\Program Files (x86)\Microsoft Visual Studio\2022\BuildTools\VC\Auxiliary\Build\vcvarsall.bat" amd64
```
