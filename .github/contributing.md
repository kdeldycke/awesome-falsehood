# Contributing

Your contributions are always welcome! Here are some guidelines.

## Status

This repository has reached an equilibrium state. We are past its accumulation phase, and in the middle of the curation process. Meaning we're more into refining its concepts, smooth the progression and carefully evaluating the addition of new content.

## Pull-requests and issues

- Search past and current issues and pull-requests for previous suggestions before making a new one. Yours may be a duplicate or a work in progress.

- Only one list item per commit.

- Only one commit per pull-request. Always squash commits after applying changes.

- Check your spelling and grammar.

- Add the reason why the linked resource is awesome. And what it adds to the existing corpus.

- GitHub repositories must meet these baseline criteria:

  1. **At least 50 stars.** A minimum traction signal to filter out unknown projects.
  2. **Not archived.** Archived repositories signal the author has moved on.
  3. **Updated within the last 3 years.** Repositories with no push in 3+ years are considered stale.

  These are defaults, not absolutes. Maintainers may make exceptions depending on the nature of the content. Static resources (reading lists, essays, falsehood articles, data sets) don't need regular commits to remain valuable. Archived repositories with high community adoption can still serve as references. Active software projects, on the other hand, are held to stricter expectations on all three criteria.

- Keep the translated content up-to-date with your proposal. Propagate changes to all `readme.*.md` files. Rely on automatic translation tools. Bilingual contributors will refine the result later.

## Linting

Your pull-request should pass the [official Awesome List's linter](https://github.com/sindresorhus/awesome-lint).

No extra work is required here as it is [already integrated by the way of GitHub actions](https://github.com/kdeldycke/awesome-falsehood/tree/main/.github/workflows).

You can still anticipate issues by running the linter locally with:

```shell-session
$ npx awesome-lint
```

## Formatting

Here are additional rules not covered by the `awesome-lint` CLI.

If one of these rule conflict with the linter, the linter's rule should takes precedence. Apply it.

### General content

- Remove any trailing whitespaces.

- Use spaces, no tabs, for indention.

- Apostrophes should be using the single ASCII mark: `'`.

- For description, try to identify the single best quote form the original content.

- If a quote couldn't be found to serve as a summary, feel free to paraphrase both the item's title and description. Remember, this is curation: we are increasing the value of the original content by aggregation and categorization. And also by smart editorializing. You just need to respect the spirit of the original content.

### Sections

- Sections **are not intentionally sorted in the alphabetical order**. That is to provide a progression, from general to specific topics.

> [!IMPORTANT]
> Exceptionally in `awesome-falsehood`, sections **are in alphabetical order**, as all topics are independent from each others.

- Section might feature one paragraph introduction and a figure (graph, drawing, photo).

### URL

- Use HTTPs protocol, if available.

- Must be reachable by CI/CD jobs. If the domain return `40x` errors for rate-limiting or content protection, replace it with a stable link:

  - [`sci-hub.st`](https://sci-hub.st) for research papers
  - [`archive.ph`](https://archive.ph) for news articles
  - [`archive.org`](https://archive.org) for anything else

- Some platforms gate content behind authentication and return `403` to anonymous traffic (Quora, most social-network discussions, paywalled news sites without an archive copy): do not use them, find an alternative source.

- When a GitHub repository has been transferred to a new owner, update the URL to the new canonical location instead of relying on the redirect (the old `OWNER/REPO` namespace can be reclaimed by anyone, which would leave the link pointing at unrelated content).

- When a vendor blog disappears (acquisition, rebrand, decommissioned subdomain), wrap the original URL with `https://web.archive.org/web/<YYYYMMDDhhmmss>/` rather than a fuzzy year prefix: a specific timestamp is more durable than letting Wayback pick the closest snapshot at request time.

### Item title

- No `“` and `”` curved quotation marks. This is reserved for original content quotation in descriptions.

- To quote, use either the single or double variations: `'` and `"`. Keep them properly balanced.

> [!IMPORTANT]
> In `awesome-falsehood`, link titles must be stripped out of the "*Programmers believe*" part to keep it compact.

### Item description

- Try to provide an actionable TL;DR as a description, quoting the original text if it stands by itself.

- [Removes `TL;DR:` prefix in description](https://github.com/kdeldycke/awesome-engineering-team-management/commit/da298ec1c39fe62fd4553e1a6de0ad4494602c57). Every description is a short summary anyway.

- Quotes should be properly delimited with the `“` and `”` curved quotation marks.

- You can reduce the original text by using an ellipsis in parenthesis `(…)`.

- For quoting inside a quote, use single or double `'` and `"` ASCII marks. Keep them properly balanced.

- To serialize a list into a description, use the following format:

  > Text of a description summarizing the item. And here is a list coming from the original content about **“three important topics: 1. Blah blah blah; 2. Blah blah blah? 3. Blah blah blah.”** And a bit more text to conclude.

  This format provides visual anchor points that help readability and quick content scanning.

  - You can skip some items from the original list and renumber it.

  - You shouldn't have to re-order it though.

- An additional link in the description is allowed. This must be limited to some rare cases. Like pointing to a bigger concept, an acronym definition, or reference material (book, biography, …).

### Licensing markers

For tool, dataset, and project entries, prefix the description with one of two emoji to inform readers about the project's commercial posture. Articles, papers, blog posts, news items, and curation lists are not marked.

- 💸 — the project's primary maintainer is a commercial vendor selling a paid version of this software: hosted cloud, Enterprise tier, or proprietary modules on top of the OSS core. The marker is informational, not a quality judgment: it tells the reader that some advanced features (compliance, audit log retention, multi-tenancy add-ons, integrations) may live outside the OSS distribution. Do not apply when the vendor only sells support, SLA, or managed hosting without feature gating (Red Hat for Keycloak, for instance).

- 🆓 — the project is fully open-source without a commercial vendor extracting value through feature gating: foundation-governed (CNCF, Apache Software Foundation, Eclipse), community-driven, corporate-OSS released without a paid product alongside (Lyft's Cartography, Yahoo's Athenz, Salesforce's Policy Sentry, Microsoft's Presidio), or sold only with support contracts (Red Hat for Keycloak).

Format: `- [Project](url) - 💸 Description.` or `- [Project](url) - 🆓 Description.`. The two markers are mutually exclusive: a project gets one or the other, never both. Awesome-lint accepts the format unchanged.

## Editorial line

The general editorial line for each list is [hinted in their introduction](https://github.com/kdeldycke/awesome-template#readme).

There's also some specific rules depending on the list:

### [`awesome-engineering-team-management`](https://github.com/kdeldycke/awesome-engineering-team-management): items order

Items are roughly ordered like so:

1. At first we'll find content appealing to software developers or new managers. We're reaching for accessibility and targets the wider audience and provide a gentle introduction.
2. Then we can have a couple of real use-cases or anecdotes, which makes the subject more hands-on and relatable.
3. Third we might add a couple of reference material to generalize concepts, provide methodical solutions and expose broader thinking frameworks.
4. At the end comes the most cynical or bleak content, which have some utility as cautionary tales, or as warning signals of deteriorating conditions.

### [`awesome-falsehood`](https://github.com/kdeldycke/awesome-falsehood): candidates

Before contributing, make sure the new link you'd like to add is a good candidate.

Here is a non-restrictive list of items which are good candidates for inclusion in the `awesome-falsehood` list.

#### Falsehood articles

Articles following the *falsehood* schema are prime candidates for inclusion in this awesome list.

These articles starts with the hypothesis that developers have a naive and simple view of a domain. Then proceed to list a set of candid assumptions that might be held by programmers. Each one is intentionally false, and in their best form are illustrated with a counter-example.

A list of falsehood is crafted as a progression that is designed to refine concepts. Having read the whole list of falsehood, the reader should possess a better overview of a domain while dispelling its myths, point out common pitfalls and demonstrate its subtleties.

*falsehood* articles are, in a sense, a suite of wordy unit-tests covering extensive edge-cases provided by real-world usage. The world is messy. Discovering a domain to be much more complex than anticipated will lead to frustrations. And cause flipping tables `(╯°□°)╯︵ ┻━┻`. This is the sign of a great candidate for that list!

Articles featuring items that are applicable to one product (or a service) and one only can't be considered as generic enough and should be avoided.

#### Libraries

Programming libraries or modules are good candidates too, if they solve or reduce the complexities pointed to by *falsehood* articles above.

That way we can put back tables in place. `┬─┬ ノ( ゜-゜ノ)`

#### Data structures

Data models and structures generic enough to cover and address most of the falsehoods are also welcome in this page.

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

[As pointed by a contributor](https://github.com/kdeldycke/awesome-engineering-team-management/issues/52):

> The links here have a tendency to go offline. For this to be a resource of long term value, link-rot can be avoided by archiving the pages.

Which is true.

I have no issue replacing the original URL with an alternative archived/cached link if the original is no longer reachable.

Broken URLs are frustrating. We will fix them one by one. Some have been moved to a new domain. Some have completely disappear, so we'll replace them with an [archived link](#url).

If you find a broken one, please propose a PR to fix it. Or just report it as an issue and I'll do the work.

### How are you going to archive articles that went offline?

This question points to the paradox that we need to archive them *before* they go offline.

There is no rush to pre-emptively archive content. Incentives exists for others to do it:

- This list is popular enough for its content to be picked up by regular archival crawlers.
- Popular content in this list are naturally archived by users who value them.
- Authors who cares about their content, or benefits from the SEO juice this list provides, have an incentive to keep them available at their original URL.

Despites these incentives, there is still a non-zero chance for content to disappear entirely from the web, with no [archived copy](#url). That's not the end of the world. Maybe the content wasn't worth it, and not good for inclusion in the first place. Think of this edge-case as a natural selection process on content, which helps natural curation.

### Why removes inactive GitHub projects?

Unmaintained GitHub repositories are usually [archived by their owners](https://docs.github.com/en/repositories/archiving-a-github-repository/archiving-repositories). But some are de-facto unmaintained, or abandoned as-is by their author, without being explicitly archived.

Either way, if the space they addresses is crowded, and there are other repositories referenced in the list, the link is a good candidate for deletion to reduce noise.

On the other hand, if the project has been forked or rebooted elsewhere, we can now point out to the new location.

### Why my commercial project is not in the list?

Probably because the core content is behind a paywall. Especially if there are better resources online, which are more extensive, and freely accessible.

This is especially true for SaaS and other licensed software. If there is an open-source project available, we'd rather point to that instead of commercial solutions.

These alternatives don't need to be better. They qualify if they're good enough to derives inspiration from, or starts something without barriers to entry.

So for as set of multiple overlapping projects, we will consider commercial ones as duplicates and remove them, to keep the list lean.

See also [Why my open-source project was removed?](#why-my-open-source-project-was-removed) for the open-core-heavy pattern, which applies even when the project is technically open-source.

### Why my open-source project was removed?

A permissive license on the GitHub repo is not enough. We also evaluate whether the project is genuinely usable in production without paying. The pattern we filter out is *open-core-heavy*: a project that ships an OSS shell while gating essential features behind a paid Enterprise tier or a hosted Cloud add-on.

What counts as an *essential feature* depends on the domain of the list. For an authentication or access-management project, MFA, SSO protocols (SAML, OIDC, LDAP federation), multi-tenancy, fine-grained permissions, SCIM/directory sync, audit logs, and admin UI are essential. For a data tooling project, the equivalent core capabilities are essential. The maintainer for each list will spell out the domain-specific list in its FAQ or in PR review comments.

When any of these is absent from the OSS distribution, sold as a per-feature add-on, kept in a separate proprietary directory (like a non-OSS-licensed `ee/` folder), or priced per-MAU, the project will not be listed alongside true-OSS alternatives in an overcrowded section.

A few softer signals, evaluated together, also count against a listing:

- The vendor's pricing page lists what looks like core features as paid tiers.
- The project README explicitly mentions a "protective barrier" or "premium features" reserved for cloud.
- Self-hosting the OSS version requires assembling several separate primitives the vendor only ships pre-integrated as a paid product.

Existing entries that pass the licensing test but fall into open-core-light (some advanced compliance or directory-sync integrations gated, but the core works in OSS) may still be listed when they cover a distinct niche. Such entries are flagged with the 💸 marker in the description.

See also [Why my commercial project is not in the list?](#why-my-commercial-project-is-not-in-the-list) for the fully-paywalled case where no OSS distribution exists.

### Why my project was removed for inactivity?

In addition to [archived repositories](#why-removes-inactive-github-projects), we also remove projects whose author has formally retired them: a notice in the README pointing users to a different project, or a public statement that "new projects should no longer rely on this", is treated as a stronger signal than the GitHub archive flag alone.

Acquisitions that result in the OSS repo being maintained-but-not-developed (Dependabot bumps and copyright touch-ups only, with the company's roadmap on a successor commercial product) are also grounds for removal in overcrowded sections.

### Why my link was rejected?

If your link was rejected, it must have been motivated and explained to the contributor as a comment to your PR.

Some reasons for rejection, which often overlaps, includes:

- duplicate content
- lack of originality
- rehash of existing content
- no motivation to explain what the new link adds to the existing corpus
- overcrowded section that [does not need more content, but more curation](https://github.com/kdeldycke/awesome-iam/pull/76)
- [not generic enough, or too specific to a single product or company](https://github.com/kdeldycke/awesome-falsehood/pull/31#issuecomment-407667679)
- marketing copy made to juice the list for SEO
- [too much URLs already pointing out to the same commercial domain name](https://github.com/kdeldycke/awesome-iam/pull/179#issuecomment-3023031941) (2 links are enough)
- lack of feedback from the contributor on raised questions
- deviance from these contribution guidelines
- violation of the [code of conduct](code-of-conduct.md)

### How can I force a link into the list?

If your contribution has been declined, there is a way to bypass the curation rules. You can [purchase a sponsorship](https://github.com/sponsors/kdeldycke) and have your product, logo and link at the top of this repository! 🤗 Like [Descope did for a year](https://twitter.com/kdeldycke/status/1676963147104784386) on the [awesome IAM list](https://twitter.com/kdeldycke/status/1676963147104784386).

## FAQ for [`awesome-falsehood`](https://github.com/kdeldycke/awesome-falsehood)

This questions are specifics to the [Awesome Falsehood](https://github.com/kdeldycke/awesome-falsehood) project.

### Why don't you copy the falsehoods in the list?

This might be a good idea to compile all falsehoods in the repository. It would allow the community to maintain them, and enrich them. It could also improve the overall quality as most external articles don't make the effort to illustrate or explain why a falsehood is a falsehood.

But that is a big endeavor, so to keep things simple, we just make a collection of external articles in this list. In the mean time, if you'd like to add falsehoods, I will ask potential contributors to [host them elsewhere](https://github.com/kdeldycke/awesome-falsehood/issues/46).

Also, if we had to host the raw falsehoods in this repository, we might have to [check on the licence and seek permission from the original author](https://github.com/kdeldycke/awesome-falsehood/issues/24).
