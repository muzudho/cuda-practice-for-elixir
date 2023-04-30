# References

# Mix new projet

* 📖 [Elixir School](https://elixirschool.com/ja/lessons/basics/mix/)

```shell
mix new example
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
# C:\GitHub\cuda-practice-for-elixir>
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
