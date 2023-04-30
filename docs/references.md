# References

# Mix new projet

* 📖 [Elixir School](https://elixirschool.com/ja/lessons/basics/mix/)

```shell
mix new example
```

# MSYS2

```plaintext
Another option is to install the Linux compatiblity tools from [MSYS2](https://www.msys2.org/).

After installation start the msys64 bit terminal from the start menu and install the
C/C++ compiler toolchain. E.g.:

  pacman -S --noconfirm pacman-mirrors pkg-config
  pacman -S --noconfirm --needed base-devel autoconf automake make libtool git \
    mingw-w64-x86_64-toolchain mingw-w64-x86_64-openssl mingw-w64-x86_64-libtool

This will give you a compilation suite nearly compatible with Unix' standard tools.
```

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

# Livebook のインストール

* 📖 [Elixirで機械学習に初挑戦①：基礎知識とLivebook＋Nx＋Axonによる機械学習入門](https://qiita.com/piacerex/items/0871b54b41128d426da5)

👇 Linux  

```shell
mix escript.install hex livebook
echo 'export PATH=$HOME/.mix/escripts:$PATH' >> ~/.bashrc
source ~/.bashrc
livebook server
```

* 公式: 📖 [Livebook](https://livebook.dev/)
    * 📖 [Livebook Desktop install](https://livebook.dev/#install)
