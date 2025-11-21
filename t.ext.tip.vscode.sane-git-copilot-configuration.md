---
id: yyktscml2r7o8gdpjgnvp2h
title: Sane Git Copilot Configuration (for Markdown)
desc: ''
updated: 1751553244811
created: 1749139527533
---

[GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) is a convenient way to enable AI assistance in VSCode.

However, we do NOT recommend enabling automatic inline suggestions in your markdown files.

<div class="central-tech-thought-centered">

Remember: Writing is thinking.
</div>

When AI automatically suggests how to finish non-obvious sentences, it can **disrupt your train of thought**. However, using AI to finish obvious sentences can provide a helpful productivity boost (and reduce finger strain).

To get the best of both worlds: enable GitHub Copilot (or your preferred AI assistant), **but** configure it to only show suggestions when you **explicitly** request them. This way, you gain productivity benefits without interrupting your writing (and thinking) process.


### PreReqs
[Set up GitHub Copilot in VS Code](https://code.visualstudio.com/docs/copilot/setup)

### How to Configure GitHub Copilot to Only Show Suggestions When You Request Them

#### Disable Automatic Inline Suggestions in Markdown
- Go to settings.
- In your settings, look for:
```txt
github.copilot.enable
```
- Under `github.copilot.enable` configuration, set `markdown:false`

![img](./assets/images/Screenshot_2025-06-05_at_10.13.04 AM.png){max-width: 500px, display: block, margin: 0 auto, border: 5px solid black}

#### Add Shortcut for Inline Suggestions
In your keyboard shortcuts, look for:

```txt
editor.action.inlineSuggest.trigger
```

Assign an easy-to-use shortcut (I use `CTRL+J CTRL+K` to stay on the home row).

![img](./assets/images/Screenshot_2025-06-05_at_10.17.23 AM.png){max-width: 500px, display: block, margin: 0 auto, border: 5px solid black}


### Related
- [[t.ext.tip.keyboard.get-rid-of-caps-lock]]