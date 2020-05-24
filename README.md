# atomic-csl

This is an Atom package providing a validating editing environment for documents conforming to a CSL schema.  It is a fork of <https://github.com/aerhard/xml-demo-package> and <https://github.com/neelsmith/atomic-tei>, configured to use CSL's `.rng` schema.


## Requirements

-  [Atom Editor](https://atom.io/), with [linter-autocomplete-jing](https://github.com/aerhard/linter-autocomplete-jing) installed.

Per [this post](https://andrewdunning.ca/getting-started-editing-tei-xml-atom), you might also add these additional package along with the above, with this command.

``` bash
apm install linter-autocomplete-jing atom-wrap-in-tag double-tag tag atom-beautify linter linter-ui-default intentions busy-signal
```

## One-time setup

From a terminal in this directory, run

    apm link

NB: if you decide to move this folder, you'll have to rerun `apm link` from the new location.


## Usage

XML files with filename extension `.csl` will be validated against CSL's `csl.rng` schema as you edit.

You can also manually set *any* XML document to use the CSL schema.  One way is to click on the file-type setting at the bottom right of the Atom window. For example, if you start up a new `Plain text` document, click on the `Plain text` label, or if you a document opens as a generic `XML` type, click on `XML`, and then choose `CSL Style` from the list of document types you're offered.  Another way to do this is to open the command palette (command-shift-p), and choose "Grammar selector: show" (control-shift-l), and choose `CSL Style`. 

## More information

The three directories `grammar`, `settings` and `schemas` configure the Atom package.  If you want to modify settings (e.g., to configure different file extensions for validation with CSL), please see the documentation for the source package this is cloned from:  <https://github.com/aerhard/xml-demo-package>.

## TODO

* Fix auto grammar application based on file extension
* Embedded schematron validation?
* Add CSL templates and maybe scripts to make creation of new, and editing existing, styles easier. For example, select author-date and apa as template, add updated element with correct datetime, etc.
