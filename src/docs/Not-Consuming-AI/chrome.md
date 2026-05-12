# Chrome

The web browser from Google.

## Changing your search engine

Most search engines show AI-generated summaries by default. Complete the following steps to choose a search engine that doesn't:

1. Open Chrome.
2. Open a new tab, and enter `chrome://settings/search` in the address bar.
3. select **Manage search engines and site search**.
4. Scroll down to the **Site search** section, and then select **Add**.
5. In the **Add Site Search** panel, enter a name. For example, `No AI`.
6. In the **Shortcut** field, enter a short, easy to remember shortcut. For example `@noai`. You won't need to use this shortcut if you complete step 9.
7. In the **URL with %s in place of query** field, choose one of the following:
    * To use Google, enter `https://google.com/search?q=%s&udm=14`.
    * To use DuckDuckGo, enter `https://noai.duckduckgo.com/?q=%s`.
8. Select **Add**.
9. **Optional**: For the site search that you just created, select **More actions** (three vertical dots), and then select **Make default**.

Now, whenever you use the address bar to search, the browser will use your non-AI search engine.

If you don't set the new search engine as your default, you can use your shortcut to access the site search. In the address bar, enter the shortcut that you chose, press the Tab key, and then enter your search query.

## Turning off the local AI model

In May 2026, it was widely reported that Google was installing a local AI model on people's computers, without their knowledge. Use the following instructions to remove the file and block it from being reinstalled.

!!! note "Note" 
    For more information, refer to [Google Chrome silently installs a 4 GB AI model on your device without consent. At a billion-device scale the climate costs are insane.](https://www.thatprivacyguy.com/blog/chrome-silent-nano-install/).

1. Open Chrome.
2. Open a new tab, and enter `chrome://settings/system` in the address bar.
3. Turn off **On-device AI**, if the setting is shown.
4. Enter `chrome://flags/` in the address bar.
5. In the search field, enter `optimization guide`.
6. For the **Enables optimization guide on device** setting, select **Disabled** from the list.
7. Select the **Relaunch** button that appears. Alternatively, close and reopen Chrome.
8. Choose one of the following options:
    * On a Windows device, open Windows Explorer, and go to `%LOCALAPPDATA%\Google\Chrome\User Data\`.
    * On a Mac, open Finder, and go to `~/Library/Application Support/Google/Chrome`.
9. Look for an `OptGuideOnDeviceModel` folder, and delete it if you find it. The main issue is a 4 GB `weights.bin` file that would be in that folder.