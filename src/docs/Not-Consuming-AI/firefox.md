# Firefox

The web browser from the [Mozilla Foundation](https://www.mozillafoundation.org/).

Mozilla's approach to AI features is ["You decide when, how or whether to use it at all."](https://blog.mozilla.org/en/firefox/ai-window/)

## Removing the AI chatbot shortcut from the sidebar

The sidebar provides shortcuts to things like bookmarks and your browsing history. To remove the AI chatbot from the sidebar, complete the following steps:

1. Select the gear icon in the lower-left corner of the Firefox window.
2. In the **Customize sidebar** panel, turn off the **AI chatbot** checkbox.
3. Close the **Customize sidebar** panel.

## Other AI features

Other AI features are available, but they're currently turned off by default.

## Using uBlock Origin in Firefox

uBlock Origin is a Firefox plugin that blocks content from specific domains. It's most common use is to block adverts, but you can also block content from known sources of AI.

1. Open Firefox.
2. Select the puzzle/jigsaw piece in the upper-right corner of the window.
3. In the **Find more add-ons** field, enter `ublock`, and then press **Enter**.
4. From the list of search results, select **uBlock Origin**.
5. On the **Extentions** page, select **Add to Firefox**.
6. In the permission panel, select **Add**.
7. **Optional**: In the confirmation panel, leave the **Pin extension to toolbar** checkbox selected.
8. Select **OK**.

The next step is to install the AI blocklist.

1. Go to the [uBlockOrigin-HUGE-AI-Blocklist GitHub page](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist).
2. Select the link in the **One-click import (any platform)** section.
3. Select **Subscribe**.

The uBlockOrigin-HUGE-AI-Blocklist GitHub page also includes instructions to manually install the list, if the one-click import doesn't work.

## Firefox without AI

Because Firefox is open source software, people can create their own, altered versions. One of these versions is [Waterfox](https://www.waterfox.com/). In a recent blog post, it was announced that [Waterfox would not include the majority of Firefox's AI features](https://www.waterfox.com/blog/no-ai-here-response-to-mozilla/), and never include large language models (LLMs). If you want a browser that has a similar browsing experience to Firefox, and many of the same features, but without AI, you could try Waterfox.

## Changing your search engine

Most search engines show AI-generated summaries by default. Complete the following steps to choose a search engine that doesn't:

1. Open Firefox.
2. Go to [about:preferences#search](about:preferences#search).
3. Scroll down to the **Search shortcuts** table, and then select **Add**.
5. In the **Add Search Engine** panel, enter a name. For example, `No AI`.
7. In the **URL with %s in place of search term** field, choose one of the following:
    * To use Google, enter `https://google.com/search?q=%s&udm=14`.
    * To use DuckDuckGo, enter `https://noai.duckduckgo.com/?q=%s`.
6. **Optional**: In the **Keyword (optional)** field, enter a short, easy to remember shortcut. For example `@noai`. You won't need to use this keyword if you complete step 9.
8. Select **Add Engine**.
9. **Optional**: Scroll up to the top of the page, and then select your new search engine from the **Default Search Engine** list.

Now, whenever you use the address bar to search, the browser will use your non-AI search engine.

If you don't set the new search engine as your default, you can use your keyword to access the site search. In the address bar, enter the keyword that you chose, press the Tab key, and then enter your search query.