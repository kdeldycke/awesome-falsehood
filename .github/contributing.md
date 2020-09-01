# Contributing

Your contributions are always welcome! Here are some guidelines.


## Good Candidates

Before contributing, make sure the new link you'd like to add is a good
candidate.

Here is a non-restrictive list of items which are good candidates for inclusion
in this awesome list.


### Falsehood Articles

Articles following the *falsehood* scheme are prime candidates for inclusion in
this awesome list.

These articles starts with the hypothesis that developers have a naive, simple
view of the subject at hand. Then proceed to list a set of candid assumptions
that might be held by the programmers. Each one is intentionally false, and
in their best form illustrated by a counter-example.

A list of falsehood is crafted as a progression that is designed to refine
concepts. Having read the whole list of falsehood, the reader should possess a
global, if not complete, overview of the domain being targeted by the article,
including most, if not all, its pitfalls, edges-cases and inconsistencies.

Sometimes, these kind of articles might provoke an emotional reaction and cause
flipping table. `(╯°□°)╯︵ ┻━┻` Because, the world is messy. Discovering the
complexity of a domain that is simple in appearance will lead to
frustrations. This is the sign of a great candidate for that list!

Articles featuring items that are applicable to one product (or a service) and
one only can't be considered as generic enough and should be avoided.


### Libraries

Programming libraries or modules are good candidates too, if they solve or
reduce the complexities pointed to by the *falsehood* articles above.

That way we can put back tables in place. `┬─┬ ノ( ゜-゜ノ)`


### Data Structures

Data models and structures generic enough to cover and address most of the
falsehoods are also welcome in this page.


## Pull-Request and Issue

- Search past and current issues and pull-requests for previous suggestions
before making a new one, as yours may be a duplicate or a work in progress.

- Only one list item per commit.

- Only one commit per pull-request. Always squash commits after applying
  changes.

- Check your spelling and grammar.

- Remove any trailing whitespaces.

- Use spaces, no tabs, for indention.

- Send a pull-request with the reason why the linked resource is awesome.


## Linting

First and foremost, have your pull-request pass the [official Awesome List's
linter](https://github.com/sindresorhus/awesome-lint). No extra work is
required here as it is [already integrated by the way of GitHub
actions](https://github.com/kdeldycke/awesome-falsehood/tree/master/.github/workflows).

To run the linter locally, do:

```
$ npm install --global awesome-lint
$ awesome-lint
```


## Additional rules

Here are some formatting style not enforced by the linter (yet), which are
specific to this awesome list.

- Cut long lines of text after 80 characters. Only exception is to let Markdown
content be properly rendered.

- If one of these rule conflict with the linter, the linter's rule should takes
precedence. Apply it.


## List items

- Link title must be [title-cased](http://titlecapitalization.com), AP style.

- Link title must be stripped out of the "*Programmers believe*" part to keep
it compact (we all know the scheme).

- URL must use HTTPs protocol if available.

- Keep descriptions concise, maximum number of characters is 350.


## Sections

- Sections must be alphabetically sorted.

- Add a section if needed.

- Eventually add a description to the section.
