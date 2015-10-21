A trilingual glossary of legislative jargon, insofar as it pertains to the
Cypriot parliament.  The glossary follows the
[JSKOS specification](https://gbv.github.io/jskos/jskos.html), a strict JSON-LD
adaptation of SKOS; but it is written in YAML, a superset of JSON, for the sake
of readability and ease of editing.  The glossary namespace is `opag`, but this
is subject to change.

Eventually, the glossary will be consumed by the *openpatata* website.

## Adding a new entry to the glossary

Entries are alphabetised.  To add a new entry, copy and paste the template
below, replacing `<id>` with a camelCase, one- or two-word, unique,
English-language identifier (e.g. "committeeMeeting").  The `prefLabel` is the
canonical name of the concept in each of the three languages (`el` for Greek;
`en` for English; and `tr` for Turkish), the `definition` is a plain-language
description of it, and the `altLabel` is a list of synonyms.  Other properties
are available; see the [table of concepts](https://gbv.github.io/jskos/jskos.html#concepts).

```yaml
- uri: opag:<id>
  type: ["http://www.w3.org/2004/02/skos/core#Concept"]
  prefLabel:
    el:
    en:
    tr:
  altLabel:
    el:
    -
    en:
    -
    tr:
    -
  definition:
    el:
    en:
    tr:
```

## Resources

- [EuroVoc](http://eurovoc.europa.eu/)
- [OpenGovLD/skos](https://github.com/OpenGovLD/skos)

## License

`openpatata-glossary` is licensed under CC BY 4.0.
