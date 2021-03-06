text-archive-engine
===================

Engine to compress and store multiple versions of text in a file

This is used by the live-archive and diff-popup Atom editor packages.  It writes and reads to/from a custom text archive file format.  It is not meant for public usage but if some has a good reason I can clean it up and make the API easier to understand and use.

### Features

- Archive
  - For simplicity all versions are kept forever
  - Archive is highly compressed
    - Text differencing
    - Bit-level binary archive format
    - Text compressed with zlib


- Reliable (virtually crash-proof)
  - All version saves are append-only in a single write
  - Archive can be backed up while in use

