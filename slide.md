---
title: 網路概論：從底層到應用的觀念與實作
description: 每天滑手機、逛網頁，是否好奇這些資訊如何從伺服器傳送到你的眼前？這堂課將帶你從網路的基礎建設、協定，到實際的應用，了解網路的運作原理。
author: Denny Huang
keywords: 網路概論, 網路基礎, TCP/IP, HTTP, RESTful API, OSI 模型, DNS 解析, ARP, Netcat, Wireshark, Python HTTP Server, 網路教學, 網路工作坊, 伺服器架設
url: https://denny.one/the-net/
paginate: true
---

<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-VF1P1LBET1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-VF1P1LBET1');
</script>

<!-- _paginate: false -->

# 網路概論：<br />從底層到應用的觀念與實作<br />
<br />

## Denny Huang

---

# Denny Huang

- <a href="https://sitcon.org/" target="_blank">SITCON 學生計算機年會</a> 共同發起人
- 雷亞遊戲 Rayark Inc.
- <a href="https://denny.one/" target="_blank">About me</a>

---

# 課程內容以 Linux 發行版本進行
## Windows 使用者請使用 WSL

---

# 已有基礎者，推薦閱讀
## Kenny Huang, Ph.D. 黃勝雄 博士

- <a href="https://www.slideshare.net/tahr1984/kenny-huang-phd" target="_blank">網路之根 – 基礎建設與標準化</a>
- <a href="https://www.youtube.com/watch?v=aa_DdMpNI5Q" target="_blank">SITCON 2017 - Cybersecurity and Internet Governance 網路安全與網路治理</a>

---

# [History of the Internet](https://zh.wikipedia.org/wiki/%E7%B6%B2%E9%9A%9B%E7%B6%B2%E8%B7%AF%E6%AD%B7%E5%8F%B2)

---

# <a href="https://zh.wikipedia.org/wiki/OSI%E6%A8%A1%E5%9E%8B" target="_blank">OSI</a>
## <a href="https://www.explainxkcd.com/wiki/index.php/1417:_Seven" target="_blank">7?</a> <a href="https://www.cs.purdue.edu/homes/comer/essay.network.layers.html" target="_blank">7?</a>

---

# [IETF](https://zh.wikipedia.org/zh-tw/%E7%B6%B2%E9%9A%9B%E7%B6%B2%E8%B7%AF%E5%B7%A5%E7%A8%8B%E4%BB%BB%E5%8B%99%E7%B5%84)/[RFC](https://zh.wikipedia.org/wiki/RFC)
## [RFC 2324](https://tools.ietf.org/html/rfc2324)
## [RFC 2468](https://tools.ietf.org/html/rfc2468)

---

# Network Interface
## [Predictable Network Interface Names](https://www.freedesktop.org/wiki/Software/systemd/PredictableNetworkInterfaceNames/)

---

# Ask the man
## `man [command]`

---

# IP
## [Public IP / Private IP](https://datatracker.ietf.org/doc/html/rfc3330#section-3)
## `ip addr / ip a`

---

# ARP
## `arp / ip neighbour / ip n`

---

# Gateway / Netmask
## `ip route / ip r / route / traceroute / mtr`

---

# Port

---

# <a href="https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE" target="_blank">TCP</a> / <a href="https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE" target="_blank">UDP</a>
## `nc -lvp [port] / nc -v [hostname/ip] [port]`
## `nc -lvup [port] / nc -vu [hostname/ip] [port]`

---

# Three-Way Handshake
## Wireshark
## `tcpdump -X host [ip]`

---

# <a href="https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE" target="_blank">DNS</a>
## `dig / nslookup`
## whois

---

# HTTP
## [request method](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods) / [status code](https://http.cat) / [headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)
[IETF HTTP-WG Mailing List 〈Re: Referer: (sic)〉](https://lists.w3.org/Archives/Public/ietf-http-wg/1995JanMar/0109.html)

---

# Response a web page

## Server
`nc -lvp 8000`
```
HTTP/1.1 200 OK[Enter]
[Enter]
Hello
^C
```
## Clint
- Browser
- `curl -v localhost:8000`

---

# Python 3 HTTP Server

## Start Server
`python3 -m http.server`

## Request with
- `nc -v 0 8000`
	- `GET / HTTP/1.1`
- `curl -v localhost:8000`
- Browser

---

# HTTPS

---

# Cookie / Session

---

# [How Browsers Work?](https://github.com/alex/what-happens-when)

---

# API
## Application Programming Interface
## [政府資料開放平台](https://data.gov.tw/) / [台北市資料大平台](https://data.taipei/)

---

# JSON
## [Example](https://json.org/example.html)
## `jq` / [JSONVue](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc)

---

# RESTful

---

# Web crawler / bot

---

# Q & A

---

# 延伸閱讀

- [從 0 開始的 Web Security](https://ithelp.ithome.com.tw/users/20129897/ironman/3431)
- [roadmap.sh](https://roadmap.sh/)
- [2021 Web Developer Roadmap](https://github.com/goodjack/developer-roadmap-chinese)

---

# Thanks for listening

<br />
<br />

###### 本投影片採用
![width:60px](./img/by-sa.png) <a href="https://creativecommons.org/licenses/by-sa/4.0/deed.zh-hant" target="_blank">創用 CC「姓名標示-相同方式分享 4.0 國際」授權條款</a>釋出
![width:60px](./img/marp.svg) <a href="https://marp.app/" target="_blank">Marp</a> 製作
