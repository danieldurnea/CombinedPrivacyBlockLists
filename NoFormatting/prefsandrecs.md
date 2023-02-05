**Recommendations & Preferences**  
How to use my lists:
- In terms of hosts files, DNSCrypt blacklists, or any DNS-based filtering solution, I only use my compiled lists (Standard/Full on desktop devices, and Mini/Light on mobile and low spec devices). I pull in data from a wide variety of sources meant to cover most ad-blocking and privacy use cases - and many locales - so I see no need to use these lists with any others.
- With Ad-blocking extensions for browsers it is a bit more complicated, so I use my ABP/uBO/AG filter list in conjunction with other lists, which always includes either AdGuard's Base + Tracking + Annoyance filters, or EasyList + EasyPrivacy + FanBoy's Annoyance filters, at bare minimum. This is mainly due to the additional exception rules, along with procedural and cosmetic filters, which other lists provide.
- My IP block lists for torrent clients and other P2P applications are meant to be used stand-alone. They offer solid protection against bad actors and threats, while reducing the risk of blocking legitimate traffic (which much larger compilations are known for).
- My CIDR IP block list is meant to function as a nice baseline for individuals and very small organizations that run public-facing servers. I have found this list to be quite effective at preventing waves of intrusion attempts when I'm running public IceCast or Shoutcast streams for days or weeks at a time. If you're dealing with a larger amount of traffic on a 24/7 basis - especially international traffic - you will likely want to supplement this list with more aggressive bogon filtering and region-specific data.

---
Privacy-oriented DNS Clients:
- [Stubby](https://dnsprivacy.org/dns_privacy_daemon_-_stubby/)
- [DNSCrypt Proxy](https://github.com/DNSCrypt/dnscrypt-proxy)
- [Systemd-Resolved](https://www.freedesktop.org/software/systemd/man/systemd-resolved.service.html)
- [Simple DNSCrypt](https://simplednscrypt.org/)

<sub>At least one of these is running around the clock on some device in my possession. They get the job done and allow the utilization of at-least one encrypted DNS protocol.</sub>

---
DNS Resolvers:
- [AdGuard](https://adguard-dns.io/en/public-dns.html)
- [Quad9](https://www.quad9.net/service/service-addresses-and-features)
- [Rethink](https://rethinkdns.com/configure)
- [DNS Warden](https://dnswarden.com/customfilter.html)

<sub>These are simply my preferences. There are other fine resolvers out there, but I love the reliability of AdGuard and Quad9, along with the enormous amount of configurability that Rethink and DNS Warden offer. All four of these resolvers have fine privacy policies that range from minimal logging, to no logging at all. In very rare circumstances when I cannot use encrypted DNS, I tend toward [OpenNIC](https://www.opennic.org/) or [OpenDNS](https://www.opendns.com/).</sub>

---
Dedicated Ad-Block / Filtering Software & Plugins:
- [AdAway](https://adaway.org/)
- [AdGuard](https://adguard.com/en/welcome.html)
- [uBlock Origin](https://github.com/gorhill/uBlock)
- [AdBlock Plus](https://adblockplus.org/)
- [Rethink DNS + Firewall](https://rethinkdns.com/app)
- [Simple-AdBlock for OpenWrt](https://docs.openwrt.melmac.net/simple-adblock/)
- [AdBlock for OpenWrt](https://github.com/openwrt/packages/tree/master/net/adblock/files)
- [banIP for OpenWrt](https://github.com/openwrt/packages/tree/master/net/banip)

<sub>My preferred ad-blocking extension is uBO, though AdGuard's flexibility is beyond impressive (this applies to both their stand-alone applications and the browser extension). ABP - while it has generated controversy in the past - is the most widely available Ad-blocking extension, has always been an open source project, and its lasting influence on other ad-blocking projects is undeniable. The infrastructure which ABP provides to list maintainers for issue reporting and feedback is profoundly useful as well. In terms of mobile software I find that AdAway is the simplest option for rooted Android devices, and Rethink offers the most flexible and performant option for Android devices without root (it is also a DNS Client for multiple protocols to boot).</sub>


<sub>In regard to the OpenWrt plugins, I use Simple-AdBlock on low spec routers, AdBlock on higher spec routers, and banIP on anything that runs OpenWrt. All three plugins are fantastic. On the topic, I have used PiHole in my home network at different points in time, and while it is superb, I have found that using OpenWrt on my routers (wired and wireless) - with some combination of the aforementioned plugins - is more than sufficient for my network-wide filtering needs.</sub>

---
Web Browsers:
- [Firefox](https://www.mozilla.org/en-US/firefox/releases/)+
- [Brave](https://brave.com/latest/)+
- [IceCat](https://www.gnu.org/software/gnuzilla/)
- [NetSurf](https://www.netsurf-browser.org/)
- [Falkon](https://www.falkon.org/)
- [Mull](https://f-droid.org/en/packages/us.spotco.fennec_dos/)

<sub>Items with a "+" require a notable amount of manual configuration to be truly respecting of user privacy, but once this is done they are more than adequate choices for users who value this. I prefer IceCat and Brave under GNU/Linux; Firefox and Brave when I am forced to use Windows or OS X; Brave and Mull under Android. Additionally, I like NetSurf for reading long articles and working on websites which don't employ complex JavaScript. I think the Falkon project is wonderful as well, so I keep it around on some machines for testing. I also test my Bromite filter list in Bromite every few weeks, but the browser is not flexible enough to warrant my using it as a daily driver.</sub>
