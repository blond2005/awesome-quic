QUIC Weekly - 20201014期
---

* **Adoption** [Chrome is deploying HTTP/3 and IETF QUIC](https://blog.chromium.org/2020/10/chrome-is-deploying-http3-and-ietf-quic.html)
  * current latest Google QUIC version (Q050) has many similarities with IETF QUIC. But up until now, the majority of Chrome users didn't communicate with IETF QUIC servers without enabling some command-line options.
  * Google search latency decreases by over 2%. YouTube rebuffer time decreased by over 9%, while client throughput increased by over 3% on desktop and over 7% on mobile. We're happy to announce that Chrome is rolling out support for IETF QUIC (specifically, draft version h3-29)
  * Today 25% of Chrome Stable users are using h3-29, and we plan on increasing that number over the coming weeks as we continue to monitor performance data
  * Chrome will actively support both IETF QUIC h3-29 and Google QUIC Q050 to provide servers that support Q050 with time to update to IETF QUIC.
* **Adoption** Cloudflare begins emailing users that [H3 will be automatically enabled](https://cloudflare-quic.com/) starting this month
* CDNs are misunderstood these days. Caching at the browser across sites is not that important, it caching at a point of presence (POP). This POP being so much closer to your end users brings performance gains because TCP is terrible over distances. QUIC may fix this by it's shift to UDP. [HackerNews](https://news.ycombinator.com/item?id=24745794)
* **TechTalk** Lucas Pardue: [QUIC & HTTP/3: Open Standards and Open Source Code](https://www.digitalocean.com/community/tech_talks/quic-http-3-open-standards-and-open-source-code) October 27, 2020
* **OpenSource** [quiche](https://github.com/cloudflare/quiche/commit/75c62c1fe97578173b74f16717a7fe9f2d34d5b0) landed supported for QUIC & HTTP/3 unreliable datagram. It can help support low-latency where guaranteed delivery of data is not paramount.
* [Developing QUIC Loss Detection and Congestion Control in Haskell](https://kazu-yamamoto.hatenablog.jp/entry/2020/09/15/121613)


Telegram群：[t.me/quic_weekly](https://t.me/quic_weekly)

* **Adoption** [Chrome 正在部署 HTTP/3 和 IETF QUIC](https://blog.chromium.org/2020/10/chrome-is-deploying-http3-and-ietf-quic.html)
  * 当前最新的 Google QUIC 版本（Q050）与 IETF QUIC 有很多相似之处。但是到目前为止，大多数 Chrome 用户在未启用某些命令行选项的情况下没有与 IETF QUIC 服务器通信。
  * Google 搜索延迟减少了2％以上。 YouTube 的重新缓冲时间减少了9％以上，而台式机的客户端吞吐量增加了3％以上，移动设备的客户端吞吐量增加了7％以上。我们很高兴地宣布，Chrome 即将推出对 IETF QUIC（特别是草稿版本 H3-29）的支持。
  * 目前，有25％的 Chrome 稳定用户正在使用 H3-29。我们计划在接下来的几周内增加该数字，并继续监控性能数据。
  * Chrome 将积极支持 IETF QUIC H3-29 和 Google QUIC Q050，让支持 Q050 的服务器有时间更新到 IETF QUIC。
* **Adoption** Cloudflare 向用户发送电子邮件，通知从本月开始 [H3 将自动启用](https://cloudflare-quic.com/)。
* CDN 最近被误解了。跨站点的浏览器缓存并不是那么重要，重要的是在存在点（POP）进行缓存。这种 POP 与你的终端用户的距离如此之近，可带来性能提升，因为TCP的传输距离很差。QUIC 可以通过改用 UDP 来解决此问题。 [HackerNews](https://news.ycombinator.com/item?id=24745794)
* **TechTalk** Lucas Pardue：[QUIC 和 HTTP/3：开放标准和开放源代码](https://www.digitalocean.com/community/tech_talks/quic-http-3-open-standards-and-开源代码) 2020年10月27日。
* **OpenSource** [quiche](https://github.com/cloudflare/quiche/commit/75c62c1fe97578173b74f16717a7fe9f2d34d5b0) 已支持 QUIC 和 HTTP/3 不可靠的数据报。在保证数据的传输不是最重要的情况下，它可以降低延迟。
* [在 Haskell 中开发 QUIC 丢失检测和拥塞控制](https://kazu-yamamoto.hatenablog.jp/entry/2020/09/15/121613)。