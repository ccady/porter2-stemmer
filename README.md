porter2-stemmer
===============

An implementation of the Porter2 stemming algorithm in C#
http://snowball.tartarus.org/algorithms/english/stemmer.html
A fork of the GitHub repo:
https://github.com/nemec/porter2-stemmer

A stemmer helps convert similar words into a common form so that they can be accurately compared, regardless of tense/part of speech/etc.

For example:

    friend -> friend  
    friendly -> friend  
    friends -> friend  
    friend's -> friend

This fork contains changes for some words.  For example:

    impersonate -> impersonat (not imperson)
    personate -> personat (not person)
    witness -> witness (not wit)
