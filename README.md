# README

## Setup

サイト作成

    $ npx gatsby new ponponpain.netlify.app https://github.com/LekoArts/gatsby-starter-portfolio-emma

サーバ起動

    $ cd ponponpain.netlify.app
    $ gatsby develop

## Github pagesとの連携

gatsby-config.js(リンクのprefixを付加:githubのレポジトリ名に設定すること)

    ...
      pathPrefix: "/gatsby-mate",
    }

gatsby-config.js(上記prefixを付加してbuildしpublicディレクトリをgh-pagesブランチにプッシュ)

    ...
    "scripts": {
      ...
      "develop": "gatsby develop",
      "deploy": "gatsby build --prefix-paths && gh-pages -d public",
      "clean": "gatsby clean",
      ...

gh-pagesのインストール

    $ npm install gh-pages --save-dev

GithubにRepository"gatsby-mate"を作成後

    $ git remote add origin git@github.com:higebobo/gatsby-mate.git
    $ git add -A
    $ git commit -m 'init'
    $ git push -u origin master

デプロイ

    $ npx run deploy

## Link

* [higebobo/gatsby\-shopify](https://github.com/higebobo/gatsby-shopify/tree/master)
* [https://github\.com/EmaSuriano/gatsby\-starter\-mate](https://github.com/EmaSuriano/gatsby-starter-mate)
* [GatsbyとNetlifyで簡単にブログを作成 \- Qiita](https://qiita.com/k-penguin-sato/items/7554e5e7e90aa10ae225)
* [How Gatsby Works with GitHub Pages \| GatsbyJS](https://www.gatsbyjs.org/docs/how-gatsby-works-with-github-pages/)
* [Can I change build directory path from public to anything else? · Issue \#14703 · gatsbyjs/gatsby](https://github.com/gatsbyjs/gatsby/issues/14703)
