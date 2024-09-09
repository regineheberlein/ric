This is a rudimentary implementation of the RiC-CM as XML for testing purposes.

### Implementation principles:
- Classes are represented as elements
- Properties (CM relations) are implemented as elements
- Properties (CM attributes) are implemented as xml attributes if they take a controlled term
- Properties (CM attributes) are implemented as xml elements if they take free text

### Implementation decisions:
- The schema does not implement inverse relations
- It does not implement relation hierarchies
- It implements controlled vocabularies as local files (CVL directory)

### Limitations:
- This schema does not enforce the right-hand class constraints of object properties

A complementary [Wikibase test implementation](https://recordsincontexts.wikibase.cloud) is in progress.
