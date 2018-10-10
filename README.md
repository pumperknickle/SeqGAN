# SeqGAN with keras

## About this
SeqGAN generate sentences similar to a novel, in this example Soseki Natsume's
(Japanese famous novelist) "Kokoro", by adversarial training.

Look at the [paper](https://arxiv.org/abs/1609.05473) for detail.

In this example, disciminator model differs from paper because keras don't support masking in Conv1D, so disciminator uses LSTM here.

## Usage
[main.ipynb](https://github.com/tyo-yo/SeqGAN/blob/master/main.ipynb) shows usage and result.

## Result
Ground truth or Generated data / Discriminator score / Sentence
❎ 0.001: 私は思いつまりもなくなって、そぞろ、話しかけの内はがらんとして辛かったからです。
❎ 0.007: しかしその特色を噛みました。
❎ 0.002: 私はそれを客に見せられます。
❎ 0.002: どっちも私に好かれるためにして来た。
⭕️ 1.000: Ｋは何ともいいませんでしたけれども、自分の所へこの姉から同じような意味の書状が二、三度来たという事を打ち明けました。
❎ 0.000: 先生は無論父の答えをないのかなら、田舎はどっちもした事は滅多に腹の生き
❎ 0.000: 私の親切が私が主張うとなって、これから未亡人というほどの眼で自分の間に成り立っ
❎ 0.000: ですと私がまたずっと下卑た家がある程度以上の抜けやしますね」と話して行きによく
❎ 0.003: 父は大抵むずかしい父を休ませていた。
❎ 0.000: 先生が昨日のようにいてから書物を読みます。なくありますね」と答えて、あまり仰山
❎ 0.000: 先生は奥さんからという場合には、私の素させようという相談をする事もあります。
❎ 0.002: 性質もそれで解って、私を坐らせる方法を講じた。
⭕️ 0.990: 先生の顔には深い一種の表情がありありと刻まれた。
❎ 0.002: 私がこの父の前に懺悔の人であった。
❎ 0.000: Ｋの感情が、すぐどうかしなければならない私の性質でも、もう少しいって、こんな事も多く
❎ 0.003: 私は無論奥にあるものも厭にしました。
❎ 0.000: 比較的上品な嗜好もなく、魔の通るや驚きましたなら、二人で暮して水と山と
❎ 0.001: 私は父も母の早呑み込みでみんなほどありました。
❎ 0.000: 私は突然調子にはいつものない私を軽蔑していられなくなりました。
❎ 0.001: 私はまだ後のない事さえよく先生は、私に足を向けました。
❎ 0.001: 奥さんは奥さんのためによく始末をつけて漸くここに帰った。
❎ 0.003: 世の中では否応なしに東京へ出た。
❎ 0.005: そうして同じところを暇を起しにも感じたらしいのです。
⭕️ 0.970: その時海岸には掛茶屋が二軒あった。
❎ 0.004: 先生は私に何事もまた歩きながらね」と奥さんが聞いた。
❎ 0.000: 「これにいる日は笑い出したけれども、お父さんの行先が再び故の洗い張りや仕立て方が両親を
❎ 0.000: 「仰山仰山」私はその友人に代って結構だ」と母がいった。
❎ 0.204: 父の眼を真向にしても一向ままに付け加えてあまり仰山だか会えない代りにします。
❎ 0.001: するとその上私の相手の希望する必要なのです。
❎ 0.000: ただ私はそうで行くとも仰山だという事を何度になるから、私にいた時の深い
❎ 0.003: 私の自白でそれを切りました。
❎ 0.000: その下へ引っ張って来た時、その翌日に続いてある方からまた相手の医者のために落ち
❎ 0.497: 結婚の申し込みを拒絶されたりしているうちに、Ｋの自尊心にとって大いなかったのです。
❎ 0.000: 私が私を驚かしたものならば、後を往来の事をこうなるだけでした。
⭕️ 0.314: 妻は定めて私といっしょになった顛末を述べてＫに喜んでもらうつもりでしたろう。
⭕️ 1.000: 静かな素人屋に一人で下宿しているのは、かえって家を持つ面倒がなくって結構だろうと考え出したのです。
⭕️ 0.984: 私と妻とは元の通り仲好く暮して来ました。
❎ 0.001: それに海へ引き移って来た私は、これからどうする事になりました。
❎ 0.082: そうした新しい光で父の病状をＫの部屋へよくある点でないからという意味と考えました。
❎ 0.000: しかしそこで一番やろうはずがどこへ出た私には、父と書いて来るまでよく解りまし
❎ 0.000: 奥さんこの沿岸はいつもの通り重い口を上げて父の所へ呼ばれる時、いつもの事もあり
❎ 0.000: つまり妻の自白になるのを、その時分からハイカラで代る代る起きては容易に見えました。
⭕️ 0.955: 私には学校の講義よりも先生の談話の方が有益なのであった。
❎ 0.005: 実際それがための貴重な時間であった。
❎ 0.000: 私は無論父やそういう点について、この間のものなら、東京へ立つ日取りを受けた私を解釈し
❎ 0.007: それでこの仕事が済んですがあった。
❎ 0.000: その中に理解さもせるのはを比較彼の根を見ているのです。
⭕️ 0.977: 私はぼんやりその前に立って、また縄を解こうかと考えた。
❎ 0.002: しかし奥さんの方は段々動かずにいなくなった。
⭕️ 0.966: 私は先生の風邪を実際軽く見ていたので。
❎ 0.000: 私も腹の付いた後、——母は自分の方で暮らすといった風に心を好いであった


## Requirements
- Python 3.6.6
- Keras==2.2.2
- tensorflow==1.10.0


## Test
> python setup.py test
