This is a rudimentary implementation of the [RiC-CM](https://www.ica.org/app/uploads/2023/12/RiC-CM-1.0.pdf) as XML for testing purposes.

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

### How to use:
1. download the repository
2. open `ric-cm-test.xml`
3. play around with changing the data
4. validate your changes against `RiC-CM.rnc`
5. you can change the controlled vocabulary values by
   - editing `RiC-CM.rnc` (for the shorter cvl definitions)
   - and\or editing the files in the `CVL` directory (for long cvl lists)
