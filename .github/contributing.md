# Contributing

Your contributions are always welcome! Here are some guidelines.

## Good Candidates

Before contributing, make sure the new link you'd like to add is a good
candidate.

Here is a non-restrictive list of items which are good candidates for inclusion
in this awesome list.

### Falsehood Articles

Articles following the *falsehood* schema are prime candidates for inclusion in
this awesome list.

These articles starts with the hypothesis that developers have a naive and
simple view of a domain. Then proceed to list a set of candid assumptions that
might be held by programmers. Each one is intentionally false, and in their
best form are illustrated with a counter-example.

A list of falsehood is crafted as a progression that is designed to refine
concepts. Having read the whole list of falsehood, the reader should possess a
better overview of a domain while dispelling its myths, point out common
pitfalls and demonstrate its subtleties.

*falsehood* articles are, in a sense, a suite of wordy unit-tests covering
extensive edge-cases provided by real-world usage. The world is messy.
Discovering a domain to be much more complex than anticipated will lead to
frustrations. And cause flipping tables `(╯°□°)╯︵ ┻━┻`. This is the sign of a
great candidate for that list!

Articles featuring items that are applicable to one product (or a service) and
one only can't be considered as generic enough and should be avoided.

### Libraries

Programming libraries or modules are good candidates too, if they solve or
reduce the complexities pointed to by *falsehood* articles above.

That way we can put back tables in place. `┬─┬ ノ( ゜-゜ノ)`

### Data Structures

Data models and structures generic enough to cover and address most of the
falsehoods are also welcome in this page.

## Pull-requests and issues

- Search past and current issues and pull-requests for previous suggestions before making a new one. Yours may be a duplicate or a work in progress.

- Only one list item per commit.

- Only one commit per pull-request. Always squash commits after applying changes.

- Check your spelling and grammar.

- Add the reason why the linked resource is awesome. And what it adds to the existing corpus.

- Keep the translated content up-to-date with your proposal. Propagate changes to all `readme.*.md` files. Rely on automatic translation tools. Bilingual contributors will refine the result later.

## Linting

Have your pull-request pass the [official Awesome List's linter](https://github.com/sindresorhus/awesome-lint).

No extra work is required here as it is [already integrated by the way of GitHub actions](https://github.com/kdeldycke/awesome-falsehood/tree/main/.github/workflows).

To run the linter locally, do:

```shell-session
$ npm i npx
$ npx awesome-lint
```

## Formatting

Additional rules not covered by `awesome-lint`, to keep the content clean and tidy.

If one of these rule conflict with the linter, the linter's rule should takes precedence. Apply it.

### General content

- Remove any trailing whitespaces.

- Use spaces, no tabs, for indention.

- Apostrophes should be using the single ASCII mark: `'`.

- Try to quote the original content as-is to summarize the point of the linked content.

- If a straight quote doesn't cut it, feel free to paraphrase both the item's title and description. Remember, this is curation: we are increasing the value of the original content by aggregation and categorization. And also by smart editorializing. You just need to respect the spirit of the original content.

### Sections

- Sections are in alphabetical order, as all topics are independent from each others.

- Section might feature one paragraph introduction and a figure (graph, drawing, photo).

### Item title

- Link title must be stripped out of the "*Programmers believe*" part to keep it compact.

- URLs must use HTTPs protocol, if available.

- No `“` and `”` curved quotation marks. This is reserved for original content quotation in descriptions.

- To quote, use either the single or double variations: `'` and `"`. Keep them properly balanced.

### Item description

- Try to provide an actionable TL;DR as a description, quoting the original text if it stands by itself.

- [Removes `TL;DR:` prefix in description](https://github.com/kdeldycke/awesome-iam/commit/537cbfd8beaca18d44a0962e107a6db9171a0345). Every description is a short summary anyway.

- Quotes should be properly delimited with the `“` and `”` curved quotation marks.

- You can reduce the original text by using an ellipsis in parenthesis `(…)`.

- For quoting inside a quote, use single or double `'` and `"` ASCII marks. Keep them properly balanced.

- To serialize a list into a description, use the following format:

  > Text of a description summarizing the item. And here is a list coming from the original content about **“a random subject: 1. Blah blah blah; 2. Blah blah blah? 3. Blah blah blah.”** And a bit more text to conclude.

  This format provides visual anchor points that help readability and quick content scanning.

  - You can skip some items from the original list and renumber it.

  - You shouldn't have to re-order it though.

- An additional link in the description is allowed. This must be limited to some rare cases. Like pointing to a bigger concept, an acronym definition, or reference material (book, biography, …).

### CLI helpers

One-liners to fix-up some common formatting mistakes. Use with great caution and always double-check and edit the results.

- Replaces star list item markers by dashes:

  ```shell-session
  $ sed -i 's/^* /- /g' ./README.md
  ```

- Replaces typographic quotes with ASCII ones:

  ```shell-session
  $ sed -i "s/‘/\'/g" ./readme.md
  $ sed -i "s/’/\'/g" ./readme.md
  ```

- Forces quotes to end with a dot:

  ```shell-session
  $ sed -i 's/`$/`\./g' ./readme.md
  ```

[Other one-liners are available](https://kevin.deldycke.com/2006/12/text-date-document-processing-commands/) on my blog.
