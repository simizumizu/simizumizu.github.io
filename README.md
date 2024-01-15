# シミズミズDEVELOPER へようこそ！

このリポジトリは、枝水ミズのホームページです  
GitHub Actions で jekyll を使って、公開しています(^^)/  

## 環境構築 Windows11の場合

[こちら](https://docs.github.com/ja/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)や[こちら](https://jekyllrb-ja.github.io/docs/installation/windows/)を参考に、構築しました  

まずは、 [RubyInstaller Downloads](https://rubyinstaller.org/downloads/) からRuby+Devkitバージョンをダウンロードして、インストールしてください。インストールはデフォルトのオプションを使用してください。  

インストールウィザードの最後の段階で、 `ridk install` ステップを実行してください。  
カラフルな「Ruby Installer2」というターミナルが表示されるので、設定します  

ブログ用のリポジトリを作成してください  

```sh
> cd YOUR_DEV_DIR
> git clone YOUR_REPOSITORY
> cd YOUR_REPOSITORY_DIR
> gem install jekyll bundler
> jekyll -v
jekyll 4.3.3
> jekyll new --skip-bundle .
```

jekyll がインストールできたら、[こちら](https://docs.github.com/ja/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll) を参考にGemfileを更新します  
項番8, 9, 10をやっていきます  

```sh
> bundle install
> bundle exec jekyll serve
```

http://localhost:4000 をブラウザで見てみましょう  
表示されたら環境構築完了です  
