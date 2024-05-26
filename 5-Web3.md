# Browser-based Sharing & Connecting

<div style="width:100%;height:0;padding-bottom:100%;position:relative;"><iframe src="https://giphy.com/embed/xThuW7icYBlQZxjnyg" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/truthorange-dog-surprised-wtf-xThuW7icYBlQZxjnyg">via GIPHY</a></p>

## Peer-To-Peer in da Browser

    {{1-2}}
``` ascii    __Fig:__ Classic Client & Server Applications
    👨🏾‍💻 --.     .-- 👩‍💻
          \   /

👩‍💻 ------  🖥️  ------ 👨🏾‍💻

          /   \
    👨🏾‍💻 --'     '-- 👩‍💻
```

    {{2}}
``` ascii    __Fig:__ Peer^2^Peer- or Mesh-Networks
- - - --👨🏾‍💻-----👩‍💻
              /  \
             /    \
    👩‍💻------+-----👨🏾‍💻- - -
      \    /      /
       \  /      /
        👨🏾‍💻     👩‍💻- - - -
```

## Sharing/Storing Content

    {{1}}
![Burning library of Alexandria](pic/alexandria.jpg)

### Data-Protocol

    {{0-3}}
> Data URLs allow for the inclusion of small data items directly within web addresses by encoding the data as a string. This method eliminates the need for external file sources and reduces the number of HTTP requests, potentially speeding up web page load times. The format for a Data URL starts with 'data:', followed by a MIME type and the data itself, usually encoded in Base64. For example, an image can be embedded directly into an HTML document using a Data URL like this: 
>
> `data:[<mediatype>][;base64],<data>`
>
> This is particularly useful for embedding small images or documents but should be used judiciously due to its impact on page size and browser performance.
>
> Source: https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URLs


    {{1-3}}
```
<img src="data:image/jpeg;base64,
/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDADIiJSwlHzIsKSw4NTI7S31RS0VFS5ltc1p9tZ++u7Kf
r6zI4f/zyNT/16yv+v/9////////wfD/////////////2wBDATU4OEtCS5NRUZP/zq/O////////
////////////////////////////////////////////////////////////wAARCAAYAEADAREA
AhEBAxEB/8QAGQAAAgMBAAAAAAAAAAAAAAAAAQMAAgQF/8QAJRABAAIBBAEEAgMAAAAAAAAAAQIR
AAMSITEEEyJBgTORUWFx/8QAFAEBAAAAAAAAAAAAAAAAAAAAAP/EABQRAQAAAAAAAAAAAAAAAAAA
AAD/2gAMAwEAAhEDEQA/AOgM52xQDrjvAV5Xv0vfKUALlTQfeBm0HThMNHXkL0Lw/swN5qgA8yT4
MCS1OEOJV8mBz9Z05yfW8iSx7p4j+jA1aD6Wj7ZMzstsfvAas4UyRHvjrAkC9KhpLMClQntlqFc2
X1gUj4viwVObKrddH9YDoHvuujAEuNV+bLwFS8XxdSr+Cq3Vf+4F5RgQl6ZR2p1eAzU/HX80YBYy
JLCuexwJCO2O1bwCRidAfWBSctswbI12GAJT3yiwFR7+MBjGK2g/WAJR3FdF84E2rK5VR0YH/9k=">
```

    {{2-3}}
<lia-keep>

<img src="data:image/jpeg;base64,
/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDADIiJSwlHzIsKSw4NTI7S31RS0VFS5ltc1p9tZ++u7Kf
r6zI4f/zyNT/16yv+v/9////////wfD/////////////2wBDATU4OEtCS5NRUZP/zq/O////////
////////////////////////////////////////////////////////////wAARCAAYAEADAREA
AhEBAxEB/8QAGQAAAgMBAAAAAAAAAAAAAAAAAQMAAgQF/8QAJRABAAIBBAEEAgMAAAAAAAAAAQIR
AAMSITEEEyJBgTORUWFx/8QAFAEBAAAAAAAAAAAAAAAAAAAAAP/EABQRAQAAAAAAAAAAAAAAAAAA
AAD/2gAMAwEAAhEDEQA/AOgM52xQDrjvAV5Xv0vfKUALlTQfeBm0HThMNHXkL0Lw/swN5qgA8yT4
MCS1OEOJV8mBz9Z05yfW8iSx7p4j+jA1aD6Wj7ZMzstsfvAas4UyRHvjrAkC9KhpLMClQntlqFc2
X1gUj4viwVObKrddH9YDoHvuujAEuNV+bLwFS8XxdSr+Cq3Vf+4F5RgQl6ZR2p1eAzU/HX80YBYy
JLCuexwJCO2O1bwCRidAfWBSctswbI12GAJT3yiwFR7+MBjGK2g/WAJR3FdF84E2rK5VR0YH/9k=">

</lia-keep>


    {{3}}
__Can it be used for more?__<!-- style="font-size: 30px" -->


### Tor & Onion-Share

> The [Tor Network](https://en.wikipedia.org/wiki/Tor_%28network%29) is a system that allows users to anonymize their online activities and identity by routing their traffic through multiple servers to conceal the source of the data. The network consists of thousands of volunteer servers around the world that act as "nodes" and encrypt the traffic to protect users' privacy.

                        {{0-1}}
![Internet censorship](https://raw.githubusercontent.com/LiaPlayground/University-Future-Festival-2023/main/img/censorship.png "Source: https://www.comparitech.com/blog/vpn-privacy/internet-censorship-map ")

                        {{1-2}}
![Taliban](https://raw.githubusercontent.com/LiaPlayground/University-Future-Festival-2023/main/img/taliban.png "Source: _ https://taz.de/Repressionen-in-Afghanistan/!5926105/ \| https://www.deutschlandfunkkultur.de/afghanistan-bildung-100.html \| https://www.business-standard.com/article/international/taliban-blocks-23-mn-websites-in-afghanistan-over-immoral-content-122082600086_1.html \| https://www.reuters.com/world/asia-pacific/afghan-girls-struggle-with-poor-internet-they-turn-online-classes-2023-03-27/ _")

    {{2}}
<section>

#### Tor Browser: For anonymous browsing

* Download & Install: https://www.torproject.org/download/

* Disable private browsing to enable IndexedDB for caching LiaScript courses:
  
  Settings >> Privacy & Security >> History >> Always use private browsing mode (disable)

* Enable CORS:

  Settings >> Extensions & Themes >> Search for "[CORS Unblock](https://addons.mozilla.org/en-US/firefox/addon/cors-unblock/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search)" >> Click on "[CORS Unblock](https://addons.mozilla.org/en-US/firefox/addon/cors-unblock/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search)" >> Install (Add to Firefox)

  If you have __disabled private browsing__ mode, enable "CORS Unblock".

  Otherwise, enable the plugin first to be used in private mode:
  Settings >> Extensions & Themes >> "CORS Unblock" >> Run in Private Windows (Allow)

  ![Activate CORS Unblock](https://addons.mozilla.org/user-media/previews/full/213/213890.png?modified=1622134234)


#### OnionShare for anonymous hosting and sharing

* Download & Install: https://onionshare.org
* Open and "Connect to Tor"
* Share data: Start Hosting >> Add Files or Add Folder >> Start sharing
* Send the Onion-Address and the Private-Key to your students
* Open the Onion-Address within the Tor-Browser, enter the private key and select "Remember this key"
* Open the README.md of the course and copy this URL
* Goto https://LiaScript.github.io and paste this URL "click on Load URL"

</section>

### IPFS & IPNS

> The __I__nter__P__lanetary __F__ile __S__ystem (IPFS) is a protocol, hypermedia and file sharing peer-to-peer network for storing and sharing data in a distributed file system ... supported by Opera, Brave-Browser, Agregore, and more to come
>
> https://ipfs.tech

![IPFS logo](https://camo.githubusercontent.com/17f4e2f91811db1b94b4d58e7ea273359b9ffa541d8787867576de0262bb55e4/68747470733a2f2f69636f6d6d756e6974792e696f2f77702d636f6e74656e742f75706c6f6164732f323032302f30382f495046532e6a7067)

### WebTorrent

> WebTorrent is a peer-to-peer (P2P) streaming torrent client written in JavaScript, from the same author, Feross Aboukhadijeh, of YouTube Instant, and the team at WebTorrent and on GitHub, for use in web browsers, as well as a WebTorrent Desktop stand alone version able to bridge WebTorrent and BitTorrent serverless networks.
>
> Source: [Wikipedia](https://en.wikipedia.org/wiki/WebTorrent)


Try it on: https://instant.io

## Connecting Users

<div style="width:100%;height:0;padding-bottom:75%;position:relative;"><iframe src="https://giphy.com/embed/SPZFhfUJjsJO0" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/internet-level-ii-SPZFhfUJjsJO0">via GIPHY</a></p>

### WebRTC

> The __Web Real-Time Communication__ is a free and open-source project providing web browsers and mobile applications with real-time communication (RTC) via application programming interfaces (APIs).
> It allows audio and video communication to work inside web pages by allowing direct peer-to-peer communication, eliminating the need to install plugins or download native apps...
>
> _Source: [Wikpedia](https://en.wikipedia.org/wiki/WebRTC)_


    {{0-1}}
``` ascii
                     (WebRTC)
Alice 👩‍💻 <------------------------------> 👨🏾‍💻 Bob
```

    {{1}}
``` ascii
               (Signaling Server)

       .-------------> 🖥️ --------------.
       |    "{1}{}"   /  A      "{2}{}" |
       |             /    \             |
       |            /      \            V
                   /        \
Alice 👩‍💻 <--------'          '--------- 👨🏾‍💻 Bob
            "{4}{}"             "{3}{}"
      A                                  A
      |                                  |
      '----------------------------------'
      A    "{5}{Direct Communication}"   A
      |                                  |
      '-- - - - - - - - - - - - - - - - -'
             "{6}{InDirect via TURN}"
```

    {{7}}
> More confusing information on WebRTC:
>
> !?[WebRTC](https://www.youtube.com/watch?v=7cbD-hFkzY0)


### CRDTs

A _**C**onflict-free **R**eplicated **D**ata **T**ype_ (CRDT) is a new type of data structure[^1] that can be replicated across multiple instances in a network with the following guarantees:

    {{1}}
1. A replica can be updated independently, concurrently and without coordinating with other replicas.
2. Inconsistencies can be resolved automatically.
3. Although replicas may have different state, they are guaranteed to eventually converge.

    {{2}}
__Task:__ Implement an distributed counter

    {{3}}
``` ascii
Alice 👩‍💻

[0]---------*-->[5]--[+1 = 6]--------*-->[8]-- - - - - - - - - - - - 
           /            \           /          \
          A              V         A            \
         /                        /              \
[0]---[+5 = 5]-----------------[+2 = 7]-- - - - --*- - - - - - - - - -

Bob 👨🏾‍💻
```

    {{4}}
__Solution:__ Use Sets and Unions instead... 

    {{5}}
``` ascii
Alice 👩‍💻

{(a,0)}----------*-->{(a,0),(b,5)}->{(a,1),(b,5)}---*-->{(a,1),(b,7)}
                /                         \        /   
               A                           V      A   
              /                                  /
{(b,0)}---{(b,5)}----------------------------{(b,7)}-----------------

Bob 👨🏾‍💻
```

    {{6}}
<section>

__ Implementations__

- [Automerge](https://automerge.org)
- [__Yjs__](https://docs.yjs.dev)

</section>


[^1]: The CRDT concept was defined in 2011 by Marc Shapiro, Nuno Preguiça, Carlos Baquero and Marek Zawirski.

      See also: https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type

## Try it Out

...