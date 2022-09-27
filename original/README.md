
# preprint-template.tex
An information-dense, two-column LaTeX template designed for, e.g., [EarthArXiv](https://eartharxiv.org) preprints. Some compiled examples can be seen [here](https://eartharxiv.org/repository/view/1095/) or [here](https://eartharxiv.org/repository/view/268/).

This repository is forked and somewhat heavily modified from https://github.com/kourgeorge/arxiv-style. 

The default version of preprint-template.tex optionally uses [arara](https://github.com/cereda/arara) directives to automate compilation. Arara is probably already included in your TeX distribution (TeX Live or MiKTeX). To use arara with [TexShop](https://pages.uoregon.edu/koch/texshop/), move `arara.engine` from `~/Library/TeXShop/Engines/Inactive/Arara` to `~/Library/TeXShop/Engines`. To make this the default, you can also set `Preferences`>`Typesetting`>`Command Listed Below`>`arara`.
