# atomic-tei

This is an Atom package providing a validating editing environment for documents conforming to a TEI P5 schema.  It is a fork of <https://github.com/aerhard/xml-demo-package>, configured to use TEI P5's "TEI all" `.rng` schema.


## Requirements

-  [Atom Editor](https://atom.io/), with [linter-autocomplete-jing](https://github.com/aerhard/linter-autocomplete-jing) installed.


## One-time setup

From a terminal in this directory, run

    apm link


## Usage

XML files with filename extension `.tei` will be validated against TEI P5 as you edit.  You can use the template file in `xml/template.tei`.



## More information

The three directories `grammar`, `settings` and `teischemas` configure the Atom package.  If you want to modify settings (e.g., to configure different file extensions for validation with TEI), please see the documentation for the source package this is cloned from:  <https://github.com/aerhard/xml-demo-package>.
