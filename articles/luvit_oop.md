luvitにおける OOP の研究
====

メタテーブルを素朴に使って多段階にクラスを継承すると、テーブル探索の回数が段階数に正比例して、懲罰的なコストがかかることが[わかっている](https://github.com/kengonakajima/blog/blob/master/articles/luaoo.md) 。

そのコストを回避する工夫が必要だが、Lua界における決定版のやり方はまだない感じである。

最近luvitのLua側ライブラリで使われるようになったOOPでは、正比例コストを回避してるのだろうか、調べる。

luvit では、lib/luvit/core.lua で Objectを定義していて、冒頭に必要なことが全部書いてある。

まず、Objectを継承するすべてのクラスで、ただひとつのメタテーブルを共有する。そのテーブルがObject.metaである。

<pre>
local Object = {}

クラスのインスタンスを作る関数はこれ:
function Object:create()
function Object:new(...)
createが新しいメモリ(からっぽのテーブル)を割り当てる実体。
newは、もし initializeという名前の関数が定義されていたら、それを呼び出すだけ。

これでRubyのクラスと同じ使い勝手になっている。

継承するには、Object:extend関数を使う。

<pre>
function Object:extend()
</pre>





luvitでは、
Object -> Emitter -> Handle -> Stream と継承している:
<pre>
	function Emitter:on(…) 内容  end
    local Handle = Emitter:extend()
    function Handle:addHandlerType(…) 内容 end
    local Stream = Handle:extend()
    function Stream:listen(…) 内容 end
</pre>

Streamのインスタンスがつくられるときはどういう動きになるか。
