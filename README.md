# cppdev
docker上にC++の開発環境を構築（gcc,g++）
以下の手順でコンテナを立ち上げる
cd cppdev

0. docker-compose build（こちらは最初の一回だけ行う）
1. docker-compose up -d（立ち上げ）

上記コマンドでコンテナが立ち上がる。

コンテナに入りたい時は以下のコマンドを実行する
docker exec -it cppdev bash（こちらのshellコマンドは任意）

コンテナ内でg++等でコンパイル、実行が可能になる
ex) g++ hello.cpp
    ./a.out

終了する時
2. docker-compose down


