# esolang-box 2.1.0 [![Build Status][travis-image]][travis-url]

[travis-image]: https://travis-ci.org/hakatashi/esolang-box.svg?branch=master
[travis-url]: https://travis-ci.org/hakatashi/esolang-box

Easy and standalized docker images for 150+ esoteric (and non-esoteric) languages.

## Usage

Distributed docker images are seperated for each esolangs.

For example docker image for [Evil](https://esolangs.org/wiki/Evil) language is named as `esolang/evil`, which is hosted on [Dockre Hub](https://hub.docker.com/r/esolang/evil/).

### How to run your own esolang program

Suppose you have program in the current directory,

```sh
$ echo aeeeaeeewueuueweeueeuewwaaaweaaewaeaawueweeeaeeewaaawueeueweeaweeeueuw > program.evil
```

then you can run the program like the following.

```sh
$ docker run -v `pwd`:/code:ro esolang/evil evil /code/program.evil
Hello, World!
```

## List of boxes

* [`esolang/base`](https://hub.docker.com/r/esolang/base/)
    * [`esolang/build-base`](https://hub.docker.com/r/esolang/build-base/)
        * [`esolang/multi-reader`](https://hub.docker.com/r/esolang/multi-reader/): [multi-reader](https://github.com/kuromunori/kusogengo)
        * [`esolang/codemania`](https://hub.docker.com/r/esolang/codemania/): [CodeMania](https://github.com/Tiramister/codemania)
        * [`esolang/3var`](https://hub.docker.com/r/esolang/3var/): [3var](https://esolangs.org/wiki/3var)
        * [`esolang/axo`](https://hub.docker.com/r/esolang/axo/): [Axo](https://esolangs.org/wiki/Axo)
        * [`esolang/befunge93`](https://hub.docker.com/r/esolang/befunge93/): [Befunge-93](https://esolangs.org/wiki/Befunge)
        * [`esolang/befunge98`](https://hub.docker.com/r/esolang/befunge98/): [Befunge-98](https://esolangs.org/wiki/Befunge)
            * [`esolang/seed`](https://hub.docker.com/r/esolang/seed/): [Seed](https://esolangs.org/wiki/Seed)
        * [`esolang/brainfuck-esotope`](https://hub.docker.com/r/esolang/brainfuck-esotope/): [Brainfuck (esotope)](https://github.com/lifthrasiir/esotope-bfc)
        * [`esolang/c-gcc`](https://hub.docker.com/r/esolang/c-gcc/): [C (GCC)](https://gcc.gnu.org/)
        * [`esolang/dis`](https://hub.docker.com/r/esolang/dis/): [Dis](https://esolangs.org/wiki/Dis)
        * [`esolang/glass`](https://hub.docker.com/r/esolang/glass/): [Glass](https://esolangs.org/wiki/Glass)
        * [`esolang/ruby`](https://hub.docker.com/r/esolang/ruby/): [Ruby 2.6.0](https://www.ruby-lang.org/)
            * [`esolang/golfscript`](https://hub.docker.com/r/esolang/golfscript/): [GolfScript](http://www.golfscript.com/golfscript/tutorial.html)
            * [`esolang/hexagony`](https://hub.docker.com/r/esolang/hexagony/): [Hexagony](https://github.com/m-ender/hexagony)
            * [`esolang/stackcats`](https://hub.docker.com/r/esolang/stackcats/): [Stack Cats](https://github.com/m-ender/stackcats)
            * [`esolang/standback`](https://hub.docker.com/r/esolang/standback/): [(?i:standback)](https://github.com/akouryy/standback)
            * [`esolang/ppap`](https://hub.docker.com/r/esolang/ppap/): [PPAP](https://github.com/yhara/ppap-lang)
            * [`esolang/starry`](https://hub.docker.com/r/esolang/starry/): [Starry](https://esolangs.org/wiki/Starry)
            * [`esolang/cy`](https://hub.docker.com/r/esolang/cy/): [Cy](https://github.com/cyoce/Cy)
            * [`esolang/labyrinth`](https://hub.docker.com/r/esolang/labyrinth/): [Labyrinth](https://github.com/m-ender/labyrinth)
            * [`esolang/typhon`](https://hub.docker.com/r/esolang/typhon/): [Typhon](https://github.com/nefo-mi/Typhon)
            * [`esolang/alice`](https://hub.docker.com/r/esolang/alice/): [Alice](https://github.com/m-ender/alice)
            * [`esolang/wake`](https://hub.docker.com/r/esolang/wake/): [wake](http://shinh.skr.jp/wake/)
            * [`esolang/reversed-c`](https://hub.docker.com/r/esolang/reversed-c/): [reversed-c](https://github.com/cookie-s/reversed-c)
            * [`esolang/copos-rb`](https://hub.docker.com/r/esolang/copos-rb/): [copos (Ruby)](https://github.com/n4o847/tsg-2018-summer)
            * [`esolang/golfish`](https://hub.docker.com/r/esolang/golfish/): [golfish](https://github.com/n4o847/tsg-2018-summer)
        * [`esolang/goruby`](https://hub.docker.com/r/esolang/goruby/): [goruby](https://github.com/ruby/ruby/blob/trunk/man/goruby.1)
        * [`esolang/ruby1`](https://hub.docker.com/r/esolang/ruby1/): [Ruby 1.8](https://www.ruby-lang.org/)
            * [`esolang/grass`](https://hub.docker.com/r/esolang/grass/): [Grass](http://www.blue.sky.or.jp/grass/)
            * [`esolang/modanshogi`](https://hub.docker.com/r/esolang/modanshogi/): [ModanShogi](https://github.com/yhara/ShogiModan)
        * [`esolang/make`](https://hub.docker.com/r/esolang/make/): [Make](https://www.gnu.org/software/make/)
        * [`esolang/malbolge`](https://hub.docker.com/r/esolang/malbolge/): [Malbolge](https://esolangs.org/wiki/Malbolge)
        * [`esolang/piet`](https://hub.docker.com/r/esolang/piet/): [Piet](http://www.dangermouse.net/esoteric/piet.html)
        * [`esolang/python1`](https://hub.docker.com/r/esolang/python1/): [Python 1](https://www.python.org/)
        * [`esolang/rail`](https://hub.docker.com/r/esolang/rail/): [Rail](https://esolangs.org/wiki/Rail)
        * [`esolang/simula`](https://hub.docker.com/r/esolang/simula/): [Simula](https://en.wikipedia.org/wiki/Simula)
        * [`esolang/snowman`](https://hub.docker.com/r/esolang/snowman/): [Snowman](https://github.com/KeyboardFire/snowman-lang)
        * [`esolang/streem`](https://hub.docker.com/r/esolang/streem/): [Streem](https://github.com/matz/streem)
        * [`esolang/unlambda`](https://hub.docker.com/r/esolang/unlambda/): [Unlambda](http://www.madore.org/~david/programs/unlambda/)
        * [`esolang/verilog`](https://hub.docker.com/r/esolang/verilog/): [Verilog (Icarus Verilog)](http://iverilog.icarus.com/)
        * [`esolang/wierd`](https://hub.docker.com/r/esolang/wierd/): [Wierd](http://catseye.tc/node/Wierd.html)
        * [`esolang/wordcpu`](https://hub.docker.com/r/esolang/wordcpu/): [Word!CPU](https://esolangs.org/wiki/Word!CPU)
        * [`esolang/aheui`](https://hub.docker.com/r/esolang/aheui/): [Aheui](http://aheui.github.io/specification.en)
        * [`esolang/whitespace`](https://hub.docker.com/r/esolang/whitespace/): [Whitespace](https://esolangs.org/wiki/Whitespace)
        * [`esolang/beatnik`](https://hub.docker.com/r/esolang/beatnik/): [Beatnik](https://esolangs.org/wiki/Beatnik)
        * [`esolang/blc`](https://hub.docker.com/r/esolang/blc/): [Binary lambda calculus](https://tromp.github.io/cl/cl.html)
        * [`esolang/z80`](https://hub.docker.com/r/esolang/z80/): [Z80](https://sites.google.com/site/codegolfingtips/Home/z80)
        * [`esolang/spl`](https://hub.docker.com/r/esolang/spl/): [Shakespeare](http://shakespearelang.sourceforge.net/)
        * [`esolang/emojicode`](https://hub.docker.com/r/esolang/emojicode/): [Emojicode](http://www.emojicode.org/)
        * [`esolang/intercal`](https://hub.docker.com/r/esolang/intercal/): [INTERCAL](https://en.wikipedia.org/wiki/INTERCAL)
        * [`esolang/lolcode`](https://hub.docker.com/r/esolang/lolcode/): [LOLCODE](http://lolcode.org/)
        * [`esolang/minus`](https://hub.docker.com/r/esolang/minus/): [Minus](http://www.golfscript.com/minus/)
        * [`esolang/sqlite3`](https://hub.docker.com/r/esolang/sqlite3/): [SQLite3](https://sqlite.org/)
        * [`esolang/taxi`](https://hub.docker.com/r/esolang/taxi/): [Taxi](https://bigzaphod.github.io/Taxi/)
        * [`esolang/adjust`](https://hub.docker.com/r/esolang/adjust/): [ADJUST](https://esolangs.org/wiki/ADJUST)
        * [`esolang/braille`](https://hub.docker.com/r/esolang/braille/): [Braille](https://esolangs.org/wiki/Braille)
        * [`esolang/rust`](https://hub.docker.com/r/esolang/rust/): [Rust](https://www.rust-lang.org/)
        * [`esolang/cubically`](https://hub.docker.com/r/esolang/cubically/): [Cubically](https://github.com/aaronryank/Cubically)
        * [`esolang/sceql`](https://hub.docker.com/r/esolang/sceql/): [Sceql](http://esolangs.org/wiki/Sceql)
        * [`esolang/apl`](https://hub.docker.com/r/esolang/apl/): [APL](https://www.gnu.org/software/apl/)
        * [`esolang/wat`](https://hub.docker.com/r/esolang/wat/): [WebAssembly Text Format](https://webassembly.github.io/spec/core/text/index.html)
        * [`esolang/lazyk`](https://hub.docker.com/r/esolang/lazyk/): [Lazy-K](http://homepages.cwi.nl/~tromp/cl/lazy-k.html)
        * [`esolang/doubleplusungood`](https://hub.docker.com/r/esolang/doubleplusungood/): [Doubleplusungood](http://argxento.hatenadiary.jp/entry/esolang-advcal12-doubleplusungood)
        * [`esolang/llvm-ir`](https://hub.docker.com/r/esolang/llvm-ir/): [LLVM IR](https://releases.llvm.org/5.0.0/docs/LangRef.html)
        * [`esolang/hanoi_stack`](https://hub.docker.com/r/esolang/hanoi_stack/): [Hanoi_Stacck](https://github.com/JP3BGY/Hanoi_Stack/)
        * [`esolang/brainfuck-moratorium`](https://hub.docker.com/r/esolang/brainfuck-moratorium/): [Brainfuck (moratorium)](https://gist.github.com/moratorium08/2fa8dbd4150c8db547a1f3a31d5499ac)
    * [`esolang/java`](https://hub.docker.com/r/esolang/java/): [Java](https://java.com/)
        * [`esolang/arnoidc`](https://hub.docker.com/r/esolang/arnoidc/): [ArnoidC](http://lhartikk.github.io/ArnoldC/)
        * [`esolang/evil`](https://hub.docker.com/r/esolang/evil/): [Evil](https://esolangs.org/wiki/Evil)
        * [`esolang/js-rhino`](https://hub.docker.com/r/esolang/js-rhino/): [JavaScript (Rhino)](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/Rhino)
        * [`esolang/floater`](https://hub.docker.com/r/esolang/floater/): [Floater](https://esolangs.org/wiki/Floater)
        * [`esolang/cjam`](https://hub.docker.com/r/esolang/cjam/): [CJam](https://sourceforge.net/p/cjam/wiki/Home/)
        * [`esolang/convex`](https://hub.docker.com/r/esolang/convex/): [Convex](https://github.com/GamrCorps/Convex)
        * [`esolang/kotlin`](https://hub.docker.com/r/esolang/kotlin/): [Kotlin](https://kotlinlang.org/)
        * [`esolang/whenever`](https://hub.docker.com/r/esolang/whenever/): [Whenever](http://www.dangermouse.net/esoteric/whenever.html)
    * [`esolang/python2`](https://hub.docker.com/r/esolang/python2/): [Python 2](https://www.python.org/)
        * [`esolang/csharp`](https://hub.docker.com/r/esolang/csharp/): [C# (Mono)](http://www.mono-project.com/)
            * [`esolang/velato`](https://hub.docker.com/r/esolang/velato/): [Velato](https://github.com/rottytooth/Velato)
            * [`esolang/pure-folders`](https://hub.docker.com/r/esolang/pure-folders/): [Pure Folders](https://esolangs.org/wiki/Folders#Pure_Folders)
                * [`esolang/concise-folders`](https://hub.docker.com/r/esolang/concise-folders/): [Concise Folders](https://esolangs.org/wiki/Folders#Concise_Folders)
            * [`esolang/function2d`](https://hub.docker.com/r/esolang/function2d/): [Function](https://esolangs.org/wiki/Funciton)
        * [`esolang/haystack`](https://hub.docker.com/r/esolang/haystack/): [Haystack](https://github.com/kade-robertson/haystack)
        * [`esolang/stuck`](https://hub.docker.com/r/esolang/stuck/): [Stuck](https://esolangs.org/wiki/Stuck)
        * [`esolang/unicat`](https://hub.docker.com/r/esolang/unicat/): [Unicat](https://github.com/gemdude46/unicat)
        * [`esolang/unreadable`](https://hub.docker.com/r/esolang/unreadable/): [Unreadable](https://esolangs.org/wiki/Unreadable)
        * [`esolang/zombie`](https://hub.docker.com/r/esolang/zombie/): [ZOMBIE](http://www.dangermouse.net/esoteric/zombie.html)
        * [`esolang/ffb`](https://hub.docker.com/r/esolang/ffb/): [Foobar and Foobaz and Barbaz, oh my!](https://esolangs.org/wiki/Foobar_and_Foobaz_and_Barbaz,_oh_my!)
        * [`esolang/aubergine`](https://hub.docker.com/r/esolang/aubergine/): [Aubergine](https://esolangs.org/wiki/Aubergine)
        * [`esolang/ubergenes`](https://hub.docker.com/r/esolang/ubergenes/): [UberGenes](https://esolangs.org/wiki/UberGenes)
        * [`esolang/path`](https://hub.docker.com/r/esolang/path/): [PATH](http://pathlang.sourceforge.net/)
        * [`esolang/recurse`](https://hub.docker.com/r/esolang/recurse/): [Recurse](https://esolangs.org/wiki/Recurse)
        * [`esolang/fernando`](https://hub.docker.com/r/esolang/fernando/): [FerNANDo](https://esolangs.org/wiki/FerNANDo)
        * [`esolang/gs2`](https://hub.docker.com/r/esolang/gs2/): [gs2](https://github.com/nooodl/gs2)
        * [`esolang/logicode`](https://hub.docker.com/r/esolang/logicode/): [Logicode](https://github.com/LogicodeLang/Logicode)
        * [`esolang/minimal2d`](https://hub.docker.com/r/esolang/minimal2d/): [Minimal-2D](https://esolangs.org/wiki/Minimal-2D)
        * [`esolang/i4004asm`](https://hub.docker.com/r/esolang/i4004asm/): [Intel 4004 Assembly](https://github.com/CodeAbbey/intel4004-emu)
        * [`esolang/suzy`](https://hub.docker.com/r/esolang/suzy/): [Suzy](http://esolangs.org/wiki/Suzy)
        * [`esolang/bash-pure`](https://hub.docker.com/r/esolang/bash-pure/): [Bash (pure)](https://tiswww.case.edu/php/chet/bash/bashtop.html)
            * [`esolang/bash-busybox`](https://hub.docker.com/r/esolang/bash-busybox/): [Bash (busybox)](https://busybox.net/)
        * [`esolang/fish-shell-pure`](https://hub.docker.com/r/esolang/fish-shell-pure/): [Fish (pure)](https://fishshell.com/)
    * [`esolang/jq`](https://hub.docker.com/r/esolang/jq/): [jq](https://stedolan.github.io/jq/)
    * [`esolang/node`](https://hub.docker.com/r/esolang/node/): [Node.js](https://nodejs.org/)
        * [`esolang/unicue`](https://hub.docker.com/r/esolang/unicue/): [Unicue](https://github.com/hakatashi/tweet-lang)
        * [`esolang/beam`](https://hub.docker.com/r/esolang/beam/): [Beam](http://esolangs.org/wiki/Beam)
        * [`esolang/cubix`](https://hub.docker.com/r/esolang/cubix/): [Cubix](https://github.com/ETHproductions/cubix)
        * [`esolang/japt`](https://hub.docker.com/r/esolang/japt/): [Japt](https://github.com/ETHproductions/japt)
        * [`esolang/stop`](https://hub.docker.com/r/esolang/stop/): [STOP](https://github.com/colinjeanne/stop-lang)
        * [`esolang/htms`](https://hub.docker.com/r/esolang/htms/): [htms](https://github.com/OinkIguana/htms)
        * [`esolang/maybelater`](https://hub.docker.com/r/esolang/maybelater/): [Maybe Later](http://esolangs.org/wiki/Maybe_Later)
        * [`esolang/nadesiko`](https://hub.docker.com/r/esolang/nadesiko/): [なでしこ3](https://nadesi.com/doc3/)
        * [`esolang/floating`](https://hub.docker.com/r/esolang/floating/): [Floating](https://github.com/KPCCoiL/floating-lang)
        * [`esolang/qlb`](https://hub.docker.com/r/esolang/qlb/): [‫قلب‬](https://github.com/nasser/---)
    * [`esolang/octave`](https://hub.docker.com/r/esolang/octave/): [Octave](https://www.gnu.org/software/octave/)
        * [`esolang/matl`](https://hub.docker.com/r/esolang/matl/): [MATL](https://github.com/lmendo/MATL)
    * [`esolang/perl`](https://hub.docker.com/r/esolang/perl/): [Perl](https://www.perl.org/)
        * [`esolang/slashes`](https://hub.docker.com/r/esolang/slashes/): [///](https://esolangs.org/wiki////)
        * [`esolang/element`](https://hub.docker.com/r/esolang/element/): [Element](https://esolangs.org/wiki/Element)
    * [`esolang/php`](https://hub.docker.com/r/esolang/php/): [PHP 7.0](https://secure.php.net/)
        * [`esolang/irc`](https://hub.docker.com/r/esolang/irc/): [IRC](https://esolangs.org/wiki/IRC)
    * [`esolang/python3`](https://hub.docker.com/r/esolang/python3/): [Python 3](https://www.python.org/)
        * [`esolang/exchangeif`](https://hub.docker.com/r/esolang/exchangeif/): [ExchangeIF](https://github.com/HyogaGlacier/ExchangeIF)
        * [`esolang/trumpscript`](https://hub.docker.com/r/esolang/trumpscript/): [TrumpScript](http://samshadwell.me/TrumpScript/)
        * [`esolang/2sable`](https://hub.docker.com/r/esolang/2sable/): [2sable](https://github.com/Adriandmen/2sable)
        * [`esolang/fish`](https://hub.docker.com/r/esolang/fish/): [><>](https://esolangs.org/wiki/Fish)
        * [`esolang/arcyou`](https://hub.docker.com/r/esolang/arcyou/): [Arcyóu](https://github.com/Nazek42/arcyou)
        * [`esolang/bots`](https://hub.docker.com/r/esolang/bots/): [Bots](https://github.com/satos---jp/bots)
        * [`esolang/emoji`](https://hub.docker.com/r/esolang/emoji/): [Emoji](https://esolangs.org/wiki/Emoji)
        * [`esolang/zucchini`](https://hub.docker.com/r/esolang/zucchini/): [Zucchini](https://esolangs.org/wiki/Zucchini)
        * [`esolang/cardinal`](https://hub.docker.com/r/esolang/cardinal/): [Cardinal](https://www.esolangs.org/wiki/Cardinal)
        * [`esolang/hbcht`](https://hub.docker.com/r/esolang/hbcht/): [Half-Broken Car in Heavy Traffic](https://esolangs.org/wiki/Half-Broken_Car_in_Heavy_Traffic)
        * [`esolang/jelly`](https://hub.docker.com/r/esolang/jelly/): [Jelly](https://github.com/DennisMitchell/jelly)
        * [`esolang/jellyfish`](https://hub.docker.com/r/esolang/jellyfish/): [Jellyfish](https://github.com/iatorm/jellyfish)
        * [`esolang/width`](https://hub.docker.com/r/esolang/width/): [Width](https://github.com/stestoltz/Width)
        * [`esolang/asciidots`](https://hub.docker.com/r/esolang/asciidots/): [AsciiDots](http://ajanse.me/asciidots/)
        * [`esolang/picfunge`](https://hub.docker.com/r/esolang/picfunge/): [PicFunge](https://github.com/Liesegang/picfunge)
        * [`esolang/iwashi`](https://hub.docker.com/r/esolang/iwashi/): [Iwashi](https://github.com/Yosshi999/iwashi-lang)
    * [`esolang/vim`](https://hub.docker.com/r/esolang/vim/): [Vim](http://www.vim.org/)
    * [`esolang/cmd`](https://hub.docker.com/r/esolang/cmd/): [cmd.exe](https://en.wikipedia.org/wiki/Cmd.exe)
    * [`esolang/lua`](https://hub.docker.com/r/esolang/lua/): [Lua](https://www.lua.org/)
        * [`esolang/rprogn`](https://hub.docker.com/r/esolang/rprogn/): [Reverse Programmer Notation](https://tehflamintaco.github.io/Reverse-Programmer-Notation/)
    * [`esolang/ocaml`](https://hub.docker.com/r/esolang/ocaml/): [OCaml](http://ocaml.org/)
    * [`esolang/haskell`](https://hub.docker.com/r/esolang/haskell/): [Haskell](https://www.haskell.org/)
    * [`esolang/erlang`](https://hub.docker.com/r/esolang/erlang/): [Erlang](http://erlang.org/)
        * [`esolang/elixir`](https://hub.docker.com/r/esolang/elixir/): [Elixir](https://elixir-lang.org/)
            * [`esolang/05ab1e`](https://hub.docker.com/r/esolang/05ab1e/): [05AB1E](https://github.com/Adriandmen/05AB1E)
* [`esolang/ubuntu-base`](https://hub.docker.com/r/esolang/ubuntu-base/)
    * [`esolang/crystal`](https://hub.docker.com/r/esolang/crystal/): [Crystal](https://crystal-lang.org/)
    * [`esolang/d-dmd`](https://hub.docker.com/r/esolang/d-dmd/): [D (DMD)](https://dlang.org/)
    * [`esolang/d-gdc`](https://hub.docker.com/r/esolang/d-gdc/): [D (GDC)](https://dlang.org/)
    * [`esolang/powershell`](https://hub.docker.com/r/esolang/powershell/): [PowerShell](https://github.com/PowerShell/PowerShell)
    * [`esolang/ruby0.49`](https://hub.docker.com/r/esolang/ruby0.49/): [Ruby 0.49](https://www.ruby-lang.org/)
    * [`esolang/fugue`](https://hub.docker.com/r/esolang/fugue/): [Fugue](https://esolangs.org/wiki/Fugue)
    * [`esolang/x86asm-nasm`](https://hub.docker.com/r/esolang/x86asm-nasm/): [x86 Assembly (nasm)](https://www.nasm.us/)
    * [`esolang/swift`](https://hub.docker.com/r/esolang/swift/): [Swift](https://swift.org/)
    * [`esolang/cpp-clang`](https://hub.docker.com/r/esolang/cpp-clang/): [C++ (Clang)](https://clang.llvm.org/)
    * [`esolang/perl1`](https://hub.docker.com/r/esolang/perl1/): [Perl 1.0](https://www.perl.org/)
    * [`esolang/moo`](https://hub.docker.com/r/esolang/moo/): [moo](https://github.com/moratorium08/moo)
* [`esolang/brainfuck-bfi`](https://hub.docker.com/r/esolang/brainfuck-bfi/): [Brainfuck (BFI)](http://esoteric.sange.fi/brainfuck/impl/interp/BFI.c)

## Notes about some languages

### Bash (pure)

Simulates behavior of "Bash (builtins)" in [Anarchy Golf](http://golf.shinh.org/version.rb).

### Brainfuck (bfi)

Unlike `Brainfuck (esotope)`, this execution simulates behavior of "brainfuck" in [Anarchy Golf](http://golf.shinh.org/l.rb?bf).

To achieve this, I have patched a tricky line to the original code.

```patch
--- BFI.c
+++ BFI.c
@@ -46,6 +46,7 @@
   int pc, args, xc, prog_len, l = 0;
   int x[32768];
   int p[32768];
+  int xxx[1] = {'['};

   FILE *stream, *fopen();
```

## Blacklisted languages

Below are the list of the languages that cannot even do the minimal jobs needed for esolang-battle.

*   ArnorldC
*   Haystack
*   INTERCAL
*   LOGICODE
*   ModanShogi
*   ~English
*   Python 1
*   Seed
*   ///
*   TrumpScript
*   Velato
*   ZOMBIE

## Build images

Prerequires [dobi](https://github.com/dnephin/dobi).

    $ cd /path/to/esolang-box
    $ ruby build.rb
    $ dobi

## Run spec

Tested with Ruby 2.6.0

    $ bundle install
    $ bundle exec rspec
