langdog
=============
Trainable Python programming language detection module based on Bayesian probability. Langdog is inspired by http://stackoverflow.com/questions/475033/detecting-programming-language-from-a-snippet

## Getting started

Some sample code on how to use langdog.

    import langdog

    lang_classifier = langdog.LangClassifier()
    lang_classifier.train(open("code.pl").read(), "perl")
    lang_classifier.train(open("code.php").read(), "php")
    lang_classifier.classify(open(sys.argv[1]).read())
