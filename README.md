# README

# 概要
  MVCの基礎を学習。タイトルと本文、および画像の投稿ができるアプリ。<br>
  リンクタグがないため、直接urlを入力することでページ遷移。

## ルーティング一覧

  * get '/top' => 'root#top'
    top画面
  * get 'posts/new'
    新規投稿画面
  * post '/posts' => 'posts#create'
    投稿の記録
  * get '/posts' => 'posts#index'
    投稿一覧ページ
  * get '/posts/:id' => 'posts#show', as: 'post'
    投稿の詳細ページ
  * get '/posts/:id/edit' => 'posts#edit', as: 'edit_post'
    投稿の編集ページ
  * patch '/posts/:id' => 'posts#update', as: 'update_post'
    投稿編集の記録
  * delete '/posts/:id' => 'posts#destroy', as: 'destroy_post'
    投稿の削除

Things you may want to cover:

* Rails version
  Rails 5.2.0

