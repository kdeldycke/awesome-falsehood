# Awesome Falsehood [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [![git-brag-stats](https://labs.turbo.run/git-brag?user=kdeldycke&repo=awesome-falsehood)](https://github.com/turbo/git-brag)

A curated list of awesome falsehoods programmers believe in.

> The logic of the world is prior to all truth and falsehood.
> - Ludwig Wittgenstein


## Contents

- [Foreword](#foreword)
- [Meta](#meta)
- [Business](#business)
- [Dates and Time](#dates-and-time)
- [Emails](#emails)
- [Geography](#geography)
- [Human Identity](#human-identity)
- [Networks](#networks)
- [Phone Numbers](#phone-numbers)
- [Postal Addresses](#postal-addresses)
- [Software Engineering](#software-engineering)
- [Contributing](#contributing)
- [Good Candidates](#good-candidates)
    - [*Falsehood* Articles](#falsehood-articles)
    - [Libraries](#libraries)
    - [Data Structures](#data-structures)
- [License](#license)


## Foreword

*Falsehood* articles are a form of commentary on a particular subject, and are
appreciated by the developer community at large for their effectiveness and
terseness. They're a convenient written form to approach an unfamiliar domain
by dispelling myths, point out common pitfalls, show inconsistencies and
subtleties.

In a sense, *Falsehood* articles are a suite of wordy unit-tests covering
extensive edge-cases provided by real-world usage.


## Meta

- [Falsehoods Programmers
Believe](http://spaceninja.com/2015/12/08/falsehoods-programmers-believe/) - A
brief list of common falsehoods. A great overview and quick introduction into
the world of falsehoods.


## Business

- [Falsehoods About Online
Shopping](http://wiesmann.codiferes.net/wordpress/?p=22201) - Covers prices,
currencies and inventory.
- [Falsehoods About
Prices](https://gist.github.com/rgs/6509585) - Covers currencies, amounts and
localization.
- [`tax`](https://github.com/commerceguys/tax) - A PHP 5.4+ tax management
library.


## Dates and Time

- [Falsehoods About
Time](http://infiniteundo.com/post/25326999628/falsehoods-programmers-believe-about-time) -
Seminal article on dates and time.
- [More Falsehoods About
Time](http://infiniteundo.com/post/25509354022/more-falsehoods-programmers-believe-about-time) -
Part. 2 of the article above.
- [Falsehoods About Time and Time
Zones](http://www.creativedeletion.com/2015/01/28/falsehoods-programmers-date-time-zones.html) -
Another takes on time-related falsehoods, with an emphasis on time zones.
- [Critique of Falsehoods About
Time](https://gist.github.com/thanatos/eee17100476a336a711e) - Takes on the
first article above and provides an explanation of each falsehood, with more
context and external resources.
- [Time Zone Database](https://www.iana.org/time-zones) - Code and data that
represent the history of local time for many representative locations around
the globe.
- [The Long, Painful History of Time](http://naggum.no/lugm-time.html) - Most
of the idiosyncracies in time keeping can find an explanation in history.
- [You Advocate a Calendar Reform](https://qntm.org/calendar) - Your idea will
not work. This article tells you why.
- [So You Want to Abolish Time Zones](https://qntm.org/abolish) – Abolishing
timezones may sound like a good idea, but there are quite a few complications
that make it not quite so.


## Emails

- [I Knew How to Validate an Email Address Until I Read the
RFC](http://haacked.com/archive/2007/08/21/i-knew-how-to-validate-an-email-address-until-i.aspx/) -
Provides intricates examples that are unsuspected valid emails according the
RFC-822.


## Geography

- [Falsehood About
Geography](http://wiesmann.codiferes.net/wordpress/?p=15187) - Takes on places,
their names and locations.
- [Falsehoods About
Maps](http://www.atlefren.net/post/2014/09/falsehoods-programmers-believe-about-maps/) -
Covers coordinates, projection and GIS.


## Human Identity

- [Falsehoods About
Names](https://www.kalzumeus.com/2010/06/17/falsehoods-programmers-believe-about-names/) -
The article that started it all.
- [Falsehoods About
Gender](https://gist.github.com/garbados/f82604ea639e0e47bf44) - Gender is part
of human identity and has its own subtleties.
- [Gay Marriage: The Database Engineering Perspective](https://qntm.org/gay) -
How to store a marriage in a database while addressing most of the falsehoods
about gender, naming and relationships.
- [XKCD #327: Exploits of a
Mom](https://xkcd.com/327/) - Funny take on how implementation of a falsehood
might lead to security holes.
- [Hello, I’m Mr. Null. My Name Makes Me Invisible to
Computers](https://www.wired.com/2015/11/null/) - Real-life example on how
implemented falsehood has negative impact on someone's life.
- [HL7 v3
RIM](http://www.hl7.org/implement/standards/product_brief.cfm?product_id=186) -
A flexible data model for representing human names.
- [Apple iOS
`NSPersonNameComponentsFormatter`](https://developer.apple.com/library/ios/documentation/Miscellaneous/Reference/NSPersonNameComponentsFormatter_Class/index.html) -
Localized representations of the components of a person’s name.


## Networks

- [Falsehoods About
Networks](http://blog.erratasec.com/2012/06/falsehoods-programmers-believe-about.html) -
Covers TCP, DHCP, DNS, VLANs and IPv4/v6.


## Phone Numbers

- [Falsehoods About Phone
Numbers](https://github.com/googlei18n/libphonenumber/blob/master/FALSEHOODS.md) -
Covers phone numbers, their representation and meaning.
- [`libphonenumber`](https://github.com/googlei18n/libphonenumber) - Google's
common Java, C++ and JavaScript library for parsing, formatting, and validating
international phone numbers. Also available for
[C#](https://github.com/erezak/libphonenumber-csharp),
[Objective-C](https://github.com/iziz/libPhoneNumber-iOS),
[Python](https://github.com/daviddrysdale/python-phonenumbers),
[Ruby](https://github.com/sstephenson/global_phone) and
[PHP](https://github.com/giggsey/libphonenumber-for-php).


## Postal Addresses

- [Falsehoods About
Addresses](https://www.mjt.me.uk/posts/falsehoods-programmers-believe-about-addresses/) -
Covers streets, postal codes, buildings, cities and countries.
- [Letter Delivered Despite No Name, No
Address](https://twitter.com/loriskumo/status/735851511331356672) - Ultimate
falsehood about postal addresses: you do not need one.
- [`libaddressinput`](https://github.com/googlei18n/libaddressinput) - Google's
common C++ and Java library for parsing, formatting, and validating
international postal addresses.
- [`addressing`](https://github.com/commerceguys/addressing) - A PHP 5.4+
addressing library, powered by Google's dataset.
- [`postal-address`](https://github.com/scaleway/postal-address) - Python
module to parse, normalize and render postal addresses.


## Software Engineering

- [Falsehoods About
Versions](https://github.com/xenoterracide/falsehoods/blob/master/versions.md) -
Attributing an identity to a software release might be harder than thought.
- [Falsehoods About Build
Systems](http://pozorvlak.livejournal.com/174763.html) - Building software is
hard. Building software that builds software is harder.
- [Big List of Naughty
Strings](https://github.com/minimaxir/big-list-of-naughty-strings) - Challenge
your assumptions about strings.
- [i18n Testing Data](https://github.com/patch/i18n-testing) - Real-word
international and diverse name data for unit testing and QA.


## Contributing

Your contributions are always welcome! Please take a look at the [contribution
guidelines](CONTRIBUTING.md) first.


## Good Candidates

Here is a non-restrictive list of items which are good candidates for inclusion
in this awesome list.

### *Falsehood* Articles

Articles following the *falsehood* scheme are prime candidates for inclusion in
this awesome list.

These articles starts with the hypothesis that developers have a naive, simple
view of the subject at hand. Then proceed to list a set of candid assumptions
that might be held by such programmers. Each one is intentionally false, and
sometimes illustrated by a counter-example.

A list of falsehood is crafted as a progression that is designed to refine
concepts. Having read the whole list of falsehood, the reader should possess a
global, if not complete, overview of the domain being targeted by the article,
including most, if not all, its pitfalls, edges-cases and inconsistencies.

In the worst case, these articles might provoke an emotional reaction and cause
flipping table. `(╯°□°)╯︵ ┻━┻`

### Libraries

When possible, we provide a list of programming libraries or modules that may
solve, or try to, the complexities and idiosyncrasies pointed by the
*falsehood* articles above.

So we can put back tables in place. `┬─┬ ノ( ゜-゜ノ)`

### Data Structures

Data models and structures generic enough to cover and address most of the
falsehoods are also welcome in this page.


## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

Content of this repository is licensed under the [Creative Commons CC0
license](https://creativecommons.org/publicdomain/zero/1.0/).

To the extent possible under law, [Kevin Deldycke](http://kevin.deldycke.com)
has waived all copyright and related or neighboring rights to this work.
