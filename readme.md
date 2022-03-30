# 😱 Awesome Falsehood [![Awesome](https://awesome.re/badge-flat.svg)](https://github.com/sindresorhus/awesome)

**A curated list of falsehoods programmers believe in.**

<p align="center">
  <a href="https://github.com/kdeldycke/awesome-falsehood/">
    <img src="https://github.com/kdeldycke/awesome-falsehood/raw/main/assets/awesome-falsehood-header.jpg" alt="Awesome Falsehood header image">
  </a>
</p>

<p align="center">
  <i>The logic of the world is prior to all truth and falsehood.</i><br>
  — Ludwig Wittgenstein<sup id="intro-quote-ref"><a href="#intro-quote-def">[1]</a></sup>
</p>

A *falsehood* is an ***idea* that you initially believe was true**, but in-reality it is **proven to be false**.

E.g. of an *idea*: valid email address exactly has one `@` character. So, you will use this rule to implement your email-field validation logic. Right? Wrong! The *reality* is: emails can have multiple `@` chars. Therefore your implementation should allow this. The initial *idea* is a falsehood you believed in.

The *falsehood* articles listed below will have a comprehensive list of those false-beliefs that you should be aware of, to help you become a better programmer.

## Contents<a name="contents"></a>

<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=2 -->

- [Contents](#contents)
- [Meta](#meta)
- [Arts](#arts)
- [Business](#business)
- [Dates and Time](#dates-and-time)
- [Education](#education)
- [Emails](#emails)
- [Geography](#geography)
- [Human Identity](#human-identity)
- [Internationalization](#internationalization)
- [Management](#management)
- [Multimedia](#multimedia)
- [Networks](#networks)
- [Phone Numbers](#phone-numbers)
- [Postal Addresses](#postal-addresses)
- [Science](#science)
- [Society](#society)
- [Software Engineering](#software-engineering)
- [Typography](#typography)
- [Video Games](#video-games)

<!-- mdformat-toc end -->

## Meta<a name="meta"></a>

- [Falsehoods Programmers Believe](https://spaceninja.com/2015/12/07/falsehoods-programmers-believe/) - A brief list of common falsehoods. A great overview and quick introduction into the world of falsehoods.
- [Falsehoods about Programming](https://chiselapp.com/user/ttmrichter/repository/gng/doc/trunk/output/falsehoods.html) - A humbling and fun list on programming and programmers themselves.
- [Falsehoods about Falsehoods Lists](https://kevin.deldycke.com/2016/12/falsehoods-programmers-believe-about-falsehoods-lists/) - Meta commentary on how these falsehoods shouldn't be handled.

## Arts<a name="arts"></a>

- [Falsehoods about Music](https://literateprogrammer.blogspot.fr/2016/07/falsehoods-programmers-believe-about.html) - False assumption that might be made in codifying music.
- [Falsehoods about Art](http://artsy.github.io/blog/2018/04/18/programmer-misconceptions-about-art/) - Common misconceptions about art.

## Business<a name="business"></a>

- [Falsehoods about Online Shopping](http://wiesmann.codiferes.net/wordpress/?p=22201) - Covers prices, currencies and inventory.
- [Falsehoods about Prices](https://gist.github.com/rgs/6509585) - Covers currencies, amounts and localization.
- [Falsehoods about IBANs](https://github.com/globalcitizen/php-iban/blob/master/docs/FALSEHOODS.md) - International Bank Account Numbers are not international.
- [Falsehoods about Economics](http://exple.tive.org/blarg/2016/09/22/falsehoods-programmers-believe-about-economics/) - Economics are not simple or rational.
- [Falsehoods about Cars](https://github.com/driveto/falsehoods-about-cars) - Even something as common as defining a car is full of pitfalls.
- [Falsehoods about Airline Seat Maps](https://duffel.com/blog/falsehoods-about-seat-maps) - Airline seat maps are far more complex than just neat rows and columns of seats.
- [Decimal Point Error in Etsy's Accounting System](https://www.reddit.com/r/Etsy/comments/hz4877/if_you_are_an_etsy_seller_do_not_purchase_postage/) - The importance of types in accounting software: missing the decimal point ends up with 100x over-charges.
- [Characters `<` and `>` in company names lead to XSS attacks](https://forum.aws.chdev.org/t/cross-site-scripting-xss-software-attack/3355) - Because [UK allows companies to be registered with special characters](https://www.legislation.gov.uk/uksi/2015/17/schedule/1/made), a hacker leveraged them to register `\"><SCRIPT SRC=MJT.XSS.HT></SCRIPT> LTD`, but also `; DROP TABLE "COMPANIES";-- LTD`, `BETTS &AMP; TWINE LTD` and `SAFDASD & SFSAF \' SFDAASF\" LTD`.
- [CLDR currency definitions](https://github.com/unicode-org/cldr/blob/release-40/common/supplemental/supplementalData.xml#L87-L94) - Currency validity date ranges overlap due to revolts, invasions, new constitutions, and slow planned adoption.
- [`tax`](https://github.com/commerceguys/tax) - A PHP 5.4+ tax management library.

## Dates and Time<a name="dates-and-time"></a>

- [Falsehoods about Time](http://infiniteundo.com/post/25326999628/falsehoods-programmers-believe-about-time) - Seminal article on dates and time.
- [More Falsehoods about Time](http://infiniteundo.com/post/25509354022/more-falsehoods-programmers-believe-about-time) - Part. 2 of the article above.
- [Falsehoods about Time and Time Zones](https://www.creativedeletion.com/2015/01/28/falsehoods-programmers-date-time-zones.html) - Another takes on time-related falsehoods, with an emphasis on time zones.
- [Critique of Falsehoods about Time](https://gist.github.com/thanatos/eee17100476a336a711e) - Takes on the first article above and provides an explanation of each falsehood, with more context and external resources.
- [Falsehoods about Unix Time](https://alexwlchan.net/2019/05/falsehoods-programmers-believe-about-unix-time/) - Mind the leap second!
- [Falsehoods about Time Zones](https://www.zainrizvi.io/blog/falsehoods-programmers-believe-about-time-zones/) - Has some nice points regarding the edge-cases of DST transitions.
- [Your Calendrical Fallacy Is Thinking…](http://yourcalendricalfallacyis.com) - List covering intercalation and cultural influence, made by a community of iOS and macOS developers.
- [Time Zone Database](https://www.iana.org/time-zones) - Code and data that represent the history of local time for many representative locations around the globe.
- [The Long, Painful History of Time](http://naggum.no/lugm-time.html) - Most of the idiosyncrasies in time keeping can find an explanation in history.
- [You Advocate a Calendar Reform](https://qntm.org/calendar) - Your idea will not work. This article tells you why.
- [So You Want to Abolish Time Zones](https://qntm.org/abolish) - Abolishing timezones may sound like a good idea, but there are quite a few complications that make it not quite so.
- [The Problem with Time & Timezones](https://www.youtube.com/watch?v=-5wpm-gesOY) - A video about why you should never, ever deal with timezones if you can help it.
- [\$26,000 Overcollection by Labor Department](http://digital.vpr.net/post/rounding-error-computer-code-leads-26000-overcollection-labor-department) - The consequence of wrong calendar accounting.
- [RFC-3339 vs ISO-8601](https://ijmacd.github.io/rfc3339-iso8601/) - An giant list of formats from the two standards, how they overlaps, and live examples.
- [ISO-8601, `YYYY`, `yyyy`, and why your year may be wrong](https://ericasadun.com/2018/12/25/iso-8601-yyyy-yyyy-and-why-your-year-may-be-wrong/) - String formatting of date is hard.
- [UTC is Enough for everyone, right?](https://zachholman.com/talk/utc-is-enough-for-everyone-right) - There are edge cases about dates and time (specifically UTC) that you probably haven't thought of.
- [Storing UTC is not a silver bullet](https://codeblog.jonskeet.uk/2019/03/27/storing-utc-is-not-a-silver-bullet/) - "Just store dates in UTC" is not always the right approach.
- [How to chooose between UT1, TAI and UTC](https://news.ycombinator.com/item?id=28047376) - Depends on your priorities between SI seconds, earth rotation sync, leap seconds avoidance.
- [Why is subtracting these two times (in 1927) giving a strange result?](https://stackoverflow.com/a/6841479/57311) - Infamous Stack Overflow answer about both complicated historical timezones, and how historical dates can be re-interpreted by newer versions of software.
- [Critical and Significant Dates](https://web.archive.org/web/20150908004245/http://www.merlyn.demon.co.uk/critdate.htm) - From Y2K to the overflow of 32-bit seconds from unix epoch, a list of special date to watch for depending on the system.

## Education<a name="education"></a>

- [Falsehoods CS Students (Still) Believe Upon Graduating](https://www.netmeister.org/blog/cs-falsehoods.html) - A list of things (not only) computer science students tend to erroneously and at times surprisingly believe even though they (probably) should know better.
- [Postdoc myths](https://www.cs.kent.ac.uk/people/staff/srk21/blog/2019/12/02/) - `Lots of things are said, written and believed about postdoctoral researchers that are simply not true.`.

## Emails<a name="emails"></a>

- [I Knew How to Validate an Email Address Until I Read the RFC](https://haacked.com/archive/2007/08/21/i-knew-how-to-validate-an-email-address-until-i.aspx/) - Provides intricate examples that are unsuspected valid email addresses according the RFC-822.
- [So you think you can validate email addresses (FOSDEM 2018)](https://fosdem.org/2018/schedule/event/email_address_quiz/) - Presentation of edge-case email addresses and why you should not use regex to parse them.
- [Your E-Mail Validation Logic is Wrong](https://www.netmeister.org/blog/email.html) - A summary of the various, surprising things that are allowed in an email address.

## Geography<a name="geography"></a>

- [Falsehoods about Geography](http://wiesmann.codiferes.net/wordpress/?p=15187) - Takes on places, their names and locations.
- [Falsehoods about Maps](http://www.atlefren.net/post/2014/09/falsehoods-programmers-believe-about-maps/) - Covers coordinates, projection and GIS.
- [I Hate Coordinate Systems](https://ihatecoordinatesystems.com) - A guide for geospatial practitioners on diagnosing and fixing common issues with coordinate systems.
- [Top 5 most insane kanji place names in Japan](https://soranews24.com/2016/12/01/w-t-f-japan-top-5-most-insane-kanji-place-names-in-japan%e3%80%90weird-top-five%e3%80%91/) - “There's one special group of kanji that's hard even for Japanese people to read: place names.”

## Human Identity<a name="human-identity"></a>

- [Falsehoods about Names](https://www.kalzumeus.com/2010/06/17/falsehoods-programmers-believe-about-names/) - The article that started it all.
- [Falsehoods about Names – With Examples](https://shinesolutions.com/2018/01/08/falsehoods-programmers-believe-about-names-with-examples/) - A revisited version of the article above, this time with detailed explanations.
- [Falsehoods about Biometrics](https://shkspr.mobi/blog/2021/01/falsehoods-programmers-believe-about-biometrics/) - Fingerprints are not unique.
- [Falsehoods about Families](https://shkspr.mobi/blog/2017/03/falsehoods-programmers-believe-about-families/) - You can't really define a family with strict rules.
- Falsehoods about Gender: [#1](https://gist.github.com/garbados/f82604ea639e0e47bf44) & [#2](https://medium.com/gender-2-0/falsehoods-programmers-believe-about-gender-f9a3512b4c9c) - Gender is part of human identity and has its own subtleties.
- [Falsehoods about Me](https://skylarmacdonald.com/falsehoods/) - Issues at the intersection of names and gender and internationalization.
- [Gay Marriage: The Database Engineering Perspective](https://web.archive.org/web/20170914014648/https://qntm.org/gay) - How to store a marriage in a database while addressing most of the falsehoods about gender, naming and relationships.
- [Personal Names Around the World](https://www.w3.org/International/questions/qa-personal-names) - How do people's names differ around the world, and what are the implications for the Web?
- [XKCD #327: Exploits of a Mom](https://xkcd.com/327/) - Funny take on how implementation of a falsehood might lead to security holes.
- [Hello, I'm Mr. Null. My Name Makes Me Invisible to Computers](https://www.wired.com/2015/11/null/) - Real-life example on how implemented falsehood has negative impact on someone's life.
- [My name causes an issue with any booking!](https://travel.stackexchange.com/questions/149323/my-name-causes-an-issue-with-any-booking-names-end-with-mr-and-mrs) - Old airline reservation systems considers the `MR` suffix as `Mister` and drops it.
- [HL7 v3 RIM](https://www.hl7.org/implement/standards/product_brief.cfm?product_id=186) - A flexible data model for representing human names.
- [Apple iOS `NSPersonNameComponentsFormatter`](https://developer.apple.com/library/ios/documentation/Miscellaneous/Reference/NSPersonNameComponentsFormatter_Class/index.html) - Localized representations of the components of a person's name.

## Internationalization<a name="internationalization"></a>

On character encoding, string formatting, unicode and internationalization.

- [Falsehoods about Language](http://garbled.benhamill.com/2017/04/18/falsehoods-programmers-believe-about-language) - Translating a software from English is not as straightforward as it seems to be.
- [Falsehoods about Plain Text](https://jeremyhussell.blogspot.com/2017/11/falsehoods-programmers-believe-about.html#main) - Plain text can't cut it and why it's surprising Unicode works as well as it does.
- [Internationalis(z)ing Code](https://www.youtube.com/watch?v=0j74jcxSunY) - A video about things you need to keep in mind when internationalizing your code.
- [Minimum to Know About Unicode and Character Sets](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/) - A good introduction to unicode, its historical context and origins, followed by an overview of its inner working.
- [Awesome Unicode](https://github.com/Wisdom/Awesome-Unicode) - A curated list of delightful Unicode tidbits, packages and resources.
- [Dark corners of Unicode](https://eev.ee/blog/2015/09/12/dark-corners-of-unicode/) - Unicode is extensive, here be dragons.
- [Let's Stop Ascribing Meaning to Code Points](https://manishearth.github.io/blog/2017/01/14/stop-ascribing-meaning-to-unicode-code-points/) - Dives deeper in Unicode and dispels myths about code points.
- [Breaking Our `Latin-1` Assumptions](https://manishearth.github.io/blog/2017/01/15/breaking-our-latin-1-assumptions/) - Most programmers spend so much time with `Latin-1` they forgets about other's scripts quirks.
- [Ode to a shipping label](http://i.imgur.com/4J7Il0m.jpg) - Character encoding is hard, more so when each broken layer of data input adds its own spice.
- [i18n Testing Data](https://github.com/patch/i18n-testing) - Compilation of real-word international and diverse name data for unit testing and QA.
- [Big List of Naughty Strings](https://github.com/minimaxir/big-list-of-naughty-strings) - A huge corpus of strings which have a high probability of causing issues when used as user-input data. A must have set of practical edge-cases to test your software against.

## Management<a name="management"></a>

- [Falsehoods about Job Applicants](https://web.archive.org/web/20170114022820/https://medium.com/@creatrixtiara/falsehoods-programmers-believe-about-job-applicants-99280437c616) - Assumptions about job applicants and their job histories aren't necessarily true.

## Multimedia<a name="multimedia"></a>

- [Falsehoods about Video](https://haasn.xyz/posts/2016-12-25-falsehoods-programmers-believe-about-%5Bvideo-stuff%5D.html) - Cover it all: video decoding and playback, files, image scaling, color spaces and conversion, displays and subtitles.

## Networks<a name="networks"></a>

- [Falsehoods about Networks](http://blog.erratasec.com/2012/06/falsehoods-programmers-believe-about.html) - Covers TCP, DHCP, DNS, VLANs and IPv4/v6.
- [Fallacies of Distributed Computing](https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing) - Assumptions that programmers new to distributed applications invariably make.
- [There's more than one way to write an IP address](https://ma.ttias.be/theres-more-than-one-way-to-write-an-ip-address/) - Some parts of the address are optional, mind the decimal and octal notations, and [don't forget IPv6](https://news.ycombinator.com/item?id=20390981) either.
- [URLs: It's complicated…](https://www.netmeister.org/blog/urls.html) - There's a lot of components in an URL, and all have their own logic.
- [`hostname-validate`](https://github.com/jakeogh/hostname-validate) - An attempt to validate hostnames in Python.

## Phone Numbers<a name="phone-numbers"></a>

- [Falsehoods about Phone Numbers](https://github.com/googlei18n/libphonenumber/blob/master/FALSEHOODS.md) - Covers phone numbers, their representation and meaning.
- [`libphonenumber`](https://github.com/googlei18n/libphonenumber) - Google's common Java, C++ and JavaScript library for parsing, formatting, and validating international phone numbers. Also available for [C#](https://github.com/twcclegg/libphonenumber-csharp), [Objective-C](https://github.com/iziz/libPhoneNumber-iOS), [Python](https://github.com/daviddrysdale/python-phonenumbers), [Ruby](https://github.com/sstephenson/global_phone) and [PHP](https://github.com/giggsey/libphonenumber-for-php).

## Postal Addresses<a name="postal-addresses"></a>

- [Falsehoods about Addresses](https://www.mjt.me.uk/posts/falsehoods-programmers-believe-about-addresses/) - Covers streets, postal codes, buildings, cities and countries.
- [Falsehoods about Residence](https://twitter.com/samphippen/status/813896916534784004) - It's not only about the address itself, but the relationship between a person and its residence.
- [Letter Delivered Despite No Name, No Address](https://twitter.com/loriskumo/status/735851511331356672) - Ultimate falsehood about postal addresses: you do not need one.
- [The Bear with Its Own ZIP Code](https://kottke.org/19/08/the-bear-with-its-own-zip-code) - Smokey Bear has his own ZIP Code (`20252`) because he gets so much mail.
- [Regex and Postal Addresses](https://smartystreets.com/articles/regular-expressions-for-street-addresses) - Why regular expressions and street addresses do not mix.
- [Parsing the Infamous Japanese Postal CSV](https://www.dampfkraft.com/posuto.html) - “I saw many horrors, but I've never seen this particular formatting choice anywhere else.”
- [`libaddressinput`](https://github.com/googlei18n/libaddressinput) - Google's common C++ and Java library for parsing, formatting, and validating international postal addresses.
- [`addressing`](https://github.com/commerceguys/addressing) - A PHP 5.4+ addressing library, powered by Google's dataset.
- [`postal-address`](https://github.com/scaleway/postal-address) - Python module to parse, normalize and render postal addresses.
- [`address`](https://github.com/Boostport/address) - Go library to validate and format addresses using Google's dataset.

## Science<a name="science"></a>

- [Falsehoods about Systems of Measurement](https://www.stevemoser.org/posts/dev/falsehoods-programmers-believe-about-systems-of-measurement.html) - On working with systems of measurement and converting between them.

## Society<a name="society"></a>

- [Falsehoods about Political Appointments](https://twitter.com/oliver_dw/status/737930439575404544) - Designing election systems has its own tricks.
- [Falsehoods about Women In Tech](https://gist.github.com/Su-Shee/5d1a417fa9de19c15477) - Myth about women in STEM (Science, Technology, Engineering, Math) industries.

## Software Engineering<a name="software-engineering"></a>

- [Falsehoods about Versions](https://github.com/xenoterracide/falsehoods/blob/master/versions.md) - Attributing an identity to a software release might be harder than thought.
- [Falsehoods about Build Systems](https://pozorvlak.livejournal.com/174763.html) - Building software is hard. Building software that builds software is harder.
- [Falsehoods about REST APIs](https://web.archive.org/web/20201112010147/http://slinkp.com/falsehoods-programmers-believe-about-apis.html) - Pitfalls to be mindful of when creating and documenting APIs.
- [Falsehoods about CSVs](https://donatstudios.com/Falsehoods-Programmers-Believe-About-CSVs) - While RFC4180 to exists, it is far from definitive and goes largely ignored.
- [Falsehoods about Package Managers](https://kdeldycke.github.io/meta-package-manager/falsehoods.html) - Covers package and their managers.
- [Falsehoods about Testing](https://club.ministryoftesting.com/t/falsehoods-testers-believe/1371) - An attempt to establish a list of falsehoods about testing.
- [Falsehoods about Search](https://opensourceconnections.com/blog/2019/05/29/falsehoods-programmers-believe-about-search/) - Why search (including analysis, tokenization, highlighting) is deceptively complex.
- [What every software engineer should know about search](https://scribe.rip/p/what-every-software-engineer-should-know-about-search-27d1df99f80d) - A better sourced article on the difficulty of implementing search engines.
- [Falsehoods about Bitcoin](https://github.com/theborakompanioni/spring-boot-bitcoin-starter/blob/master/docs/FALSEHOODS.md) - A list of mistaken perspectives on Bitcoin.
- [Falsehoods about Pagination](https://www.hezmatt.org/~mpalmer/blog/2018/12/12/falsehoods-programmers-believe-about-pagination.html) - Why your pagination algorithm is giving someone (possibly you) a headache.
- [Falsehoods about garbage collection](https://paul.bone.id.au/blog/2018/10/19/gc-falsehoods/) - Misconceptions about the predictability and performance of garbage collection.
- [Myths about File Paths](https://yakking.branchable.com/posts/falsehoods-programmers-believe-about-file-paths/) - Diversity of file-systems and OSes makes file paths a little harder than we might think of.
- [Myths about CPU Caches](https://software.rajivprab.com/2018/04/29/myths-programmers-believe-about-cpu-caches/) - Misconceptions about caches often lead to false assertions, especially when it comes to concurrency and race conditions.
- [Myths about `/dev/urandom`](https://www.2uo.de/myths-about-urandom) - There are a few things about `/dev/urandom` and `/dev/random` that are repeated again and again. Still they are false.
- [Hi! My name is…](https://www.youtube.com/watch?v=NIebelIpdYk) - This talk could have been named "falsehoods about usernames (and other identifiers)".
- [Popular misconceptions about `mtime`](https://apenwarr.ca/log/20181113) - Part of a post on why file's `mtime` comparison could be considered harmful.
- [Rules for Autocomplete](http://jeremymikkola.com/posts/2019_03_19_rules_for_autocomplete.html) - Not falsehoods *per-se*, but still a great list of good practices to implement autocompletion.
- [Floating Point Math](https://0.30000000000000004.com) - "Your language isn't broken, it's doing floating point math. (…) This is why, more often than not, `0.1 + 0.2 != 0.3`."
- [The Hidden Complexity of Downloading Favicons, Told in 15+ Edge Cases](https://www.simplecto.com/complexity-downloading-favicons-told-in-15-plus-edge-cases/) - Downloading that little icon you see in you browser tabs should be a simple exercise. It turned out to be a lot more complicated than you think. Be vigilant that you are not shaving a Yak.
- [Norway is not False](https://mobile.twitter.com/chrisjrn/status/1232016100038266880) - Norway's ISO country code is also valid YAML for False.

## Typography<a name="typography"></a>

- [Falsehoods about Fonts](https://github.com/RoelN/Font-Falsehoods) - Assumptions about typography on the web and in desktop applications.
- [Truths programmers should know about case](https://www.b-list.org/weblog/2018/nov/26/case/) - A complete reverse of the falsehoods format, on the topic of case (as in uppercase and lowercase text).

## Video Games<a name="video-games"></a>

- [The Door Problem](https://lizengland.com/blog/2014/04/the-door-problem/) - All the things you have not considered implementing for your doors in games.

## Contributing<a name="contributing"></a>

Your contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/kdeldycke/awesome-falsehood/blob/main/.github/contributing.md) first.

## Footnotes<a name="footnotes"></a>

The [header image](https://github.com/kdeldycke/awesome-falsehood/blob/main/assets/awesome-falsehood-header.jpg) is based on a modified [photo taken in February 2010 by Iza Bella](https://commons.wikimedia.org/wiki/File:BLW_Truth_and_Falsehood.jpg), distributed under a [Creative Commons BY-SA 2.0 UK license](https://creativecommons.org/licenses/by-sa/2.0/uk/deed.en).

<!--lint disable no-undefined-references-->

<a name="intro-quote-def">\[1\]</a>: [*Notebooks, 1914-1916*, page 14e](https://archive.org/details/notebooks191419100witt/page/n35) (Harper & Brothers, New York, 1961). [\[↑\]](#intro-quote-ref)
