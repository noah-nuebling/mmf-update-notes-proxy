# mmf-update-notes-proxy

On the mac-mouse-fix/update-feed branch we create html files containing update notes for each release. However, when accessing them via raw.githubusercontent their mime type is text/plain instead of text/html. 
This prevents them from being displayed correctly by the Sparkle update window in Mac Mouse Fix.

This repo provides a proxy which 'copies' the content of one of the update-notes html files servers as a properly mime-typed html document.

Alternative:
  Another solution would be to host the html files on GitHub pages directly. Then they would be served with the right mime type. But that's awkward because then we'd have to commit the GitHub page of the mac-mouse-fix repo entirely to the update-feed branch. (I think, as of [Feb 2025])

Example usage:
```
https://noah-nuebling.github.io/mmf-update-notes-proxy/?url=https://raw.githubusercontent.com/noah-nuebling/mac-mouse-fix/update-feed/update-notes/html/en/3.0.3.html
```

Also see: 
- BetterDisplay appcast system:
  - appcast.xml: https://betterdisplay.pro/betterdisplay/sparkle/appcast.xml
  - changelog.html script: (Similar to this) https://waydabber.github.io/BetterDisplay/changelog.html

---

Credits to Claude AI
