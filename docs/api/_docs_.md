---
tilte: lsd module _docs_
description: lsd module _docs_ description
---


# lsd module _docs_

This script defines several functions for documentation tasks.

* `lsd-mod.docs.mkdocs` Builds a documentation site using the mkdocs command and a configuration file specified as an argument or located at the default location mkdocs.yml.

* `lsd-mod.docs.pandoc.markdown2latex` Converts a Markdown document in the clipboard to a LaTeX document using the pandoc command, and copies the result to the clipboard.

* `lsd-mod.docs.mkdocs.link` Creates a symbolic link to a built documentation site located in the _site directory of the current working directory in the user's public_html directory.

* `lsd-mod.docs.mkdocs.serve` Serves a built documentation site located in the _site directory of the current working directory using the mkdocs command.

* `lsd-mod.docs.mkdocs.clean` Removes the built documentation site located in the _site directory of the current working directory.

* `lsd-mod.docs.asciidoc.link` Creates a symbolic link to an AsciiDoc documentation site located in the current working directory in the user's public_html directory.

* `lsd-mod.docs.asciidoc.clean` Removes an AsciiDoc documentation site located in the current working directory.

* `lsd-mod.docs.asciidoc.serve` Serves an AsciiDoc documentation site located in the current working directory using the asciidoctor command.

* `lsd-mod.docs.asciidoc.convert` Converts an AsciiDoc documentation site located in the current working directory to HTML using the `as

* `lsd-mod.docs.asciidoc.publish` converts an AsciiDoc documentation site located in the current working directory to HTML using the asciidoctor command and publishes the result to the user's public_html directory.

* `lsd-mod.docs.asciidoc.install` installs the required dependencies for building an AsciiDoc documentation site.

* `lsd-mod.docs.asciidoc.build` builds an AsciiDoc documentation site located in the current working directory using the asciidoctor command.

* `lsd-mod.docs.asciidoc.pdf` converts an AsciiDoc documentation site located in the current working directory to a PDF document using the asciidoctor-pdf command.

* `lsd-mod.docs.asciidoc.push` pushes an AsciiDoc documentation site located in the current working directory to a Git repository.

* `lsd-mod.docs.asciidoc.rebuild` rebuilds an AsciiDoc documentation site located in the current working directory using the asciidoctor command.

* `lsd-mod.docs.asciidoc.update` updates the dependencies for an AsciiDoc documentation site located in the current working directory.

* `lsd-mod.docs.asciidoc.update.gemfile` updates the Gemfile for an AsciiDoc documentation site located in the current working directory.