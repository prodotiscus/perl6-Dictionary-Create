# Example

With `Dictionary::Create::DSL` you can create a dictionary article in .dsl format:
```perl6
use Dictionary::Create;
my $article = Dictionary::Create::DSL::Article.new;
$article.set-title('duck');
my $meaning = $article.translation('a bird');
my $section = $article.m-tag(1, $meaning);
$article.append-line($section);
say $article.give(); # will return the .dsl format article
```

# License

All files (unless noted otherwise) can be used, modified and redistributed
under the terms of the Apache License Version 2. Examples (in the
documentation, in tests or distributed as separate files) can be considered
public domain.

# Installation

To install this module, please use zef from https://github.com/ugexe/zef and
type

    zef install Dictionary::Create

or from a checkout of this source treeor from a checkout of this source tree,

    zef install .
