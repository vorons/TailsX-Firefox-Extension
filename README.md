# TailsX-Firefox-Extension
**TailsX** is a privacy-respecting, ad-free, self-hosted Google metasearch engine with strong security that offers full API support and utilizes Qwant for images, Brave Search for videos, and DuckDuckGo for auto-complete.

[**Original TailsX repository on GitHub**](https://github.com/Extravi/tailsx).

# How does it work?
Extension use `manifest.json` settings which change your main search engine.

Example:

(**Default settings**)
```json
{
  "chrome_settings_overrides": {
    "search_provider": {
      "search_url": "https://example.com/search?q={searchTerms}",
      "suggest_url": "https://example.com/suggestions?q={searchTerms}",
    }
  }
}
```

(**With addon**)
```json
{
  "chrome_settings_overrides": {
    "search_provider": {
      "search_url": "https://search.nya.pub/search?q={searchTerms}",
      "suggest_url": "https://search.nya.pub/suggestions?q={searchTerms}",
    }
  }
}
```

It means that your browser starts to use second link when you make search request.

# Tricks
If you want use **TailsX** as support to main search engine do this:
- fork this repository and change the search URL according to your domain
- add this addon into your browser
- agree when browser shows you "Add this extension?"
- disagree when browser shows "Do you want change your main search engine?"
- use keywords like `@tailsx, @tx` if you want use **TailsX** when you make request

# Distribute your extension
https://extensionworkshop.com/documentation/publish/
