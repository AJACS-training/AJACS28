
<h2>AJACS28/fujieda</h2>

<div class="body">
	<div class="section">
<hr class="full_hr" />
<p>目次</p>
<div class="contents">
<a id="contents_1"></a>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="#vd6d6235">  BodyParts3D/Anatomographyとは </a></li>
<li><a href="#da6d0127">  BodyParts3D/Anatomographyの場所 </a></li>
<li><a href="#j358ae2f"> 【実習1】基本的な操作手順を覚える </a></li>
<li><a href="#q8b55583"> 【実習2】ヒートマップをつくる </a></li>
<li><a href="#e59335d2">  【実習３】質問コーナー！作りたい画像をつくってみてください！</a></li>
<li><a href="#l9cb2248">  講習会資料(pdf)ダウンロード </a></li></ul>
</div>

<hr class="full_hr" />
<h3 id="content_1_0"><a id="vd6d6235" href="" title="vd6d6235"><span class="sanchor">_</span></a> BodyParts3D/Anatomographyとは  </h3>
<p>BodyParts3D(ボディパーツ3D)は人体各部位の位置や形状を3次元モデルで記述したデータベースです。Anatomography(アナトモグラフィー)を使って、BodyParts3Dから解剖学用語を選択して自由に人体のモデル図を作成できます。</p>

<h3 id="content_1_1"><a id="da6d0127" href="" title="da6d0127"><span class="sanchor">_</span></a> BodyParts3D/Anatomographyの場所  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li><a href="http://lifesciencedb.jp" rel="nofollow">統合データベースプロジェクト</a>の「ツール＆解析サービス」から。</li>
<li><a href="http://lifesciencedb.jp/bp3d" rel="nofollow">トップページURL (http://lifesciencedb.jp/bp3d)</a></li>
<li><a href="http://www.google.co.jp/search?q=BodyParts3D&amp;ie=utf-8&amp;oe=utf-8&amp;aq=t&amp;hl=ja&amp;client=firefox-a&amp;rlz=1R1GGGL_ja___JP322" rel="nofollow">「BodyParts3D or Anatomography or アナトモグラフィー」でgoogle検索</a></li></ul>

<h3 id="content_1_2"><a id="j358ae2f" href="" title="j358ae2f"><span class="sanchor">_</span></a> 【実習1】基本的な操作手順を覚える  </h3>
<ul class="list1" style="padding-left:16px;margin-left:16px"><li>「Information」タブ→「ユーザガイド」→「<a href="http://lifesciencedb.jp/bp3d/info/userGuide/gettingStarted/index.html" rel="nofollow">Getting Started</a>」をひと通り実施します。</li></ul>
<p>他：pin、Legend、格子について</p>
<p>　詳しくは、【統合TV】
<a href="http://togotv.dbcls.jp/20111130.html#p01" rel="nofollow">http://togotv.dbcls.jp/20111130.html#p01</a>を参照してください。</p>

<h3 id="content_1_3"><a id="q8b55583" href="" title="q8b55583"><span class="sanchor">_</span></a> 【実習2】ヒートマップをつくる  </h3>
<p><strong>方法1</strong>：臓器別数値を臓器ごとに手入力する</p>
<p>　　　　心臓　1500</p>
<p>　　　　小腸　1200</p>
<p>　　　　大腸　610</p>
<p>　　　　肝臓　230</p>
<p>このようなデータを用いてヒートマップを作成する。</p>
<p>　１．各臓器をPalletに加えます。→臓器の画像をドラッグすると追加できます。</p>
<p>　２．Anatomographyをクリック。</p>
<p>　３．MAPをクリックします。→パレットにValueが追加される。</p>
<p>　４．Valueに数値を入力していく。</p>
<p>　５．Window controlsを開きます。</p>
<p>　６．Heat mapのMaxとMinに最高値、最低値を入力する。（ディフォルト　最高値：65535、最低値：-35535）</p>
<p>　７．Valueに入力した数値によって、臓器が色分けされる。
赤→最大値、青→最少値</p>
<p><strong>方法2</strong>：臓器別数値を一括入力する（エクセルなどの表になっている臓器名と数値データをコピペする）</p>
<p>ヒトアルブミンの臓器別遺伝子発現量を人体ヒートマップで表示し発現状況を可視化する。</p>
<p>　１.　<a href="http://refex.dbcls.jp/index.php?lang=ja&amp;db=human" rel="nofollow">RefExStarted</a>を使ってアルブミンの発現量をさがす。</p>
<p>　２.　Quick Searchでキイワード&quot;alb&quot;を入力→　Search</p>
<p>　３.　1　NM_000477　albumin・・・をクリック→アルブミンの詳細情報ページが開かれる。</p>
<p>　　相対発現量をみる</p>
<p>　　EST、Gene Chip、CAGE、RNA-seqによるそれぞれの組織別発現量が表示されている</p>
<p>ここまでは、先ほどやっていただいた手順です。</p>
<p>　４.　Gene Chipのデータ組織10分類発現データを表にまとめたもの。</p>
<div class="ie5"><table class="style_table" cellspacing="1" border="0"><tbody><tr><td class="style_td">臓器名</td><td class="style_td">発現値</td></tr><tr><td class="style_td">Nervous system</td><td class="style_td">3.06</td></tr><tr><td class="style_td">cardiovascular system</td><td class="style_td">3.1</td></tr><tr><td class="style_td">connective tissue</td><td class="style_td">3.17</td></tr><tr><td class="style_td">reproductive system</td><td class="style_td">3.07</td></tr><tr><td class="style_td">muscular system</td><td class="style_td">3.41</td></tr><tr><td class="style_td">digestive system</td><td class="style_td">3.88</td></tr><tr><td class="style_td">liver</td><td class="style_td">13.72</td></tr><tr><td class="style_td">lung</td><td class="style_td">3.1</td></tr><tr><td class="style_td">kidney</td><td class="style_td">7.74</td></tr><tr><td class="style_td">endocrine</td><td class="style_td">4.27</td></tr></tbody></table></div>
<p>　５.　Anatomographyをクリック。</p>
<p>　６.　MAPをクリックします。→パレットにValueが追加され、ヒートマップバリューバーが出てくる。</p>
<p>　７.　Pasteアイコンをクリックする。</p>
<p>　８.　表をコピペする。</p>
<p>　　　臓器名→English、発現量→Value　→　OKをクリックする。　</p>
<p>描画が出てきたら
筋肉が全身に覆われていて内臓が見えないので筋肉の透明度を0.1にする。</p>
<ol class="list2" style="padding-left:32px;margin-left:32px"><li>作成済みヒートマップ1→
<a href="http://lifesciencedb.jp/bp3d/IM/image.cgi?shorten=81j0vmbqG5HDb45LrmLrWLLr" rel="nofollow">作製済みマップのリンク1</a></li></ol>
<ol class="list2" style="padding-left:32px;margin-left:32px"><li>こちらも試してみてください！</li></ol>
<p>　Gene Chipのアルブミン臓器別発現量抜粋（消化器系の数値を細かく分けたデータ）</p>
<div class="ie5"><table class="style_table" cellspacing="1" border="0"><tbody><tr><td class="style_td">english</td><td class="style_td">value</td></tr><tr><td class="style_td">stomach</td><td class="style_td">2.94</td></tr><tr><td class="style_td">small intestine</td><td class="style_td">4.33</td></tr><tr><td class="style_td">duodenum</td><td class="style_td">8.79</td></tr><tr><td class="style_td">jejunum</td><td class="style_td">3.0 4</td></tr><tr><td class="style_td">colon</td><td class="style_td">2.98</td></tr><tr><td class="style_td">colon cecum</td><td class="style_td">2.94</td></tr><tr><td class="style_td">liver</td><td class="style_td">13.72</td></tr><tr><td class="style_td">lung</td><td class="style_td">3.10</td></tr><tr><td class="style_td">kidney</td><td class="style_td">7.54</td></tr><tr><td class="style_td">pancreas</td><td class="style_td">10.48</td></tr></tbody></table></div>
<div class="spacer">&nbsp;</div>
<ol class="list2" style="padding-left:32px;margin-left:32px"><li>作成済みヒートマップ2→
<a href="http://lifesciencedb.jp/bp3d/IM/image.cgi?shorten=9rqy0zuCiGbGzSb4PTGH99Pz" rel="nofollow">作製済みマップのリンク2臓器のみ</a>、<a href="http://lifesciencedb.jp/bp3d/IM/image.cgi?shorten=THPb0fL5zKPvP19LjuO11z09" rel="nofollow">作製済みマップのリンク2骨格を挿入</a></li></ol>
<p>　　（全身を表示したいときは、骨格系や皮膚を挿入する。）</p>

<h3 id="content_1_4"><a id="e59335d2" href="" title="e59335d2"><span class="sanchor">_</span></a> 【実習３】質問コーナー！作りたい画像をつくってみてください！ </h3>
