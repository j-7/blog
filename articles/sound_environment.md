ソフトウェア開発と、作業場の音環境
====
05/08/2006 08:54:01 AM


<p>連休中、1日だけ京都に行くことがあったのだが、<br />
そのとき<a href="http://www.aritsugu.com/">「有次」</a>という老舗の刃物鍛冶屋に立ち寄った。</p>

<p>その店でいろいろな刃物を見ているとき、さまざまな「作業の音」が耳に入ってきていて、<br />
それが店の雰囲気を作っていることに気づいた。刃物鍛冶屋では、<br />
鍋の底を金づちでカンカン叩く音、回転やすりのゴーゴーと回る音、<br />
大根おろしを作るために金属の針で金属板をギリギリひっかく音、<br />
包丁を紙やすりでシュッシュッと仕上げる音、万力をコリコリと調整する音など、<br />
さまざまな音が混ざった状態で聞こえてくる。<br />
お客さんに対応している年長の職人は、お客さんと話しをしつつも店の音に聞き耳をたてていて、<br />
若いエンジニアが作業手順を間違っていないかどうかチェックしているようだ。</p>

<p>ソフトウェア開発の現場は、鍛冶屋とは異なり、みんなが集中していればしているほど、静かだ。<br />
音といえば、キーボードを叩く音とＰＣのファンが回る音ぐらいのもので、<br />
ちょっと離れると聞こえなくなるほど小さいし、ＰＣのファンはずっと一定の音を出しているので、<br />
変化としてはとらえることができない。ゲーム開発の現場でも<br />
テスト用モニターの音量は最小にしておくのが通例だ。</p>

<p>音は、光と異なり、音源の方向を向いていなくても感知でき、<br />
さらにちょっと意識すれば音源の方向を把握できるという、<br />
独特の特徴を持っている。作業場（オフィス）においては、<br />
仕事仲間の動きを、自分の手を止めたり、視線を動かさずに、<br />
「なんとなく知る」ために、作業音が役に立っている可能性がある。<br />
仮にソフトウエア開発の現場に、作業音による状況把握のしくみを<br />
持ち込むとしたらどんな感じだろうか。試しに、鍛冶屋になぞらえて想像してみる。</p>

<p>やはり、ソースコードをバリバリ書いているときは、<br />
金槌でガンガン叩いているだろう。これは8時間のうち最大でも1時間ぐらいだろうか。<br />
デバッガを使ってメモリの内容を微修正しているときは、<br />
紙やすりでシュッシュっと微修正だ。例外が発生したら、金属板をペキッと割った音がする。<br />
エディタを開閉すると箱を開閉する音がする。でかいファイルだと音もでかい。<br />
もちろん、エディタの種類によって音が異なる。<br />
コンパイル中は機械が活躍しているので、エンジンの音がしても良い。<br />
Warningが出たら、バックファイアのパンパンという音が出てしまう。<br />
巨大なコンパイルをするとエンジンは高回転になる。<br />
プロファイラを利用してベンチマークを調べているときは、<br />
メジャーをカリカリと伸ばす音がする。UNIXコマンドを入力しているときは、<br />
ドライバーでねじを回す音がする。<br />
コードをばっさりと削除したら、ノコギリでぎこぎこ。削除した量によって音の長さや大きさが変化する。<br />
ファイルを削除したら、くしゃくしゃと紙を丸める音がする（macosはそうだった。）<br />
数ギガもあるディレクトリを削除したときは、ドドドという音とともに流れていく。</p>

<p>ソフトウェアの場合は、鍛冶屋ではなく、建設現場のような雰囲気のほうが合っているかもしれない。</p>

<p>こういった音を発生するデバイスをすべての端末につけて、<br />
自分ではなく自分とは反対の方向に音が出るように設置しておく。<br />
作業場がうるさすぎるとストレスになるから、<br />
音量や音の内容には注意する必要があるが、<br />
音量は各自がその日の気分や担当などに応じて、自由に調整したらよいだろう。<br />
あるいは、若いエンジニアは、まだ学習途上だから、<br />
あえて音を大きく聞こえるようにして、年長者のアドバイスを<br />
もらいやすい環境を作るのも良いかもしれない。<br />
ステルス作業をして、ほかのスタッフを驚かせたい場合は、無音に設定してもよいだろう。</p>

<p>音による情報共有は、まだまだハックされてないのではないか。</p>
