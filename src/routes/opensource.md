<svelte:head>
  <title>Open Source - Kevin R. Whitley</title>
</svelte:head>

<style lang="scss">
  li img {
    position: relative;
    bottom: 0.1em;
    vertical-align: middle;
    max-height: 1.3em;
  }
</style>

I strongly believe in innovation through collaboration; that more eyes/feedback on a thing makes it better than the close-sourced equivalent; that we should be leading through obsession and passion, rather than through defending progress with secrets.

To this end, I not only "build-in-public" as much as I'm able, but also continuously share back tooling created along the way. Here
are a few of the more popular libraries (or just the ones I think are pretty cool):

- **[apicache](https://www.npmjs.com/package/apicache)** ![downloads](https://img.shields.io/npm/dw/apicache.svg) -
  This is the one that started it all... actually my first major published library, designed for simplifying route-caching.  At the time (and still to this day), Node/Express lacked an obvious
  and human-readable path for response caching, so apicache was my answer to that - created to minimize server work, but most importantly, reduce
  latency to the end-user requests.  Still pretty popular to this day for some reason...

- **[itty-router](https://www.npmjs.com/package/itty-router)** ![downloads](https://img.shields.io/npm/dw/itty-router.svg) -
  An ultralight (around 500 bytes) micro router for easy/elegant routing within Service Workers.  Adopted throughout much of the [Cloudflare Workers](https://workers.cloudflare.com/) community, and used extensively in the official Cloudflare documentation.  Has grown from ~100 downloads/week in December 2020 to over 3k/week within one year.

- **[itty-router-extras](https://www.npmjs.com/package/itty-router-extras)** ![downloads](https://img.shields.io/npm/dw/itty-router-extras.svg) -
  Supporting library for itty-router to further turn routing/API code into tiny, easy-to-read functions.

- **[itty-durable](https://www.npmjs.com/package/itty-durable)** ![downloads](https://img.shields.io/npm/dw/itty-durable.svg) -
  Takes the boilerplate out of working with [Cloudflare Durable Objects](https://blog.cloudflare.com/introducing-workers-durable-objects/) (DO), by automatically wiring up the required routing bits (uses itty-router internally to the DO).  This allows DO implementations to be clean and pure data/business-logic, rather than messy routing code, storage handling, or other common calls.

- **[react-data-hooks](https://www.npmjs.com/package/react-data-hooks)** ![downloads](https://img.shields.io/npm/dw/react-data-hooks.svg) -
  "Hooks"-style React API queries, to remove all the async mess of API-fetching from your component/state code. This predated react-query, which should certainly be used instead these days.

- **[use-store](https://www.npmjs.com/package/use-store)** ![downloads](https://img.shields.io/npm/dw/use-store.svg) -
  A simplified cross-component, persistable version of React's "useState" hook. Sometimes you just don't need an upstream context/provider or external state store!

- **[yarn-release](https://www.npmjs.com/package/yarn-release)** ![downloads](https://img.shields.io/npm/dw/yarn-release.svg) -
  I do a fair bit of publishing, and any  time wasted in boilerplate steps (that I'm prone to forget in the heat of the moment), is time I could be doing... literally anything else.  This library simplifies the entire process, making releasing to major/minor/patch/next/whatever versions a one-liner, including committing, pushing, tagging, version-bumping, etc.  Standard inclusion in all my public libraries.

- **[treeize](https://www.npmjs.com/package/treeize)** ![downloads](https://img.shields.io/npm/dw/treeize.svg) - From back in the day when I used to actually get relational data out of direct
  queries and needed them to be transformed to a nice API-like graph.

- and many, many others...
