# NF-eBOT - Scrapers
Web scraper responsible to extract relevant news in Brazilian government portals.

## To build
#### First create ```doc/config.h``` with ```doc/config.h.dist``` template and run:
`./scripts/gcc_build.sh`

## Folder Structure

* `build`: where builded executable is saved
* `doc`: configuration file
* `include`: local headers
* `include/parsers`: logic of portals/sites scraped
* `lib`: vendor libs
* `scripts`: scripts to help build and install
* `spike`: files to test technologies or ideas
* `src`: main file

## TODO
* Create makefile based in `spike/gcc_build.sh`
* Make `doc/config.h` more simple
* Change all #include to use .h files
* Make const parameters in `include/helpers.h`
* Refactor this code block in `src/main.cpp`:
```
rapidxml::xml_document<> doc;
char *cstr = new char[res.size() + 1];
strcpy(cstr, res.c_str());
doc.parse<0>(cstr);
```


## Special thanks to:
[@mattgodbolt](https://github.com/mattgodbolt)
[@dascandy](https://github.com/dascandy)
[@famastefano](https://github.com/famastefano)
[@grisumbras](https://github.com/grisumbras)
[@Corristo](https://github.com/Corristo)

and other guys in [C++ Slack Group](http://cpplang.diegostamigni.com/)
