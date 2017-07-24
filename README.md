# digital_source

> gh-pages friendly jekyll digital collections template

set the `_config.yml` variables

- in `_home` are index, about, and other pages that become the central portal for all collections.
- in `_data` are the metadata that drive content creation: 
    - metadata for individual digital collections is placed in `collections_info.csv` template.
    - metadata for items in a digital collection are in individual csv files in the `collection_metadata` directory.
- in `_digital_collections` are directories that represent each collection to build. `.md` stubs in these directories represent the pages that will be built for the collection.

to add a collection:

- copy the `template` directory in `_digital_collections`, and give it the collection name.
- Delete the `.md` stub page types you do NOT want to generate for the collection. Some stub templates may have special settings for the page, or content can be added.
- add an entry in `_data/collections_info.csv` for the collection. the "collection" field must match the directory name.
- Place a csv with metadata about all items in the collection in the `_data/collection_metadata` directory (following the template). The csv must be named the same as the collection directory.
