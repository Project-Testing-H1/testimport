# Iframe has title

## Rule Details

`<iframe>` should have a title attribute that helps identify the content. When an `<iframe>` is missing a title, screen reader users will only hear "frame". 

If the `<iframe>` does not contain meaningful content, such as Javascript, hide it from screen reader users by setting `aria-hidden="true"`. 

👎 Examples of **incorrect** code for this rule:

```erb
<iframe src="team_introduction_video.html"></iframe>
```

👍 Examples of **correct** code for this rule:

```erb
<!-- good -->
<iframe title="Team introduction" src="team_introduction_video.html"></iframe>
```

```erb
<!-- also good -->
<iframe aria-hidden="true"></iframe>
```

## Resources

- [Deque: Be Sure to Provide Titles for Iframes](https://dequeuniversity.com/tips/provide-iframe-titles).
- [Frames must have title attribute](https://dequeuniversity.com/rules/axe/3.2/frame-title)
- [jsx-eslint: iframe-has-title](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/master/docs/rules/iframe-has-title.md)