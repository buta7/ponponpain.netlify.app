# README

## Setup

サイト作成

    $ npx gatsby new ponponpain.netlify.app https://github.com/LekoArts/gatsby-starter-portfolio-emma

サーバ起動

    $ cd ponponpain.netlify.app
    $ gatsby develop

## Netlifyとの連携

### Github側

"ponponpain.netlify.app"というレポジトリを作成(private)

リモートレポジトリの設定

    $ git remote add origin git@github.com:higebobo/ponponpain.netlify.app.git

コミット

    $ git add -A
    $ git commit -m 'init'
    $ git push -u origin master

### Netlify側

1. ログインしてNew site from Gitをクリック
2. Githubを選び上記"ponponpain.netlify.app"を選択
3. Build Commandなどはデフォルトのままで"Deploy Site"をクリックして作成
4. Githubのレポジトリにプッシュすれば自動的にビルド＆公開される

## Link

* [gatsby\-starter\-portfolio\-emma: Gatsby Starter \| GatsbyJS](https://www.gatsbyjs.org/starters/LekoArts/gatsby-starter-portfolio-emma/)
* [GatsbyとNetlifyで簡単にブログを作成 \- Qiita](https://qiita.com/k-penguin-sato/items/7554e5e7e90aa10ae225)
