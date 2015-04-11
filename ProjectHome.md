**Note : as Google is closing Google Code, the new official xxHash repository is now on Github** => https://github.com/Cyan4973/xxHash

xxHash is an extremely fast non-cryptographic Hash algorithm, working at speeds close to RAM limits.

32-bits hash comparison (single thread, Windows Seven 32 bits, using [Open Source's SMHasher](http://code.google.com/p/smhasher/wiki/SMHasher) on a Core 2 Duo @3GHz)

```
Name		Speed       Q.Score   Author
xxHash          5.4 GB/s     10
MumurHash 3a    2.7 GB/s     10       Austin Appleby
SpookyHash      2.0 GB/s     10       Bob Jenkins
SBox            1.4 GB/s      9       Bret Mulvey
Lookup3         1.2 GB/s      9       Bob Jenkins
CityHash64      1.05 GB/s    10       Pike & Alakuijala
FNV             0.55 GB/s     5       Fowler, Noll, Vo
CRC32           0.43 GB/s     9
MD5-32          0.33 GB/s    10       Ronald L. Rivest
SHA1-32         0.28 GB/s    10
```

Q.Score is a measure of quality of the hash function.
It depends on successfully passing [SMHasher test set](http://code.google.com/p/smhasher/wiki/SMHasher).
10 is a perfect score.
Hash functions with a Q.score < 5 are not listed in this table.

A new 64-bits version, named XXH64, is available since [r35](https://code.google.com/p/xxhash/source/detail?r=35). It offers better speed for 64-bits applications.

Hash comparison (single thread, Linux Mint 64 bits, using [Open Source's SMHasher](http://code.google.com/p/smhasher/wiki/SMHasher) on a Core i5 3340M @2.7GHs)
```
Name     Speed on 64 bits    Speed on 32 bits
XXH64       13.8 GB/s            1.9 GB/s       
XXH32        6.8 GB/s            6.0 GB/s
```

**[Download latest xxHash source code here](https://github.com/Cyan4973/xxHash/releases/latest)**


---


### Other versions : ###

  * **Java** : by Adrien Grand, at https://github.com/jpountz/lz4-java

  * **Javascript** (pure) : by Pierre Curto, at https://npmjs.org/package/xxhashjs

  * **Javascript** (NodeJS binding) : by Brian White, at https://npmjs.org/package/xxhash

  * **JSX** (static Javascript) : by Yoshiki Shibukawa, at https://www.npmjs.org/package/xxhash.jsx

  * **Ruby** (pure) : by Justin W Smith, at http://rubygems.org/gems/ruby-xxHash

  * **Ruby** wrapper : by Vasiliy Ermolovich, at https://rubygems.org/gems/xxhash

  * **C#** (XXH32) : by Seok-ju Yun, at https://github.com/noricube/xxHashSharp

  * **C#** (XXH64) : by Brandon Dahler, at http://www.nuget.org/packages/System.Data.HashFunction.xxHash/

  * **PHP** : by Stuart Herbert, at https://github.com/stuartherbert/php-xxhash

  * **Python** (XXH32) : by Ewen Cheslack-Postava, at https://pypi.python.org/pypi/pyhashxx/

  * **Python** (XXH64) : by Yue Du, at https://pypi.python.org/pypi/xxhash/

  * **Perl** : by Sanko Robinson, at https://metacpan.org/module/Digest::xxHash

  * **Pascal** : by Vojtěch Čihák, at http://sourceforge.net/projects/xxhashfpc

  * **Lua** (binding) : by Masatoshi Teruya, at https://github.com/mah0x211/lua-xxhash

  * **Lua-jit** : by szensk, at https://github.com/szensk/luaxxhash

  * **D** : by Masahiro Nakagawa, at https://github.com/repeatedly/xxhash-d

  * **Go** (XXH32) : by Stéphane Bunel, at https://bitbucket.org/StephaneBunel/xxhash-go

  * **Go** (XXH64) : by Ahmed Waheed, at https://github.com/OneOfOne/xxhash

  * **Haskell** : by Christian Marie, at http://hackage.haskell.org/package/xxhash

  * **Rust** : by György Andrasek, at https://github.com/Jurily/rust-xxhash

  * **Erlang** : by Pierre Matri, at https://github.com/pierresforge/erlang-xxhash



---


### What's new : ###

[r39](https://code.google.com/p/xxhash/source/detail?r=39) : minor alignment adjustments

[r38](https://code.google.com/p/xxhash/source/detail?r=38) : xxhsum can use stdin as input (default)



---


### xxHash is used by ###

  * **Databases** : <img src='https://dl.dropboxusercontent.com/u/59565338/Images/PrestoDB_logo.png' alt='PrestoDB' height='50' /> [PrestoDB](http://prestodb.io/) [(\*)](https://github.com/facebook/presto/commit/87cb4f2ba8a57a3edb6e4d5a89658b6a3191b3e7), <img src='https://fbcdn-dragon-a.akamaihd.net/hphotos-ak-ash3/t39.2365-6/851565_684758381542082_1107415997_n.png' alt='RocksDB' height='50' /> [RocksDB](http://rocksdb.org/) [(\*)](https://github.com/facebook/rocksdb/pull/87), [ArangoDB](https://www.arangodb.org/) [(\*)](http://fossies.org/dox/ArangoDB-2.1.2/xxhash_8h.html)

  * **Games** : <img src='http://www.cocos2d-x.org/attachments/709/cocos2dx_portrait.png' alt='cocos2D' height='50' /> [cocos2D](http://www.cocos2d.org/), <img src='http://upload.wikimedia.org/wikipedia/commons/thumb/d/dc/PPSSPP_logo.svg/512px-PPSSPP_logo.svg.png' alt='PPSSPP' height='50' /> [PPSSPP](http://ppsspp.org/) [(\*)](https://github.com/hrydgard/ppsspp/blob/master/ext/xxhash.h), <img src='http://i.imgur.com/rPAnDs2.png' alt='dolphin' height='50' /> [dolphin](https://dolphin-emu.org) [(\*)](https://github.com/dolphin-emu/dolphin/tree/master/Externals/xxhash)

  * **Security** : <img src='http://cdn1.itcentralstation.com/vendors/logos/original/pfsense-logo-chopped_reasonably_small.png?1371111700' alt='pfSense' height='50' /> [pfSense](https://www.pfsense.org/) [(\*)](https://doc.pfsense.org/index.php/2.2_New_Features_and_Changes#OS_Changes), [Rspamd](https://rspamd.com/) [(\*)](https://github.com/vstakhov/rspamd/tree/master/contrib/xxhash),

  * **Filters** : [LZ4](https://code.google.com/p/lz4/) [(\*)](https://code.google.com/p/lz4/source/browse/#svn%2Ftrunk), [Flexible I/O Tester](http://freecode.com/projects/fio), [Bloomxx](https://npmjs.org/package/bloomxx), [C & Python Bloom Filter](http://devisedbydavid.com/open_source/bloom_filter), <img src='http://upload.wikimedia.org/wikipedia/commons/5/5c/Mozilla_dinosaur_head_logo.png' alt='mozilla' height='50' /> [Mozilla's LUA bloom filter](https://github.com/mozilla-services/lua_bloom_filter)

  * **Other** : [PKG](https://wiki.freebsd.org/pkgng) [(\*)](https://github.com/freebsd/pkg/blob/master/external/libucl/src/xxhash.c), <img src='http://factorcode.org/logo.png' alt='Factor' width='115' /> [Factor](http://factorcode.org/) [(\*)](http://re-factor.blogspot.fr/2014/04/checksum-improvements.html), <img src='http://www.jigsaw24.com/news/wp-content/uploads/2013/04/Silverstack_logo.png' alt='Sliverstack' height='50' /> [Silverstack](http://pomfort.com/silverstack/) [(\*)](http://dorkinatent.com/2014/10/10/silverstack-v4-0/), [TeamViewer](http://www.teamviewer.com/) [(\*)](http://fr.scribd.com/doc/252185217/CopyRights-FOR-TEAM-VIEWER#scribd), [simplebayes](https://pypi.python.org/pypi/simplebayes/1.0.1), <img src='http://nvlabs.github.io/nvbio/nvidia_cubes.png' alt='NVBio' width='70' /> [NVBio](http://nvlabs.github.io/nvbio/index.html) [(\*)](http://nvlabs.github.io/nvbio/xxhash_8h_source.html)