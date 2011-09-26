langdog
=============
Trainable Python programming language detection module based on Bayesian probability

## Getting started

import langdog

lang_classifier = langdog.LangClassifier()
lang_classifier.train(open("code.pl").read(), "perl")
lang_classifier.train(open("code.php").read(), "php")
lang_classifier.classify(open(sys.argv[1]).read())
