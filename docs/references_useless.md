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

# Axon

📝 `mix.exs`:  

```elixir
  # ...
  defp deps do
    [
      # ...
      {:castore, "~> 1.0"},
      {:elixir_make, "~> 0.6"},
      {:nx, "~> 0.5.1"},
      {:telemetry, "~> 1.0"},
      {:xla, "~> 0.4.4"},
      {:exla, "~> 0.5.3"},
      {:axon, "~> 0.3"},
      {:table_rex, "~> 3.1"}
    ]
  end
```

```shell
cd example

set XLA_BUILD=true

# もし、掃除したいなら
mix deps.clean --all

# mix.exs ファイルの deps の設定にしたがって、モジュールを取得
mix deps.get

# コンパイルおよび実行
mix run
```

