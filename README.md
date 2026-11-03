# chromosomix-docs

The published documentation of [chromosomix](https://github.com/js2264/chromosomix), served by GitHub
Pages at **<https://doc.chromosomix.app>**.

Nothing here is written by hand. The documentation's source is
[`documentation/`](https://github.com/js2264/chromosomix/tree/main/documentation) in
js2264/chromosomix, and its workflow,
[`docs.yml`](https://github.com/js2264/chromosomix/blob/main/.github/workflows/docs.yml), builds it and
writes the site into the **`gh-pages`** branch of this repository, which is what Pages serves:

```
/                the latest release's copy
/v0.20.0/        each release's copy, built from its tag, kept for ever
/dev/            main's copy, rebuilt on every push
/versions.json   what is published, which every copy's version menu reads
```

Each publish replaces `gh-pages` with a single commit, so the branch holds the site and not its
history; any copy can be built again from its tag. To change a page, change its source in
js2264/chromosomix (see its
[`documentation/README.md`](https://github.com/js2264/chromosomix/blob/main/documentation/README.md));
a change pushed here is lost at the next publish.
