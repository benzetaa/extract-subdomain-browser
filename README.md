## 🎁 Make your own top-subdomains wordlist from Firefox and Brave history: 

```
grep -Pao "(http|https)://[a-zA-Z0-9]+"  ~/.config/BraveSoftware/Brave-Browser/*/History |  sort -u | sed -E 's/(http:\/\/|https:\/\/)//g' | sort -u
grep -Pao "(http|https)://[a-zA-Z0-9]+" ~/snap/firefox/common/.mozilla/firefox/*/places.sqlite |  sort -u | sed -E 's/(http:\/\/|https:\/\/)//g' | sort -u
```
