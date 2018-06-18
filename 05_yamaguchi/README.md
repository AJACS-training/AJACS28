
<h2>AJACS28/atsuko</h2>

<div class="body">
	<div class="section">
<hr class="full_hr" />
<p>目次</p>
<div class="contents">
<a id="contents_1"></a>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="#s9ce7df0">  DBCLS Galaxy について </a></li>
<li><a href="#n676bfcb">  TogoDB について </a></li>
<li><a href="#za2d3e8d">  実習方法 </a></li>
<li><a href="#k5432b73"> 【実習1】DBCLS Galaxy </a></li>
<li><a href="#g58d8116"> 【実習2】TogoDB </a></li></ul>
</div>

<hr class="full_hr" />
<h3 id="content_1_0"><a id="s9ce7df0" href="" title="s9ce7df0"><span class="sanchor">_</span></a> DBCLS Galaxy について  </h3>
<p><a href="http://galaxy.dbcls.jp/" rel="nofollow">http://galaxy.dbcls.jp/</a></p>
<p>Galaxy とは，ゲノムなどの生物学データを対象とした，データ解析，共有，公開のためのインタフェイスです．DBCLS Galaxy は，日本国内の生物学研究者をターゲットにして，カスタマイズを加えた Galaxy です．</p>
<p>今回の実習では，Amazon EC2 上に構築した DBCLS Galaxy を利用します．小グループにわかれ，データアップロード，ツール利用，共有を体験していただく予定です．</p>

<h3 id="content_1_1"><a id="n676bfcb" href="" title="n676bfcb"><span class="sanchor">_</span></a> TogoDB について  </h3>
<p><a href="http://togodb.dbcls.jp/" rel="nofollow">http://togodb.dbcls.jp/</a></p>
<p>チュートリアル:
<a href="https://www.evernote.com/shard/s1/sh/a4685655-53d4-4b0f-88bd-0d79518caa47/6efe72502215e37b974e308a41dd733f" rel="nofollow">https://www.evernote.com/shard/s1/sh/a4685655-53d4-4b0f-88bd-0d79518caa47/6efe72502215e37b974e308a41dd733f</a></p>
<p>TogoDB とは，簡単に検索などの基本機能付きデータベースが構築・公開できるサービスです．今回は
<a href="http://semantic.togodb.dbcls.jp/" rel="nofollow">http://semantic.togodb.dbcls.jp/</a>
を利用し，DBCLS Galaxy の実習でできたデータをWWW上で公開します．</p>

<h3 id="content_1_2"><a id="za2d3e8d" href="" title="za2d3e8d"><span class="sanchor">_</span></a> 実習方法  </h3>
<p>3名ごとのグループを作ります．1つのグループに 1 つの DBCLS Galaxy サーバと 3つの DBCLS OpenID を割当てます．各自，自分が触るサーバと割当てられた OpenID を確認してください．</p>
<p>(実習直前にここに書き込み，直後に消去します)</p>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>サーバ1: <a href="http://ec2-184-72-57-227.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-184-72-57-227.us-west-1.compute.amazonaws.com:37180/</a></li>
<li>サーバ2: <a href="http://ec2-204-236-167-40.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-204-236-167-40.us-west-1.compute.amazonaws.com:37180/</a></li>
<li>サーバ3: <a href="http://ec2-50-18-132-70.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-50-18-132-70.us-west-1.compute.amazonaws.com:37180/</a></li>
<li>サーバ4: <a href="http://ec2-204-236-178-175.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-204-236-178-175.us-west-1.compute.amazonaws.com:37180/</a></li>
<li>サーバ5: <a href="http://ec2-204-236-159-29.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-204-236-159-29.us-west-1.compute.amazonaws.com:37180/</a></li>
<li>サーバ6: <a href="http://ec2-50-18-240-181.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-50-18-240-181.us-west-1.compute.amazonaws.com:37180/</a></li>
<li>サーバ7: <a href="http://ec2-50-18-140-242.us-west-1.compute.amazonaws.com:37180/" rel="nofollow">http://ec2-50-18-140-242.us-west-1.compute.amazonaws.com:37180/</a></li></ul>

<h3 id="content_1_3"><a id="k5432b73" href="" title="k5432b73"><span class="sanchor">_</span></a> 【実習1】DBCLS Galaxy  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>1. サーバにアクセスします．</li>
<li>2. 自分に割当てられたOpenIDでログインします．</li>
<li>3. 解析に使うデータを取得します
<ul class="list2" style="padding-left:16px;margin-left:16px"><li>3-1. 自分の手持ちのデータのアップロード
<ul class="list3" style="padding-left:16px;margin-left:16px"><li>テキストエディタでデータを作ってアップロードしてみましょう．</li></ul></li>
<li>3-2. 公開されているデータベースからデータを取得
<ul class="list3" style="padding-left:16px;margin-left:16px"><li>条件を選んでデータベースからデータを取得してみましょう．人の染色体22番に含まれる exon の区間データを全部取得します．</li></ul></li></ul></li></ul>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>4. 簡単な解析をします．
<ul class="list2" style="padding-left:16px;margin-left:16px"><li>exonのデータを長さでフィルタします(長さ100以上のものだけにする)</li>
<li>exon の長さを計算して，実際に100以上のものだけが残っていることを確認します</li></ul></li>
<li>5. 計算履歴を共有します
<ul class="list2" style="padding-left:16px;margin-left:16px"><li>計算履歴を同じグループ内の他のユーザと共有します</li></ul></li></ul>

<h3 id="content_1_4"><a id="g58d8116" href="" title="g58d8116"><span class="sanchor">_</span></a> 【実習2】TogoDB  </h3>
<ul class="list2" style="padding-left:32px;margin-left:32px"><li>実習1の結果をダウンロードします</li>
<li>tsvからcsvに<span class="noexists">OpenOffice<a href="http://MotDB.DBCLS.jp/?cmd=edit&amp;page=OpenOffice&amp;refer=AJACS28%2Fatsuko">?</a></span> Calc, MS Excel, Google Doc などを利用して変換します</li>
<li>サーバにアクセスして，実習1の結果を公開するデータベースを構築します．</li></ul>
