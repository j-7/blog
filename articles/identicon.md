identicon
====
02/20/2007 07:56:50 AM


<p><a href="http://www.radiumsoftware.com/0702.html#070201">identicon</a>というすばらしすぎるアイデアがある。</p>

<p>ドメイン名からidenticonを生成してページの左上に表示する<a href="http://d.hatena.ne.jp/tosik/20070204/1170527652">greasemonkeyスクリプト</a>を教えてもらった。</p>

<p>これを使って、このブログ(www.ce-lab.net)を見ると以下のようになる。<br />
<img alt="identicon.png" src="http://www.ce-lab.net/ringo/archives/identicon.png" width="190" height="241" /></p>

<p>この模様が気に入らない！<br />
何とかしたい。</p>

<p>同じ気持ちになる人は多いだろう。<br />
模様になってしまうと、こだわりが出てきてしまう。</p>

<p>identiconと同じ機能を保ちながら、見た目の満足感を得る方法はないのだろうか。</p>

<p>identiconに、セキュリティの機能だけを求めるならば、<br />
「自分にとってフィッシングサイトかどうか」だけがわかればよく、<br />
ほかの人が見たときと異なる模様になってもいいので、<br />
模様をつくるアルゴリズムを、自分専用にカスタマイズすればよい。<br />
しかしそれだと、以下の点で問題である。</p>

<p>1そもそも「他の人にどう見えているか」が重要である<br />
2「あの赤色の三角模様のサイト」とか言えなくなる<br />
3プロジェクタを使って画面を共有するときも多く、混乱する</p>

<p>みんな共通の模様になるほうが良いと思う。<br />
お金の価値と同じで、「他にどう見えているか？」<br />
によってそれ自体の価値が決まるのだ。これからidenticonシェア争いが始まるのだろう。</p>

<p>さて、世界共通のidenticonを保ったまま、見た目の満足感を得るにはどうしたらいいか？</p>

<p>例えば、今回使ったidenticonの生成アルゴリズムが生成できる模様の多様性は、<br />
17ビット分しかない。<br />
しかし重要なのはビット数ではない。<br />
模様が直線的な要素のみで構成されているので、人間のパターン認識能力の、<br />
ごく一部しか使っていないのが問題なのだ。そこに限界があるから、<br />
17ビットを24ビットにしても、人間にとっての多様性は増えにくいと考えられる。</p>

<p>- 曲線を使う。<br />
- 多色を使う。<br />
- 立体的な表現を使う。<br />
- 顔のパターンを使い、顔認識細胞のようなものを使う。<br />
- 文字を使う。<br />
- 自然物（葉っぱとか）の模様を使う。<br />
- 実写写真を使う。<br />
- 動画にする。</p>

<p>などといった応用により、脳の別の部分も活用するように改善する。<br />
もし、そうすることで、多様性を10倍、100倍にまずすることができたら、<br />
各ドメイン管理者が、identicon生成エンジンがどの絵を表示すべきかを<br />
選択できると思う。</p>

<p>数字で言うと、</p>

<p>現在：17ビットの多様性をもつ画像を生成：そのまま受け入れる<br />
改善版：20ビットの多様性をもつ画像を生成：8種類の中から選ぶ</p>

<p>といった具合になる。<br />
あまりにも多くから選べると、元のサイトに似た画像が含まれてしまうかもしれないので、<br />
具体的な落としどころとしては、画像をちょっと大きくして曲線と3色ぐらいを使い、<br />
10種類ぐらいから選べるぐらいがちょうどいいかもしれない。</p>

<p>こういうのをイメージしている：<br />
<a href="http://www.flickr.com/groups/processing/">Flickr group: processing</a></p>

<p>立体的な花を複数自動生成して、ブーケにするとかすると素敵かもしれないなあ。 </p>

<p>追記：<br />
トラックバックにもあったが、<br />
「攻撃者が、ドメイン名を狙って取る」が可能になるという穴は、そう簡単には埋まらなそうだ。<br />
みんなが同じidenticonを見るということがなくても、<br />
攻撃者が何千というドメインを取得すれば、コストは上がるが原理的には防げない。<br />
「ＵＲＬよりはマシ」というものは何かしら可能そうだが、<br />
フィッシングを抜本的に解決というためには使えないだろう。<br />
identiconの用途として、セキュリティは主にはならない気がする。<br />
それでも面白い考え方であることには違いない。<br />
</p>