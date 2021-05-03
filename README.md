# transvent

    * Package to translate between event file structures to facilitate communication between implementing packages.
    * Possible design reqs:
        * event.tsv <- -> tool specific event files
            * tools: afni, spm, fsl, nilearn, others?
        * super light weight, no deps, to lower barriers to use by other packages
        * command line interface, probably argparse
        * core functionality in C to ease import and in memory use in other laguages?
            * --OR-- core functions in python
        * How to deal with dense vs sparse?
    * Other implementation details:
        * Event file validation
        * Testing
        * best intermediate data representation? named types, list of dicts (high memory if we have dense), lightweight custom class, data objects (3.7)
        * Which repo?
        * Define IO spec, input path, output path (we don't want to always infer type)
        * Name: narrow scope (oesteban did a niitransforms), transvent?
