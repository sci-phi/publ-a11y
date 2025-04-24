# Publishing scripts

These bash scripts were developed to simplify the document publishing process.

## Requirements

On mac you have to install `checklink` (I've tried to install version 5.0.0 on mac, but I got errors). These terminal commands should work:

```
sudo cpan install App::cpanminus
sudo cpanm W3C::LinkChecker@4.81
sudo cpan install Mozilla::CA
```

## publish-guidelines.sh

Script for creating static version for the guidelines document. It starts from the published draft (in the main branch): [https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.1/draft/guidelines/](https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.1/draft/guidelines/)

It generates the static version, it runs nuchecker and link checker.

The output is a zip folder that can be sent to W3C staff for publishing on the website.

## publish-techniques.sh

Script for creating static version for the techniques documents. It starts from the published draft (in the main branch):

- [https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.1/draft/techniques/epub-metadata/](https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.1/draft/techniques/epub-metadata/)
- [https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.1/draft/techniques/onix-metadata/](https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.1/draft/techniques/onix-metadata/)

It generates the static versions, it runs nuchecker and link checker.

The output saved in the "live" directory `a11y-meta-display-guide/2.1/techniques`.