# git undo generator

Three questions in, one exact command out: was the commit pushed, do you keep
the changes, does anyone else pull the branch. The tool prints the right
`git reset`, `git revert` or reflog rescue — with a warning where the command
bites.

**Use it: <https://mrsaynothing.dev/en/hub/git-undo?utm_source=github&utm_medium=referral>**

## Why

Search data says people don't want a version-control essay mid-crisis. This
site ranked for "git reset last commit keep changes" at position ~12 with zero
clicks — the query wants a command, not reading. The generator answers in one
screen. The reasoning behind every row of the decision table lives in the
companion posts:

- [Git undo last commit: keep changes, stay safe](https://mrsaynothing.dev/en/blog/2026-09-03/git-undo-last-commit?utm_source=github&utm_medium=referral)
- [git revert vs reset](https://mrsaynothing.dev/en/blog/2026-09-15/git-revert-vs-reset?utm_source=github&utm_medium=referral)
- [Undo Anything in Git — the full recovery map](https://mrsaynothing.dev/en/hub/git-undo?utm_source=github&utm_medium=referral)

## Run it

Zero build, zero dependencies:

```bash
# open index.html, or serve it
python3 -m http.server 8080
```

Everything runs client-side. No account, no upload, no analytics, no cookies.

## Embed it

One static file — drop it anywhere, keep the MIT notice:

```html
<iframe
  src="https://mrsaynothing.dev/en/hub/git-undo?utm_source=embed&utm_medium=referral"
  title="Git undo generator"
  style="width:100%;max-width:44rem;height:38rem;border:1px solid #2a2a2a;border-radius:8px"
  loading="lazy"></iframe>
```

Or self-host: copy `index.html`, serve it, done.

Made by [mrsaynothing.dev](https://mrsaynothing.dev/?utm_source=github&utm_medium=referral)
— one post a day, every claim tested or consolidated from named sources.

The version embedded in [mrsaynothing.dev](https://mrsaynothing.dev/?utm_source=github&utm_medium=referral)
is the same logic as a static SvelteKit route.

## License

MIT — fork it, restyle it, rip out the wording.
