porter2-stemmer
===============

A stemmer helps convert similar words into a common form so that they can be accurately compared, regardless of tense/part of speech/etc.

An implementation of the Porter2 stemming algorithm in C#

    http://snowball.tartarus.org/algorithms/english/stemmer.html
    
This is a fork of the GitHub repo:

    https://github.com/nemec/porter2-stemmer

For example:

    friend -> friend  
    friendly -> friend  
    friends -> friend  
    friend's -> friend

This fork contains changes for some words.  For example:

    impersonate -> impersonat (not imperson)
    personate -> personat (not person)
    witness -> witness (not wit)
    
Some words that should be stemmed differently than the default Porter2 algorithm are found at https://github.com/alphagov/rummager/blob/master/config/schema/stems.yml
