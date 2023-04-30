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
