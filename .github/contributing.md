# Contributing

Your contributions are always welcome! Here are some guidelines.

## Editorial line

The editorial line is [describe in the intro of the main list](https://github.com/kdeldycke/awesome-engineering-team-management#readme).

Items are roughly ordered like so:

1. At first we'll find content appealing to software developers or new managers. We're reaching for accessibility and targets the wider audience and provide a gentle introduction.
1. Then we can have a couple of real use-cases or anecdotes, which makes the subject more hands-on and relatable.
1. Third we might add a couple of reference material to generalize concepts, provide methodical solutions and expose broader thinking frameworks.
1. At the end comes the most cynical or bleak content, which have some utility as cautionary tales, or as warning signals of deteriorating conditions.

## Status

This repository has reached an equilibrium state. We are past its accumulation phase, and in the middle of the curation process. Meaning we're more into refining its concepts, smooth the progression and carefully evaluating the addition of new content.

## Pull-requests and issues

- Search past and current issues and pull-requests for previous suggestions before making a new one. Yours may be a duplicate or a work in progress.

- Only one list item per commit.

- Only one commit per pull-request. Always squash commits after applying changes.

- Check your spelling and grammar.

- Add the reason why the linked resource is awesome. And what it adds to the existing corpus.

- Keep the translated content up-to-date with your proposal. Propagate changes to all `readme.*.md` files. Rely on automatic translation tools. Bilingual contributors will refine the result later.

## Linting

Have your pull-request pass the [official Awesome List's linter](https://github.com/sindresorhus/awesome-lint).

No extra work is required here as it is [already integrated by the way of GitHub actions](https://github.com/kdeldycke/awesome-template/tree/main/.github/workflows).

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

- Sections are not in the alphabetical order, to provide a progression, from general to specific topics.

- Section might feature one paragraph introduction and a figure (graph, drawing, photo).

### Item title

- URLs must use HTTPs protocol, if available.

- No `“` and `”` curved quotation marks. This is reserved for original content quotation in descriptions.

- To quote, use either the single or double variations: `'` and `"`. Keep them properly balanced.

### Item description

- Try to provide an actionable TL;DR as a description, quoting the original text if it stands by itself.

- [Removes `TL;DR:` prefix in description](https://github.com/kdeldycke/awesome-engineering-team-management/commit/da298ec1c39fe62fd4553e1a6de0ad4494602c57). Every description is a short summary anyway.

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

## FAQ

Some cases to illustrate the curation process.

### Can I rewrite your sentences and paragraphs?

Yes. I'm a non-native speaker, so some of my writings might be a little bit fancy. If you can propose a shorter, to the point, and accurate version of my initial text, go for it! These improvements [adds a lot of readability for both kind of readers](https://github.com/kdeldycke/awesome-falsehood/pull/105).

### Can I propose YouTube videos for the list?

Yes, but try to pin-point the start of the video to a relevant time. Like with the `&t=13m30s` parameter in YouTube URLs.

Better than a video: have a link to its written transcript. Or presentation slides if it doesn't dillute the point being made.

### Can I link to an X thread?

Yes, but try to search first in the content produced by the author: sometimes the said author edited its rant into a more digestible article elsewhere. We'll prefer to link to that.

### How to prevent link-rot?

[As pointed by a contributor](https://github.com/kdeldycke/awesome-engineering-team-management/issues/52#issue-1499417056):

> The links here have a tendency to go offline. For this to be a resource of long term value, link-rot can be avoided by archiving the pages.

Which is true.

I have no issue replacing the original URL with an alternative archived/cached link if the original is no longer reachable.

Broken URLs are frustrating. We will fix them one by one. Some have been moved to a new domain. Some have completely disappear, so we'll replace them with a `archive.org` link.

If you find a broken one, please propose a PR to fix it. Or just report it as an issue and I'll do the work.

### How are you going to archive articles that went offline?

This question points to the paradox that we need to archive them *before* they go offline.

There is no rush to pre-emptively archive content. Incentives exists for others to do it:

- This list is popular enough for its content to be picked up by regular archival crawlers.
- Popular content in this list are naturally archived by users who value them.
- Authors who cares about their content, or benefits from the SEO juice this list provides, have an incentive to keep them available at their original URL.

Despites these incentives, there is still a non-zero chance for content to disappear entirely from the web, with no archived copy in `archive.org`. That's not the end of the world. Maybe the content wasn't worth it, and not good for inclusion in the first place. Think of this edge-case as a natural selection process on content, which helps natural curation.

### Why removes inactive GitHub projects?

Unmaintained GitHub repositories are usually [archived by their owners](https://docs.github.com/en/repositories/archiving-a-github-repository/archiving-repositories). But some are de-facto unmaintained, or abandoned as-is by their author, without being explicitly archived.

Either way, if the space they addresses is crowded, and there are other repositories referenced in the list, the link is a good candidate for deletion to reduce noise.

On the other hand, if the project has been forked or rebooted elsewhere, we can now point out to the new location.

### Why my commercial project is not in the list?

Probably because the core content is behind a paywall. Especially if there are better resources online, which are more extensive, and freely accessible.

This is especially true for SaaS and other licensed software. If there is an open-source project available, we'd rather point to that instead of commercial solutions.

These alternatives don't need to be better. They qualify if they're good enough to derives inspiration from, or starts something without barriers to entry.

So for as set of multiple overlapping projects, we will consider commercial ones as duplicates and remove them, to keep the list lean.

### Why my link was rejected?

If your link was rejected, it must have been motivated and explained to the contributor as a comment to your PR.

Some reasons for rejection, which often overlaps, includes:

- deviance from these contribution guidelines
- violation of the [code of conduct](code-of-conduct.md)
- duplicate content
- lack of motivation in what the new link adds to the existing corpus
- lack of originality
- overcrowded section that [needs more curation than additional content](https://github.com/kdeldycke/awesome-iam/pull/76)
- [commercially-sponsored content only proposed for SEO](https://github.com/kdeldycke/awesome-falsehood/pull/31#issuecomment-407667679)
- lack of feedback from the contributor on raised questions

### How can I force a link into the list?

If your contribution has been declined, there is a way to bypass the curation rules. You can [purchase a sponsorship](https://github.com/sponsors/kdeldycke) and have your product, logo and link at the top of this repository! 🤗 Like [Descope did for a year](https://twitter.com/kdeldycke/status/1676963147104784386) on the [awesome IAM list](https://twitter.com/kdeldycke/status/1676963147104784386).

## FAQ (falsehoods)

This questions are specifics to the [Awesome Falsehood](https://github.com/kdeldycke/awesome-falsehood) project.

### Why don't you copy the falsehoods in the list?

This might be a good idea to compile all falsehoods in the repository. It would allow the community to maintain them, and enrich them. It could also improve the overall quality as most external articles don't make the effort to illustrate or explain why a falsehood is a falsehood.

But that is a big endeavor, so to keep things simple, we just make a collection of external articles in this list. In the mean time, if you'd like to add falsehoods, I will ask potential contributors to [host them elsewhere](https://github.com/kdeldycke/awesome-falsehood/issues/46).

Also, if we had to host the raw falsehoods in this repository, we might have to [check on the licence and seek permission from the original author](https://github.com/kdeldycke/awesome-falsehood/issues/24#issuecomment-354112401).
