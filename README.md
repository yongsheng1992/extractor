# Extractor
一个简单的HTML文档正文提取工具。

## 使用
``` bash
$ git clone https://github.com/yongsheng1992/extractor.git
$ cd extractor
$ ipython
In [1]: from extractor import Article

In [2]: import requests

In [3]: url = 'http://news.sina.com.cn/china/xlxw/2017-10-18/doc-ifymzqpq2122603.shtml'

In [4]: resp = requests.get(url)

In [5]: article = Article(resp.content)

In [6]: article.text
Out[6]: '原标题：中国共产党第十九次全国代表大会在京开幕 习近平代表第十八届中央委员会向大会作报告 李克强主持大会2338名代表和特邀代表出席大会\n新华社北京10月18日电 绘就伟大梦想新蓝图，开启伟大事业新时代。举世瞩目的中国共产党第十九次全国代表大会18日上午在人民大会堂开幕。\n习近平代表第十八届中央委员会向大会作了题为《决胜全面建成小康社会夺取新时代中国特色社会主义伟大胜利》的报告。习近平指出，中国共产党第十九次全国代表大会，是在全面建成小康社会决胜阶段、中国特色社会主义进入新时代的关键时期召开的一次十分重要的大会。大会的主题是：不忘初心，牢记使命，高举中国特色社会主义伟大旗帜，决胜全面建成小康社会，夺取新时代中国特色社会主义伟大胜利，为实现中华民族伟大复兴的中国梦不懈奋斗。\n人民大会堂雄伟庄严，万人大礼堂气氛热烈。主席台上方悬挂着“中国共产党第十九次全国代表大会”的会标，后幕正中是镰刀和锤头组成的党徽，10面鲜艳的红旗分列两侧。二楼和三楼眺台上分别悬挂着“不忘初心，牢记使命，高举中国特色社会主义伟大旗帜，决胜全面建成小康社会，夺取新时代中国特色社会主义伟大胜利，为实现中华民族伟大复兴的中国梦不懈奋斗！”“伟大、光荣、正确的中国共产党万岁！”的横幅。\n在主席台前排就座的大会主席团常务委员会成员有习近平、李克强、张德江、俞正声、刘云山、王岐山、张高丽、马凯、王沪宁、刘延东、刘奇葆、许其亮、孙春兰、李建国、李源潮、汪洋、张春贤、范长龙、孟建柱、赵乐际、胡春华、栗战书、郭金龙、韩正、江泽民、胡锦涛、李鹏、朱镕基、李瑞环、吴邦国、温家宝、贾庆林、宋平、李岚清、曾庆红、吴官正、李长春、贺国强、杜青林、赵洪祝、杨晶。\n大会由李克强主持。上午9时，会议开始。全场起立，高唱《中华人民共和国国歌》。随后，全体同志为毛泽东、周恩来、刘少奇、朱德、邓小平、陈云等已故老一辈无产阶级革命家和革命先烈默哀。\n李克强宣布，党的十九大应出席代表2280人，特邀代表74人，共2354人，今天实到2338人。他对列席大会的党外朋友和有关方面负责同志表示热烈的欢迎。\n习近平代表第十八届中央委员会向大会作的报告共分13个部分：一、过去五年的工作和历史性变革；二、新时代中国共产党的历史使命；三、新时代中国特色社会主义思想和基本方略；四、决胜全面建成小康社会，开启全面建设社会主义现代化国家新征程；五、贯彻新发展理念，建设现代化经济体系；六、健全人民当家作主制度体系，发展社会主义民主政治；七、坚定文化自信，推动社会主义文化繁荣兴盛；八、提高保障和改善民生水平，加强和创新社会治理；九、加快生态文明体制改革，建设美丽中国；十、坚持走中国特色强军之路，全面推进国防和军队现代化；十一、坚持“一国两制”，推进祖国统一；十二、坚持和平发展道路，推动构建人类命运共同体；十三、坚定不移全面从严治党，不断提高党的执政能力和领导水平。\n习近平在报告中指出，十八大以来的五年，我们坚持稳中求进工作总基调，迎难而上，开拓进取，取得了改革开放和社会主义现代化建设的历史性成就，党和国家事业全面开创新局面：经济建设取得重大成就；全面深化改革取得重大突破；民主法治建设迈出重大步伐；思想文化建设取得重大进展；人民生活不断改善；生态文明建设成效显著；强军兴军开创新局面；港澳台工作取得新进展；全方位外交布局深入展开；全面从严治党成效卓著。同时，必须清醒看到，我们的工作还存在许多不足，也面临不少困难和挑战。\n习近平说，五年来的成就是全方位的、开创性的，五年来的变革是深层次的、根本性的。五年来，我们党以巨大的政治勇气和强烈的责任担当，提出一系列新理念新思想新战略，出台一系列重大方针政策，推出一系列重大举措，推进一系列重大工作，解决了许多长期想解决而没有解决的难题，办成了许多过去想办而没有办成的大事，推动党和国家事业发生历史性变革。这些历史性变革，对党和国家事业发展具有重大而深远的影响。\n习近平指出，经过长期努力，中国特色社会主义进入了新时代，这是我国发展新的历史方位。这标志着我国社会主要矛盾已经转化为人民日益增长的美好生活需要和不平衡不充分的发展之间的矛盾。我国社会主要矛盾的变化，没有改变我们对我国社会主义所处历史阶段的判断，我国仍处于并将长期处于社会主义初级阶段的基本国情没有变，我国是世界最大发展中国家的国际地位没有变。\n习近平强调，全党要牢牢把握社会主义初级阶段这个基本国情，牢牢立足社会主义初级阶段这个最大实际，牢牢坚持党的基本路线这个党和国家的生命线、人民的幸福线，领导和团结全国各族人民，以经济建设为中心，坚持四项基本原则，坚持改革开放，自力更生，艰苦创业，为把我国建设成为富强民主文明和谐美丽的社会主义现代化强国而奋斗。\n关于新时代中国共产党的历史使命，习近平指出，实现中华民族伟大复兴是近代以来中华民族最伟大的梦想。中国共产党一经成立，就把实现共产主义作为党的最高理想和最终目标，义无反顾肩负起实现中华民族伟大复兴的历史使命。今天，我们比历史上任何时期都更接近、更有信心和能力实现中华民族伟大复兴的目标。\n习近平强调，实现伟大梦想，必须进行伟大斗争；实现伟大梦想，必须建设伟大工程；实现伟大梦想，必须推进伟大事业。伟大斗争，伟大工程，伟大事业，伟大梦想，紧密联系、相互贯通、相互作用，其中起决定性作用的是党的建设新的伟大工程。\n习近平用“八个明确”对新时代中国特色社会主义思想进行了阐述。他说，新时代中国特色社会主义思想明确坚持和发展中国特色社会主义，总任务是实现社会主义现代化和中华民族伟大复兴，在全面建成小康社会的基础上，分两步走在本世纪中叶建成富强民主文明和谐美丽的社会主义现代化强国。\n习近平指出，新时代中国特色社会主义思想，是对马克思列宁主义、毛泽东思想、邓小平理论、“三个代表”重要思想、科学发展观的继承和发展，是马克思主义中国化最新成果，是党和人民实践经验和集体智慧的结晶，是中国特色社会主义理论体系的重要组成部分，是全党全国人民为实现中华民族伟大复兴而奋斗的行动指南，必须长期坚持并不断发展。\n习近平阐述了构成新时代坚持和发展中国特色社会主义基本方略的“十四条坚持”：坚持党对一切工作的领导；坚持以人民为中心；坚持全面深化改革；坚持新发展理念；坚持人民当家作主；坚持全面依法治国；坚持社会主义核心价值体系；坚持在发展中保障和改善民生；坚持人与自然和谐共生；坚持总体国家安全观；坚持党对人民军队的绝对领导；坚持“一国两制”和推进祖国统一；坚持推动构建人类命运共同体；坚持全面从严治党。\n习近平在谈到“两个一百年”奋斗目标时说，改革开放之后，我们党对我国社会主义现代化建设作出战略安排，提出“三步走”战略目标。解决人民温饱问题、人民生活总体上达到小康水平这两个目标已提前实现。从现在到二〇二〇年，是全面建成小康社会决胜期。从十九大到二十大，是“两个一百年”奋斗目标的历史交汇期。我们既要全面建成小康社会、实现第一个百年奋斗目标，又要乘势而上开启全面建设社会主义现代化国家新征程，向第二个百年奋斗目标进军。\n习近平提出，从二〇二〇年到本世纪中叶可以分两个阶段来安排。第一个阶段，从二〇二〇年到二〇三五年，在全面建成小康社会的基础上，再奋斗十五年，基本实现社会主义现代化。第二个阶段，从二〇三五年到本世纪中叶，在基本实现现代化的基础上，再奋斗十五年，把我国建成富强民主文明和谐美丽的社会主义现代化强国。\n习近平指出，要贯彻新发展理念，建设现代化经济体系。深化供给侧结构性改革；加快建设创新型国家；实施乡村振兴战略；实施区域协调发展战略；加快完善社会主义市场经济体制；推动形成全面开放新格局。\n习近平阐述了健全人民当家作主制度体系，发展社会主义民主政治的内容：一是坚持党的领导、人民当家作主、依法治国有机统一；二是加强人民当家作主制度保障；三是发挥社会主义协商民主重要作用；四是深化依法治国实践；五是深化机构和行政体制改革；六是巩固和发展爱国统一战线。\n习近平指出，要坚定文化自信，推动社会主义文化繁荣兴盛。牢牢掌握意识形态工作领导权；培育和践行社会主义核心价值观；加强思想道德建设；繁荣发展社会主义文艺；推动文化事业和文化产业发展。\n习近平强调，要提高保障和改善民生水平，加强和创新社会治理。优先发展教育事业；提高就业质量和人民收入水平；加强社会保障体系建设；坚决打赢脱贫攻坚战；实施健康中国战略；打造共建共治共享的社会治理格局；有效维护国家安全。\n习近平提出，要加快生态文明体制改革，建设美丽中国。推进绿色发展；着力解决突出环境问题；加大生态系统保护力度；改革生态环境监管体制。\n习近平指出，坚持走中国特色强军之路，全面推进国防和军队现代化。必须全面贯彻新时代党的强军思想，贯彻新形势下军事战略方针，建设强大的现代化陆军、海军、空军、火箭军和战略支援部队，打造坚强高效的战区联合作战指挥机构，构建中国特色现代作战体系，担当起党和人民赋予的新时代使命任务。\n习近平指出，要坚持“一国两制”，推进祖国统一。保持香港、澳门长期繁荣稳定，支持香港、澳门融入国家发展大局，发展壮大爱国爱港爱澳力量，让香港、澳门同胞同祖国人民共担民族复兴的历史责任、共享祖国繁荣富强的伟大荣光。继续坚持“和平统一、一国两制”方针，推动两岸关系和平发展，推进祖国和平统一进程。坚决维护国家主权和领土完整，绝不容忍国家分裂的历史悲剧重演。\n习近平指出，坚持和平发展道路，推动构建人类命运共同体。中国将高举和平、发展、合作、共赢的旗帜，恪守维护世界和平、促进共同发展的外交政策宗旨，坚定不移在和平共处五项原则基础上发展同各国的友好合作，推动建设相互尊重、公平正义、合作共赢的新型国际关系。\n习近平强调，坚定不移全面从严治党，不断提高党的执政能力和领导水平。\n习近平提出了新时代党的建设总要求以及必须抓好的八个方面重要任务：把党的政治建设摆在首位；用新时代中国特色社会主义思想武装全党；建设高素质专业化干部队伍；加强基层组织建设；持之以恒正风肃纪；夺取反腐败斗争压倒性胜利；健全党和国家监督体系；全面增强执政本领。\n习近平报告过程中，全场一次次响起热烈的掌声。\n现任和曾任全国人大常委会副委员长、全国政协副主席的党外人士，在京各民主党派中央、全国工商联副主席，无党派代表人士，宗教界代表人士，在京全国人大、全国政协常委中的民主党派、无党派和民族宗教界人士作为来宾列席大会。党内有关负责同志也列席了大会。\n3000多名中外记者采访报道了开幕会盛况。\n责任编辑：刘光博 '

In [7]:

```