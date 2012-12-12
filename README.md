# JavaScript Implementations (Presentation for [CopenhagenJS}(http://copenhagenjs.dk)

Mindmap/notes:


- Intro
    - Introduction
        - Excuse to read up on JavaScript Engines
        - Made yesterday night
        - My background
    - Overview of talk
        - Intro to major open source JavaScript implementations
        - Selected features
        - Unselected implementations
- Different implementations
    - v8
        - Chrome
        - node.js, CouchBase, ...
        - Full compiler + optimising compiler
    - JavaScriptCore
        - Safari
        - Qt 4.7+, ...
        - LLIN, Baseline JIT, DFG JIT
    - SpiderMonkey
        - Firefox
        - Adobe acrobat, CouchDB, MongoDB, ...
        - Trace-(tracing), Jäger-, and  Ion-(ssa, current beta) -monkey
    - Nashorn and Rhino
        - JavaScript on Java (version 8 for Nashorn)
        - Nashorn: not released yet, node.js-api-prototype
        - piggybacking on JVM (jit, gc, (invokedynamic), etc.)
- Selected features
    - Inline caches (nb: monomorphic)
    - Hidden classes / type inference (nb: object assignment order)
    - Values: SMI(v8), NaN-boxing(spidermonkey+jsc) (or nun-boxing), Java-objects
    - Generational Garbage Collection(v8, java) (on way for JSC, still mark'n'sweep for spidermonkey)
- Conclusion
    - Summary
    - Feedback welcome
    - Questions?

## TODO

- make presentation mindmap
- make slides
- fix transitions/style in slides

## Notes

- most of the files (except index.html and readme) is the slideshow engine from https://github.com/hakimel/reveal.js/
## Links

- http://www.youtube.com/watch?v=kul3HO3WRgI
