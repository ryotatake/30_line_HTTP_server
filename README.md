# 30_line_HTTP_server

[Building a 30 line HTTP server in Ruby | AppSignal Blog](https://blog.appsignal.com/2016/11/23/ruby-magic-building-a-30-line-http-server-in-ruby.html)で作成した、Rubyによるwebサーバーです。

## 使い方

### TCPサーバー

ターミナルを二つ立ち上げて、片方で
```bash
$ ruby tcp_server.rb
```
としてから、もう片方で
```bash
$ ruby tcp_client.rb
```
とすると、
```ruby
$ ruby tcp_client.rb
Hello world! The time is 2016-11-23 15:17:11 +0100
```
のように表示されます。


### HTTPサーバー

```bash
$ ruby http_server.rb
```
としてサーバーを起動してからブラウザで http://localhost:5678 にアクセスすると以下のような画面が表示されます。

![lobster](https://user-images.githubusercontent.com/39555429/55663818-9e72bb00-585e-11e9-8505-f774b07add86.JPG)

"flip!"をクリックしてロブスターの向きを変えたり、"crash!"をクリックしてエラーを起こすことが出来ます。
