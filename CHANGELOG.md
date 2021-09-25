# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [Revision 20] - 2011-04-26

### Fixed

- Fixed a typo resulting in `FIRST_ORDERED_NODE_TYPE` results being wrong,
  thanks to <shi_a009 (at) hotmail.com>.

## [Revision 19] - 2005-11-29

### Changed

- Nodesets now store their nodes in a height balanced tree, increasing
- performance for the common case of selecting nodes in document order,
  thanks to Sébastien Cramatte <contact (at) zeninteractif.com>.
- AVL tree code adapted from Raimund Neumann <rnova (at) gmx.net>.

## [Revision 18] - 2005-10-27

### Added

- DOM 3 XPath support. Caveats:
  - Namespace prefixes aren't resolved in XPathEvaluator.createExpression,
    but in XPathExpression.evaluate.
  - XPathResult.invalidIteratorState is not implemented.

## [Revision 17] - 2005-10-25

### Fixed

- Some core XPath function fixes and a patch to avoid crashing certain
  versions of MSXML in PathExpr.prototype.getOwnerElement, thanks to
  Sébastien Cramatte <contact (at) zeninteractif.com>.

## [Revision 16] - 2005-09-22

### Fixed

- Workarounds for some IE 5.5 deficiencies.
- Fixed problem with prefix node tests on attribute nodes.

## [Revision 15] - 2005-05-21

### Fixed

- Fixed problem with QName node tests on elements with an xmlns="...".

## [Revision 14] - 2005-05-19

### Fixed

- Fixed QName node tests on attribute node regression.

## [Revision 13] - 2005-05-03

### Fixed

- Node tests are case insensitive now if working in an HTML DOM.

## [Revision 12] - 2005-04-26

### Changed

- Updated licence.
- Slight code changes to enable use of Dean
  Edwards' script compression, <http://dean.edwards.name/packer/ >.

## [Revision 11] - 2005-04-23

### Fixed

- Fixed bug with 'and' and 'or' operators, fix thanks to
  Sandy McArthur <sandy (at) mcarthur.org>.

## [Revision 10] - 2005-04-15

### Fixed

- Added support for a virtual root node, supposedly helpful for
  implementing XForms.
- Fixed problem with QName node tests and
- the parent axis.

## [Revision 9] - 2005-03-17

### Fixed

- Namespace resolver tweaked so using the document node as the context
  for namespace lookups is equivalent to using the document element.

## [Revision 8] - 2005-02-13

### Added

- Handle implicit declaration of 'xmlns' namespace prefix.
- Instance data can now be associated with a FunctionResolver.

### Fixed

- Fixed bug when comparing nodesets.
- Workaround for MSXML not supporting 'localName' and 'getElementById',
  thanks to Grant Gongaware.
- Fix a few problems when the context node is the root node.

## [Revision 7] - 2005-02-11

### Fixed

- Default namespace resolver fix from Grant Gongaware
  <grant (at) gongaware.com>.

## [Revision 6] - 2005-02-10

### Fixed

- Fixed bug in 'number' function.

## [Revision 5] - 2005-02-09

### Fixed

- Fixed bug where text nodes not getting converted to string values.

## [Revision 4] - 2005-01-21

### Added

- Implemented union '|' operator.

### Fixed

- Bug in 'name' function, thanks to Bill Edney.
- Fixed incorrect processing of namespace nodes.
- Fixed NamespaceResolver to resolve 'xml' namespace.

## [Revision 3] - 2005-01-14

### Fixed

- Fixed bug with nodeset comparisons, bug lexing < and >.

## [Revision 2] - 2004-10-26

### Fixed

- QName node test namespace handling fixed.
- Few other bug fixes.

## [Revision 1] - 2004-08-13

### Fixed

- Bug fixes from William J. Edney <bedney (at) technicalpursuit.com>.
- Added minimal licence.

## [Revision 0] - 2004-06-14

### Added

- Initial version

[unreleased]: https://github.com/olivierlacan/keep-a-changelog/compare/revision20...HEAD
[revision 20]: https://github.com/olivierlacan/keep-a-changelog/compare/revision19...revision20
[revision 19]: https://github.com/olivierlacan/keep-a-changelog/compare/revision18...revision19
[revision 18]: https://github.com/olivierlacan/keep-a-changelog/compare/revision17...revision18
[revision 17]: https://github.com/olivierlacan/keep-a-changelog/compare/revision16...revision17
[revision 16]: https://github.com/olivierlacan/keep-a-changelog/compare/revision15...revision16
[revision 15]: https://github.com/olivierlacan/keep-a-changelog/compare/revision14...revision15
[revision 14]: https://github.com/olivierlacan/keep-a-changelog/compare/revision13...revision14
[revision 13]: https://github.com/olivierlacan/keep-a-changelog/compare/revision12...revision13
[revision 12]: https://github.com/olivierlacan/keep-a-changelog/compare/revision11...revision12
[revision 11]: https://github.com/olivierlacan/keep-a-changelog/compare/revision10...revision11
[revision 10]: https://github.com/olivierlacan/keep-a-changelog/compare/revision9...revision10
[revision 9]: https://github.com/olivierlacan/keep-a-changelog/compare/revision8...revision9
[revision 8]: https://github.com/olivierlacan/keep-a-changelog/compare/revision7...revision8
[revision 7]: https://github.com/olivierlacan/keep-a-changelog/compare/revision6...revision7
[revision 6]: https://github.com/olivierlacan/keep-a-changelog/compare/revision5...revision6
[revision 5]: https://github.com/olivierlacan/keep-a-changelog/compare/revision4...revision5
[revision 4]: https://github.com/olivierlacan/keep-a-changelog/compare/revision3...revision4
[revision 3]: https://github.com/olivierlacan/keep-a-changelog/compare/revision2...revision3
[revision 2]: https://github.com/olivierlacan/keep-a-changelog/compare/revision1...revision2
[revision 1]: https://github.com/olivierlacan/keep-a-changelog/compare/revision0...revision1
[revision 0]: https://github.com/olivierlacan/keep-a-changelog/releases/tags/revision0
