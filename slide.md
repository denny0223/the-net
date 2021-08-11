title: The Net
output: index.html

--

<h1 style="font-size: 72px">
  HTTP、RESTful<br />
  觀念與實作<br />
</h1>
<br />

## Denny Huang

--

### Who am I ?

<br />
<h2 style="font-size: 60px">
  <b>Denny Huang</b>
</h2>

* SITCON 2013, 2014 總召

* Rayark Inc.

* <a href="https://denny.one/" target="_blank">About me</a>

--

# WSL

--

### Kenny Huang, Ph.D. 黃勝雄 博士

* <a href="https://www.slideshare.net/tahr1984/kenny-huang-phd" target="_blank">網路之根 – 基礎建設與標準化</a>


* <a href="https://www.youtube.com/watch?v=aa_DdMpNI5Q" target="_blank">SITCON 2017 - Cybersecurity and Internet Governance 網路安全與網路治理</a>

--

# [History of the Internet](https://zh.wikipedia.org/wiki/%E7%B6%B2%E9%9A%9B%E7%B6%B2%E8%B7%AF%E6%AD%B7%E5%8F%B2)

--

# <a href="https://zh.wikipedia.org/wiki/OSI%E6%A8%A1%E5%9E%8B" target="_blank">OSI</a>
## <a href="https://www.explainxkcd.com/wiki/index.php/1417:_Seven" target="_blank">7?</a>

--

# [IETF](https://zh.wikipedia.org/zh-tw/%E7%B6%B2%E9%9A%9B%E7%B6%B2%E8%B7%AF%E5%B7%A5%E7%A8%8B%E4%BB%BB%E5%8B%99%E7%B5%84)/[RFC](https://zh.wikipedia.org/wiki/RFC)
## [RFC 2324](https://tools.ietf.org/html/rfc2324)
## [RFC 2468](https://tools.ietf.org/html/rfc2468)

--

# Network Interface
## [Predictable Network Interface Names](https://www.freedesktop.org/wiki/Software/systemd/PredictableNetworkInterfaceNames/)

--

# Ask the man
## `man [command]`

--

# IP
## [Public IP / Private IP](https://datatracker.ietf.org/doc/html/rfc3330#section-3)
## `ip a`

--

# Port

--

# ARP
## `arp / ip neighbour`

--

# Gateway / Netmask
## `ip route / route / traceroute / mtr`

--

# <a href="https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE" target="_blank">TCP</a> / <a href="https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE" target="_blank">UDP</a>
## `nc -lvp [port] / nc -v [hostname/ip] [port]`
## `nc -lvup [port] / nc -vu [hostname/ip] [port]`

--

# Three-Way Handshake
## `tcpdump -X host [ip]`

--

# <a href="https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE" target="_blank">DNS</a>
## `dig / nslookup`

--

# HTTP
## [request method](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods) / [status code](https://http.cat) / [headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)

--

### Response a web page

#### Server
`nc -lvp 8000`
```
HTTP/1.1 200 OK[Enter]
[Enter]
Hello
^C
```
#### Clint
- Browser
- `curl -v localhost:8000`

--

### Python 3 HTTP Server

#### Start Server
`python3 -m http.server`

#### Request with
- `nc -v 0 8000`
	- `GET / HTTP/1.1`
- `curl -v localhost:8000`
- Browser

--

# HTTPS

--

# Cookie / Session

--

# [How Browsers Work?](https://github.com/alex/what-happens-when)

--

# API
## Application Programming Interface
## [政府資料開放平台](https://data.gov.tw/) / [台北市資料大平台](https://data.taipei/)

--

# JSON
## [Example](https://json.org/example.html)
## `jq` / [JSON Viewer](https://chrome.google.com/webstore/detail/json-viewer/gbmdgpbipfallnflgajpaliibnhdgobh) / [JSONView](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc)

--

# RESTful

--

# Web crawler / bot

--

# Q & A

--

### 延伸閱讀

- [從 0 開始的 Web Security](https://ithelp.ithome.com.tw/users/20129897/ironman/3431)

--

<h1 style="font-size: 72px">
  Thanks for listening!
</h1>

<br /><br /><br />
<div align="center">
  <img style="width:100px;" src="./img/by-sa.png" />
</div>
<h2 style="font-size: 18px">
本投影片採用<a href="http://creativecommons.org/licenses/by-sa/3.0/tw/" target="_blank">創用 CC「姓名標示—相同方式分享 3.0 台灣」授權條款</a>
</h2>
