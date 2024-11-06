<!--lint disable awesome-heading-->

<p align="center">
  <a href="https://github.com/kdeldycke/awesome-falsehood/">
    <img src="https://github.com/kdeldycke/awesome-falsehood/raw/main/assets/awesome-falsehood-header.jpg" alt="Awesome Falsehood header image">
  </a>
</p>

<p align="center">
  <a href="https://github.com/sponsors/kdeldycke">
    <strong>产品展示!</strong>
    <br/>
    <sup>使用GitHub赞助可以在这添加你的公司或产品链接.</sup>
  </a>
</p>

---

<p align="center">
  <a href="https://github.com/kdeldycke/awesome-falsehood#readme.md" hreflang="en"><img src="https://img.shields.io/badge/lang-English-blue?style=flat-square" lang="en" alt="English"></a>
  <a href="https://github.com/kdeldycke/awesome-falsehood/blob/main/readme.zh.md" hreflang="zh"><img src="https://img.shields.io/badge/lang-中文-blue?style=flat-square" lang="zh" alt="中文"></a>
</p>

<p align="center">
  <i>世界的逻辑在所有真理和虚假之前.</i><br>
  — 路德维希·维特根斯坦<sup id="intro-quote-ref"><a href="#intro-quote-def">[1]</a></sup>
</p>

一个精心策划的 [![Awesome](https://awesome.re/badge-flat.svg)](https://github.com/sindresorhus/awesome) 程序员谬误清单.  *谬误* 指的是你最初相信的 *观点*,但是它被证明是错的.

举个例子, 一个*观点*: 有效的电子邮件地址恰好有一个 `@` 字符. 因此，你会使用这个规则来实现你的电子邮件字段验证逻辑。对吗？错了！  *实际* 是: 电子邮件可以有多个 `@` 字符. 
因此，你的实现应该允许这种情况。最初的*观点*是你曾经相信的一个谬误.

下面列出的*谬误*文章将提供一个全面的列表，帮助你了解这些错误信念，以便让你成为一个更优秀的程序员.

## 目录

<!-- mdformat-toc start --slug=github --no-anchors --maxlevel=6 --minlevel=2 -->

- [元](#元)
- [艺术](#艺术)
- [业务](#业务)
- [加密货币](#加密货币)
- [日期和时间](#日期和时间)
- [教育](#教育)
- [邮件](#邮件)
- [地理](#地理)
- [人类身份](#人类身份)
- [国际化](#国际化)
- [管理](#管理)
- [多媒体](#多媒体)
- [网络](#网络)
- [电话号码](#电话号码)
- [邮政编码](#邮政编码)
- [科学](#科学)
- [社会](#社会)
- [软件工程](#软件工程)
- [交通](#交通)
- [排版](#排版)
- [视频游戏](#视频游戏)
- [Web](#web)

<!-- mdformat-toc end -->

## 元

- [程序员的谬误](https://spaceninja.com/2015/12/07/falsehoods-programmers-believe/) - 常见谬误的简要清单. 对谬误世界的精彩概述与快速入门介绍.
- [编程的谬误](https://chiselapp.com/user/ttmrichter/repository/gng/doc/trunk/output/falsehoods.html) - 让程序员有点丢人但有趣谬误列表.
- [对谬误列表的误解](https://kevin.deldycke.com/2016/falsehoods-programmers-believe-about-falsehoods-lists) - "不应该这么对待谬误的说明".

## 艺术

- [音乐的谬误](https://literateprogrammer.blogspot.fr/2016/07/falsehoods-programmers-believe-about.html) - 在编纂音乐时可能产生的错误假设.
- [艺术的谬误](http://artsy.github.io/blog/2018/04/18/programmer-misconceptions-about-art/) - 对艺术的常见误解.

## 业务

- [网上购物的谬误](https://wiesmann.codiferes.net/wordpress/archives/22201) - 涵盖价格、货币和库存.
- [价格谬误](https://gist.github.com/rgs/6509585) - 涵盖货币、金额和本地化.
- [IBAN谬误](https://github.com/globalcitizen/php-iban/blob/master/docs/FALSEHOODS.md) - 国际银行账户号码并不是全球统一的.
- [经济学谬误](http://exple.tive.org/blarg/2016/09/22/falsehoods-programmers-believe-about-economics/) - 经济学不简单，也不理性.
- [Etsy会计系统的小数点错误](https://www.reddit.com/r/Etsy/comments/hz4877/if_you_are_an_etsy_seller_do_not_purchase_postage/) - 会计软件中类型的重要性：漏掉小数点会导致多收费100倍.
- [两万五千刀的水分资金](http://rachelbythebay.com/w/2022/12/02/25k/) - 这种把美元和美分切割的错误同样出现在谷歌广告中，把 250美元的内部优惠券变成了 25000美元. 我的建议是: [货币值抛弃小数和浮点数. 用 decimals. 或者用回字符串解析, 而不校验.](https://twitter.com/kdeldycke/status/1599113889093890049)
- [公司名称中的`<` 和 `>`会导致XSS攻击](https://forum.aws.chdev.org/t/cross-site-scripting-xss-software-attack/3355) - 因为 [英国允许用特殊字符注册公司](https://www.legislation.gov.uk/uksi/2015/17/schedule/1/made), 一个骇客利用这种方式注册 `\"><SCRIPT SRC=MJT.XSS.HT></SCRIPT> LTD`, but also `; DROP TABLE "COMPANIES";-- LTD`, `BETTS &AMP; TWINE LTD` and `SAFDASD & SFSAF \' SFDAASF\" LTD`.
- [公司名称的细节](https://twitter.com/nthnmsmth/status/1587880523124408322) - 怎么让特拉华州和国税局的规则不冲突.
- [CLDR货币定义](https://github.com/unicode-org/cldr/blob/release-40/common/supplemental/supplementalData.xml#L87-L94) - 由于 叛乱、侵略、新法和缓慢的推进的计划，货币的有效日期范围出现重叠.
- [`税`](https://github.com/commerceguys/tax) - 一个PHP 5.4 的税务管理库.

## 加密货币

- [比特币谬误](https://github.com/theborakompanioni/spring-boot-bitcoin-starter/blob/master/docs/FALSEHOODS.md) - 关于比特币的错误观点列表.
- [以太坊谬误](https://gist.github.com/spalladino/a349f0ca53dbb5fc3914243aaf7ea8c6) - 合约编程的误解和常见陷阱.

## 日期和时间

- [时间谬误](http://infiniteundo.com/post/25326999628/falsehoods-programmers-believe-about-time) - 关于时间和日期的开创性文章.
- [更多的时间谬误](http://infiniteundo.com/post/25509354022/more-falsehoods-programmers-believe-about-time) - 上文的第二部分.
- [时间和时区谬误](https://www.creativedeletion.com/2015/01/28/falsehoods-programmers-date-time-zones.html) - 另一个关于时间的谬误，重点在于时区.
- [对时间谬误的批判](https://gist.github.com/thanatos/eee17100476a336a711e) - 源自上文的第一篇文章,对每一个谬误进行了解释, 有更多的背景和外部资源.
- [Unix时间谬误](https://alexwlchan.net/2019/05/falsehoods-programmers-believe-about-unix-time/) - 注意润秒!
- [时区谬误](https://www.zainrizvi.io/blog/falsehoods-programmers-believe-about-time-zones/) - 关于 DST 转换的边缘情况有一些不错的观点.
- [日历谬误](http://yourcalendricalfallacyis.com) - 一个涵盖插值和文化影响的清单，由 iOS 和 macOS 开发者社区制作.
- [时区数据库](https://www.iana.org/time-zones) - 全球许多代表性地点当地时间历史的代码和数据.
- [漫长而痛苦的时间史](http://naggum.no/lugm-time.html) - 时间记录中的大多数特殊性都可以在历史中找到解释.
- [你提倡日历改革](https://qntm.org/calendar) - 这篇文章告诉你为什么你的想法行不通.
- [所以你想废除时区](https://qntm.org/abolish) - 废除时区听起来似乎是个好主意，但有很多复杂因素让它似乎没那么好.
- [时间和时区的问题](https://www.youtube.com/watch?v=-5wpm-gesOY) - 一个视频，介绍了为什么"非必要不处理时区".
- [劳动部门超额征收 26000刀](http://digital.vpr.net/post/rounding-error-computer-code-leads-26000-overcollection-labor-department) - 错误的日历计算带来的后果.
- [RFC-3339 vs ISO-8601](https://ijmacd.github.io/rfc3339-iso8601/) - 一份包含两个标准的格式列表，展示了它们的重叠部分及实际示例.
- [ISO-8601, `YYYY`, `yyyy`, 为什么你的年份是错的](https://ericasadun.com/2018/12/25/iso-8601-yyyy-yyyy-and-why-your-year-may-be-wrong/) - 日期的字符串格式化很难.
- [UTC对于每个人来说都够了，对吗?](https://zachholman.com/talk/utc-is-enough-for-everyone-right) - 你可能没有想到关于日期和时间（特别是 UTC）的一些边缘情况.
- [存储 UTC 不是灵丹妙药](https://codeblog.jonskeet.uk/2019/03/27/storing-utc-is-not-a-silver-bullet/) - "只存 UTC" 并不总是对的.
- [如何在 UT1、TAI 和 UTC 之间进行选择](https://news.ycombinator.com/item?id=28047376) - 这取决于你对 SI 秒、地球自转同步和避免闰秒的优先级.
- [为什么 1927年的这两个时间想减得到了奇怪的结果?](https://stackoverflow.com/a/6841479/57311) - 臭名昭著的 Stack Overflow 答案，涉及复杂的历史时区，以及如何通过新版本的软件重新解释历史日期.
- [至关重要的日期](https://web.archive.org/web/20150908004245/http://www.merlyn.demon.co.uk/critdate.htm) - 从 Y2K 到 Unix 纪元的 32 位秒溢出，列出了一些特殊日期，需根据系统进行关注.
- “我要去佛蒙特的一个公社，期间不打算处理比一个季节更短的时间单位” - 这是一个在 70 年代辞职的工程师留下的留言，他在处理亚秒级计时问题上付出了过多的努力. 出处: [The Soul of a New Machine](https://www.amazon.com/dp/0316491705?&linkCode=ll1&tag=kevideld-20&linkId=ec2881e22fb26c2d43de0daeebd5424d&language=en_US&ref_=as_li_ss_tl).

## 教育

- [计算机科学的学生毕业后(仍然)相信的谎言](https://www.netmeister.org/blog/cs-falsehoods.html) - 一个关于事情的清单（不仅限于）计算机科学学生常常错误地、甚至令人惊讶地相信的观点，尽管他们（可能）应该更了解真相.
- [博士后流言](https://www.cs.kent.ac.uk/people/staff/srk21/blog/2019/12/02/) - “关于博士后研究人员，有很多言论、文章和信念都是完全不真实的.”

## 邮件

- [邮件谬误](https://beesbuzz.biz/code/439-Falsehoods-programmers-believe-about-email) - 关于地址、内容和交付.
- [我以为我知道如何验证邮件地址,直到我读了 RFC](https://haacked.com/archive/2007/08/21/i-knew-how-to-validate-an-email-address-until-i.aspx/) - 提供一些复杂的例子，这些例子是根据 RFC-822 标准认为有效的电子邮件地址.
- [所以你认为你可以验证邮件地址 (FOSDEM 2018)](https://fosdem.org/2018/schedule/event/email_address_quiz/) - 边缘案例电子邮件地址的展示以及为何不应使用正则表达式来解析它们.
- [你的邮件验证的逻辑是错的](https://www.netmeister.org/blog/email.html) - 电子邮件地址中允许的各种令人惊讶的内容总结.
- [`libvldmail`](https://github.com/dertuxmalwieder/libvldmail) - 一个实现基于 RFC 的邮件地址检查的库.

## 地理

- [地理谬误](https://wiesmann.codiferes.net/wordpress/archives/15187) - 讨论地点、它们的名称和位置.
- [地图谬误](http://www.atlefren.net/post/2014/09/falsehoods-programmers-believe-about-maps/) - 涵盖坐标、投影和 GIS.
- [我讨厌坐标系](https://ihatecoordinatesystems.com) - 地理空间从业者关于诊断和修复坐标系统常见问题的指南.
- [日本五个最离谱的汉字地名](https://web.archive.org/web/20210310050932/https://soranews24.com/2016/12/01/w-t-f-japan-top-5-most-insane-kanji-place-names-in-japan%E3%80%90weird-top-five%E3%80%91/) - "有一类特殊的汉字，对于日本人来说也很难读：地名."

## 人类身份
- [名字谬误](https://www.kalzumeus.com/2010/06/17/falsehoods-programmers-believe-about-names/) - 一切的开始.
- [名字谬误 – 举例](https://shinesolutions.com/2018/01/08/falsehoods-programmers-believe-about-names-with-examples/) - 上面文章的重温版本，这次有详细的解释.
- [生物识别谬误](https://shkspr.mobi/blog/2021/01/falsehoods-programmers-believe-about-biometrics/) - 指纹不是唯一的.
- [家庭谬误](https://shkspr.mobi/blog/2017/03/falsehoods-programmers-believe-about-families/) - 你不能用严格的规则来定义一个家庭.
- 性别谬误: [#1](https://gist.github.com/garbados/f82604ea639e0e47bf44) & [#2](https://medium.com/gender-2-0/falsehoods-programmers-believe-about-gender-f9a3512b4c9c) - 性别是人类身份的一部分，具有其自身的复杂性.
- [关于我的谬误](https://skylarmacdonald.com/falsehoods/) - 姓名、性别与国际化交叉的问题.
- [同性婚姻: 数据库工程视角](https://web.archive.org/web/20170914014648/https://qntm.org/gay) - 如何在数据库中存储婚姻信息，同时解决关于性别、姓名和关系的多数谬误.
- [世界各地人的名字](https://www.w3.org/International/questions/qa-personal-names) - 人们的姓名在世界各地有何不同，这对网络有什么影响?
- [XKCD #327: 妈妈的壮举](https://xkcd.com/327/) - 关于如何实现一种可能导致安全漏洞的谬误的幽默解读.
- [你好, 我是 Null 先生. 我的名字让计算机看不到我](https://www.wired.com/2015/11/null/) - 关于错误实现如何对某人生活产生负面影响的真实案例.
- [HL7 v3 RIM](https://www.hl7.org/implement/standards/product_brief.cfm?product_id=186) - 用于表示人类姓名的灵活数据模型.
- [Apple iOS `NSPersonNameComponentsFormatter`](https://developer.apple.com/library/ios/documentation/Miscellaneous/Reference/NSPersonNameComponentsFormatter_Class/index.html) - 一个人姓名各个组成部分的本地化表示.

## 国际化

关于字符编码，字符串格式，Unicode 和国际化.

- [语言谬误](http://garbled.benhamill.com/2017/04/18/falsehoods-programmers-believe-about-language) - 把软件从英文翻译成其他语言并不像看起来那么简单.
- [纯文本谬误](https://jeremyhussell.blogspot.com/2017/11/falsehoods-programmers-believe-about.html#main) - 纯文本难以满足需求，而 Unicode 的强大在于其能够良好运作，显得尤为出色.
- [文本谬误](https://wiesmann.codiferes.net/wordpress/archives/30296) -以上谬误中的一部分，并附带一些示例说明.
- [代码国际化](https://www.youtube.com/watch?v=0j74jcxSunY) - 关于在代码国际化时需要注意的事项的视频.
- [关于Unicode 和字符集你至少应该知道的](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/) - 对unicode很棒的介绍, 包括其历史背景和起源，随后概述其内部工作原理.
- [Awesome Unicode](https://github.com/Wisdom/Awesome-Unicode) - 精心总结的 Unicode 小知识、软件包和资源清单.
- [Unicode的黑暗角落](https://eev.ee/blog/2015/09/12/dark-corners-of-unicode/) - Unicode 非常庞大，小心其中的陷阱.
- [别给码位加戏了](https://manishearth.github.io/blog/2017/01/14/stop-ascribing-meaning-to-unicode-code-points/) - 深入探讨 Unicode，并揭穿关于码位的流言.
- [Unicode谬误](https://jean.abou-samra.fr/blog/unicode-misconceptions/) - 一系列关于大小写、编码、字符串长度等的谬误.
- [打破我们对 `Latin-1` 的假设](https://manishearth.github.io/blog/2017/01/15/breaking-our-latin-1-assumptions/) - 大多数程序员在'Latin-1'上花了太多时间，以至于忘记了其他脚本的特点.
- [致货运标签](http://i.imgur.com/4J7Il0m.jpg) - 字符编码很复杂，尤其是当每一层损坏的数据输入都增添了自己的复杂性时.
- [本地化失败：困难的温度](https://randomascii.wordpress.com/2023/10/17/localization-failure-temperature-is-hard/) - 你无法直接对温差进行本地化处理.
- [国际化测试数据](https://github.com/patch/i18n-testing) - 用于单元测试和质量保证的真实词汇的国际和多样化姓名数据集汇编.
- [违规字符串大集合](https://github.com/minimaxir/big-list-of-naughty-strings) - 一个庞大的字符串语料库,当作为用户输入数据时，很有可能导致问题. 必须有一组有效的边缘案例来测试您的软件.

## 管理

- [求职者谬误](https://web.archive.org/web/20170114022820/https://medium.com/@creatrixtiara/falsehoods-programmers-believe-about-job-applicants-99280437c616) - 关于求职者及其工作经历的假设未必准确。.

## 多媒体

- [视频谬误](https://haasn.xyz/posts/2016-12-25-falsehoods-programmers-believe-about-%5Bvideo-stuff%5D.html) - 涵盖全部内容：视频解码与播放、文件、图像缩放、色彩空间与转换、显示设备和字幕.
- [处理音乐时需要考虑的棘手边缘案例](https://dustri.org/b/horrible-edge-cases-to-consider-when-dealing-with-music.html) - 音乐目录数据中充满了各种奇葩内容.
- [MusicBrainz数据库表](https://musicbrainz.org/doc/MusicBrainz_Database/Schema) - 一个开源的数据库项目，似乎解决了音乐目录管理的复杂性.
- [DDEX](https://ddex.net/standards/) - 音乐元数据的行业标准，包括档案管理、声音录制、销售和使用报告、版权和许可协议.
- [Apple Music 风格指南](https://help.apple.com/itc/musicstyleguide/en.lproj/static.html) - 提高可发现性的音乐、艺术和元数据格式的质量保证指南

## 网络

- [网络谬误](http://blog.erratasec.com/2012/06/falsehoods-programmers-believe-about.html) - 包括 TCP, DHCP, DNS, VLANs 和 IPv4/v6.
- [分布式计算谬误](https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing) - 新接触分布式应用的程序员不可避免的错误假设.
- [IP地址不止一种写法](https://ma.ttias.be/theres-more-than-one-way-to-write-an-ip-address/) - 地址的某些部分是可选的，要注意十进制和八进制表示，而且 [别忘了 IPv6](https://news.ycombinator.com/item?id=20390981) .
- [IDN 很疯狂](https://daniel.haxx.se/blog/2022/12/14/idn-is-crazy/) - 域名中的国际字符意味着支持同形异义词和异形异义词.
- [`主机名-校验`](https://github.com/jakeogh/hostname-validate) - 一个尝试校验主机名的 python库.

## 电话号码

- [电话号谬误](https://github.com/googlei18n/libphonenumber/blob/master/FALSEHOODS.md) - 包括电话号码，他们的表示和意义.
- [`libphonenumber`](https://github.com/googlei18n/libphonenumber) - Google的一个通用库，用于解析，校验，格式化国际电话号码.包括Java, C++ 和 JavaScript.也能用于  [C#](https://github.com/twcclegg/libphonenumber-csharp), [Objective-C](https://github.com/iziz/libPhoneNumber-iOS), [Python](https://github.com/daviddrysdale/python-phonenumbers), [Ruby](https://github.com/sstephenson/global_phone) 和 [PHP](https://github.com/giggsey/libphonenumber-for-php).

## 邮政编码

- [邮政编码谬误](https://www.mjt.me.uk/posts/falsehoods-programmers-believe-about-addresses/) -包括街道、邮政编码、建筑物、城市和国家.
- [居住谬误](https://twitter.com/samphippen/status/813896916534784004) - 这不仅仅是地址本身的问题，而是一个人和它的住所之间的关系.
- [尽管没有姓名和地址，信件仍被送达](https://twitter.com/loriskumo/status/735851511331356672) - 关于邮政地址的终极谬误：你并不需要这些信息.
- [英国地址的奇特之处](https://paulplowman.com/stuff/uk-address-oddities/) - 从1995年以来英格兰和威尔士的大多数住宅物业销售列表中提取的奇特之处.
- [什么是最简化的英国地址?](https://microblog.vladh.net/posts/most-minimal-uk-address/) - 诀窍在于依赖邮政编码，在英国，邮政编码非常具体，‘通常标识一栋或几栋特定的建筑，而不像某些国家那样，一个邮政编码代表整个社区’.
- [拥有自己邮政编码的熊](https://kottke.org/19/08/the-bear-with-its-own-zip-code) - 斯莫基熊拥有自己的邮政编码（'20252'），因为他收到的邮件太多.
- [为什么哥斯达黎加不使用真实地址？](https://www.crcdaily.com/p/why-doesnt-costa-rica-use-real-addresses) - 哥斯达黎加使用一种特有的地址系统，该系统依赖于地标、历史和相当多的猜测。.
- [正则表达式和邮政地址](https://smartystreets.com/articles/regular-expressions-for-street-addresses) - 为什么正则表达式和街道地址不相容.
- [解析臭名昭著的日本邮政 CSV](https://www.dampfkraft.com/posuto.html) - "我见过许多可怕的事情，但从未在其他地方见过这种特殊的格式选择".
- [USPS 邮政地址标准](https://pe.usps.com/text/pub28/welcome.htm) - 描述了标准化的地址格式和内容.
- [`libaddressinput`](https://github.com/googlei18n/libaddressinput) - 谷歌用于解析、格式化和验证国际邮政地址的常用 C++ 和 Java 库.
- [`addressing`](https://github.com/commerceguys/addressing) - 一个基于谷歌数据集的 PHP 5.4+ 地址库.
- [`postal-address`](https://github.com/scaleway/postal-address) - 用于解析、标准化和渲染邮政地址的 Python 模块.
- [`address`](https://github.com/Boostport/address) - 基于谷歌的数据集的用于验证和格式化地址的 Go 库.

## 科学

- [关于测量系统的谬误](https://www.stevemoser.org/posts/dev/falsehoods-programmers-believe-about-systems-of-measurement.html) - 关于使用测量系统和它们之间转换的内容.

## 社会

- [政治任命谬误](https://twitter.com/oliver_dw/status/737930439575404544) - 设计选举系统有其自身的技巧.
- [科技领域的女性谬误](https://gist.github.com/Su-Shee/5d1a417fa9de19c15477) - 关于女性在 STEM（科学、技术、工程、数学）行业的流言.

## 软件工程

- [版本谬误](https://github.com/xenoterracide/falsehoods/blob/master/versions.md) - 为软件发布分配一个身份可能比想象中要困难.
- [构建系统谬误](https://pozorvlak.livejournal.com/174763.html) -  构建软件很难. 构建构建软件本身更难.
- [Undefined行为谬误](https://predr.ag/blog/falsehoods-programmers-believe-about-undefined-behavior/) - 调用`undefined`行为可能导致任何事情发生，其范围比人们想象的要广得多.
- [CSV谬误](https://donatstudios.com/Falsehoods-Programmers-Believe-About-CSVs) - 尽管 RFC4180 存在，但它远非权威，且在很大程度上被忽视.
- [包管理谬误](https://kdeldycke.github.io/meta-package-manager/falsehoods.html) - 涵盖包及其管理工具.
- [测试谬误](https://club.ministryoftesting.com/t/falsehoods-testers-believe/1371) - 试图建立关于测试的谬误列表.
- [搜索谬误](https://opensourceconnections.com/blog/2019/05/29/falsehoods-programmers-believe-about-search/) - 为什么搜索（包括分析、分词、高亮）看上去那么复杂.
- [每个软件工程师应该了解的搜索知识](https://scribe.rip/p/what-every-software-engineer-should-know-about-search-27d1df99f80d) - 一篇关于`实现一个搜索引擎有多难`的很棒的文章.
- [分页谬误](https://www.hezmatt.org/~mpalmer/blog/2018/12/12/falsehoods-programmers-believe-about-pagination.html) - 为什么你的分页算法让某些人（可能是你自己）感到头痛.
- [垃圾回收算法谬误](https://paul.bone.id.au/blog/2018/10/19/gc-falsehoods/) - 关于垃圾收集的可预测性和性能的误解.
- [文件路径谬误](https://yakking.branchable.com/posts/falsehoods-programmers-believe-about-file-paths/) - 文件系统和操作系统的多样性使得文件路径比我们想象的要复杂一些.
- [Windows文件路径的奇异世界](https://www.fileside.app/blog/2023-03-17_windows-file-paths/) - “在任何 Unix 衍生系统中，路径是一个令人钦佩的简单概念：如果它以 / 开头，那么它就是一个路径。但在 Windows 上情况并非如此。”
- [CPU 缓存流言](https://software.rajivprab.com/2018/04/29/myths-programmers-believe-about-cpu-caches/) - 关于缓存的误解常常导致错误的断言，特别是在并发和竞争条件方面.
- [`/dev/urandom` 流言](https://www.2uo.de/myths-about-urandom) - 关于 '/dev/urandom' 和 '/dev/random' 有一些反复出现的说法，但它们仍然是错误的.
- [状态机事实](https://codeberg.org/catseye/The-Dossier/src/branch/master/article/Facts-about-State-Machines/README.md) - 状态机常常被误解并且应用不足.
- [嗨! 我的名字是…](https://www.youtube.com/watch?v=NIebelIpdYk) - 这次演讲本可以命名为*关于用户名（和其他标识符）的谬误*.
- [`mtime`的主流误解](https://apenwarr.ca/log/20181113) - 为什么文件的 `mtime` 有害的部分文章.
- [自动补全规则](http://jeremymikkola.com/posts/2019_03_19_rules_for_autocomplete.html) - 并不严格是谬误，但仍然是实现自动补全功能的良好实践的优秀清单.
- [浮点流言](https://0.30000000000000004.com) - “你的语言没坏, 它只是在进行浮点计算. (…) 这就是为什么经常发生 `0.1 + 0.2 != 0.3`.
- [来自地狱的YAML文档](https://ruudvanasseldonk.com/2023/01/11/the-yaml-document-from-hell) - YAML 充满了模糊的复杂性，例如意外的数字和非字符串键.
- [我对标签系统充满了无尽的兴趣](https://twitter.com/hillelogram/status/1534301374166474752) - 即使在应该是简单的标签系统中，也存在一些边缘情况.
- [量子技术谬误](https://github.com/gottfriedsz/falsehoods-quantum) - 关于量子技术和计算机的常见误解
- [事件驱动系统谬误](https://dimtion.fr/blog/falsehoods-event-driven/) - 关于事件驱动系统和消息传递的误解.

## 交通

- [汽车谬误](https://github.com/driveto/falsehoods-about-cars) - 即使是像定义一辆汽车这样普遍的事情也充满了陷阱.
- [航空座位图谬误](https://duffel.com/blog/falsehoods-about-seat-maps) - 航空公司座位图远比整齐的座位排和列复杂得多.
- [大量混乱到令人抓狂的航空码](https://www.youtube.com/watch?v=jfOUVYQnuhw) - 多个国际和国家机构试图调和历史、实用性和物流，导致航空码遵循古怪的规则.
- [我的名字在任何预约中都会出问题!](https://travel.stackexchange.com/questions/149323/my-name-causes-an-issue-with-any-booking-names-end-with-mr-and-mrs) - 旧的航空公司预订系统将 'MR' 后缀视为 'Mister'，并将其省略.

## 排版

- [字体谬误](https://github.com/RoelN/Font-Falsehoods) - 关于网页和桌面排版的假设.
- [程序员应该知道的大小写的真相](https://www.b-list.org/weblog/2018/nov/26/case/) - 一个关于大小写（如大写和小写文本）主题的内容，以完全相反的方式呈现谬误列表格式。.

## 视频游戏

- [门问题](https://lizengland.com/blog/2014/04/the-door-problem/) - 在游戏中，所有你没有考虑的关于门的东西.

## Web

- [HTML谬误](https://www.aartaka.me.eu.org/falsehoods-html) - “web是好看的，web是丑陋的，web是令人惊叹的。而其中一部分魅力来自 HTML 及其独特的历史遗留问题”
- [REST API谬误](https://web.archive.org/web/20201112010147/http://slinkp.com/falsehoods-programmers-believe-about-apis.html) - 在创建和写API文档的时候要注意的陷阱.
- [URL: 它很复杂…](https://www.netmeister.org/blog/urls.html) - 一个 URL 中包含许多组成部分，每个部分都有其自身的逻辑.
- [下载网站图标的隐藏复杂性：通过 15 个以上的边缘案例讲述](https://web.archive.org/web/20230604033340/https://www.simplecto.com/complexity-downloading-favicons-told-in-15-plus-edge-cases/) - 下载您在浏览器标签中看到的小图标应该是一个简单的任务。结果证明，这比您想象的要复杂得多。请注意，别陷入无休止的琐事中.

## 贡献

随时欢迎你的贡献! 首先请看一下 [贡献指南](https://github.com/kdeldycke/awesome-falsehood/blob/main/.github/contributing.zh.md) .

## 注脚

这份列表在过去几年里在社交媒体上获得了一些人气. 可以看看这个 [其他讨论](https://github.com/kdeldycke/kdeldycke/blob/main/in-the-media.md).

这个[标题图片](https://github.com/kdeldycke/awesome-falsehood/blob/main/assets/awesome-falsehood-header.jpg) 以 [photo taken in February 2010 by Iza Bella](https://commons.wikimedia.org/wiki/File:BLW_Truth_and_Falsehood.jpg)为基础修改的 , 根据 [Creative Commons BY-SA 2.0 UK 许可协议](https://creativecommons.org/licenses/by-sa/2.0/uk/deed.en) 分发.

<!--lint disable no-undefined-references-->

<a name="intro-quote-def">\[1\]</a>: [*Notebooks, 1914-1916*](https://www.amazon.com/dp/1324090804?&linkCode=ll1&tag=kevideld-20&linkId=a1903c3fbfdc82fbe2e566fca40718fb&language=en_US&ref_=as_li_ss_tl) (Liveright, 2022) - [出处: 14页](https://archive.org/details/notebooks191419100witt/page/n35). [\[↑\]](#intro-quote-ref)
