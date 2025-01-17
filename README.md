# Library_Template

[![build status][1]][2]
[![codecov][3]][4]
[![license][5]][6]
[![latest release][7]][8]
![platforms][9]

<!--
    Above uses reference-style links with numbers.
    See also https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links.

    For example, `[![build status][1]][2]` evaluates to the following:
        `[link_text][2]`
        `[2]` is a reference to a link, i.e. `[link_text](https://...)`

        `[link_text]` = `[![build status][1]]`
        `[1]` is once again a reference to a link - this time an image, i.e. `[![build status](https://...)]
        `![build status]` is the text that should be displayed if the linked resource (`[1]`) is not available

    `[![build status][1]][2]` hence means:
    Show the picture linked under `[1]`. In case it cannot be displayed, show the text "build status" instead.
    The picture, or alternative text, should link to `[2]`.
-->

[1]: https://img.shields.io/github/actions/workflow/status/seqan/library-template/ci_linux.yml?branch=main&style=flat&logo=github&label=CI "Open GitHub actions page"
[2]: https://github.com/seqan/library-template/actions?query=branch%3Amain
[3]: https://codecov.io/gh/seqan/library-template/branch/main/graph/badge.svg?token=BH1FQiBBle "Open Codecov page"
[4]: https://codecov.io/gh/seqan/library-template
[5]: https://img.shields.io/badge/license-BSD-green.svg "Open Copyright page"
[6]: https://github.com/seqan/library-template/blob/main/LICENSE.md
[7]: https://img.shields.io/github/release/seqan/library-template.svg "Get the latest release"
[8]: https://github.com/seqan/library-template/releases/latest
[9]: https://img.shields.io/badge/platform-linux%20%7C%20bsd%20%7C%20osx-informational.svg

## Quick start

You may want to replace `LIBRARY_TEMPLATE` with your library name:

```bash
# Rename files
find $(pwd) -type f -not -path '*/\.git/*' -iname "library_template*" -exec bash -c 'mv $1 ${1/library_template/<your_lib>}' bash {} \;
# Rename directories
find $(pwd) -type d -not -path '*/\.git/*' -iname "library_template*" -exec bash -c 'mv $1 ${1/library_template/<your_lib>}' bash {} \;
# Rename occurrences in files
find $(pwd) -type f -not -path '*/\.git/*' -exec sed -i 's/LIBRARY_TEMPLATE/<YOUR_LIB>/g' {} \;
find $(pwd) -type f -not -path '*/\.git/*' -exec sed -i 's/Library_Template/<Your_Lib>/g' {} \;
find $(pwd) -type f -not -path '*/\.git/*' -exec sed -i 's/library_template/<your_lib>/g' {} \;
# Rename URLs
find $(pwd) -type f -not -path '*/\.git/*' -exec sed -i 's/seqan\/library-template/<repo_owner>\/<repo_name>/g' {} \;
```

## Sponsorships

[![Vercel](https://raw.githubusercontent.com/seqan/library-template/main/test/documentation/.vercel/powered-by-vercel.svg)](https://vercel.com/?utm_source=seqan&utm_campaign=oss)

Vercel is kind enough to sponsor our documentation preview-builds within our pull requests. Check them out!
