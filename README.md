next.jsをチュートリアルからやってみる


This is a starter template for [Learn Next.js](https://nextjs.org/learn).

* Dynamic Routes,API Routes

1. `pages/posts`配下に`[id].js`ファイルを作成。これにより動的にページが返される仕組み。
1. libにpostsの中のデータ(今回はmdファイル)をparamsがキーとなるIDと名前のオブジェクトを返す関数`getAllPostIds()`を作成
1. `[id].js`のgetStaticPathsが作成した`getAllPostIds()`でオブジェクトを返す(Paths)。これによりどのパスでプレレンダリングされるか決定される
1. libにidによってファイルを指定して中身を読みだす`getPostData()`を作成
1. `[id].js`の`getStaticProps()`がIDに紐づくデータをフェッチ、propsとして返す