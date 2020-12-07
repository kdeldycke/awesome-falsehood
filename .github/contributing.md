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

- Search past and current issues and pull-requests for previous suggestions before making a new one, as yours may be a duplicate or a work in progress.

- Only one list item per commit.

- Only one commit per pull-request. Always squash commits after applying changes.

- Check your spelling and grammar.

- Add the reason why the linked resource is awesome. And what it adds to existing content.

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

- If a straight quote doesn't cut it, feel free to paraphrase both the item's title and description. Remember, this is curation: we are increasing the value of the original content by aggregation and categorization, yes, but also by smart editorializing. As long as you respect the spirit of the original content it's OK.

### Sections

- Sections are in alphabetical order, as all topics are independent from each others.

- Section might feature one paragraph introduction and a figure (graph, drawing, photo).

### Item title

- Link title must be stripped out of the "*Programmers believe*" part to keep it compact.

- URL must use HTTPs protocol if available.

- No `“` and `”` curved quotation marks. This is reserved for original content quotation in descriptions.

- To quote, use either the single or double variations: `'` and `"`. Keep them properly balanced.

### Item description

- Quotes should be properly delimited with the `“` and `”` curved quotation marks.

- You can reduce the original text by using an ellipsis in parenthesis `(…)`.

- For quoting inside a quote, use single or double `'` and `"` ASCII marks. Keep them properly balanced.

- To serialize a list into a description, use the following format:

  > This is my own description. Here is a list quoted from the original content about **“a random subject: 1. Blah blah blah; 2. Blah blah blah? 3. Blah blah blah.”** This makes sense right?

  This provides visual anchor points that help readability and quick content scanning.

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
