# Wepwawet

```
                                          =
                                     -:  .=.
                                     -=  -+:
                                    .-*  -#=
                                    :-- --#=
                                    :.:.+=#+
                                    :  =:=#+
                              ..::..      #*
                       ::..::.   .--.     -+
                      .-               .  .*
                        -====++==::::-- .  #
                                .:+#=.     *-
                                   =.......=*
                                   =........*+
                                   -        .#+
                                  -          :#*
                                 ::           +===-:::................::-=-.
                                .-           :.                           .-=
                               -                               ::           +
  888       888               :.                           ..:.             :=  888
  888   o   888  ............::        .. .           .:::....              :#  888
  888  d8b  888                      .=- ............*.                     +#  888
  888 d888b 888  .d88b.  88888b.  888  888  888  8888b.  888  888  888  .d88b.  888888
  888d88888b888 d8P  Y8b 888 "88b 888  888  888     "88b 888  888  888 d8P  Y8b 888
  88888P Y88888 88888888 888  888 888  888  888 .d888888 888  888  888 88888888 888
  8888P   Y8888 Y8b.     888 d88P Y88b 888 d88P 888  888 Y88b 888 d88P Y8b.     Y88b.
  888P     Y888  "Y8888  88888P"   "Y8888888P"  "Y888888  "Y8888888P"   "Y8888   "Y888
                         888
                         888
                         888

```

Wepwawet is an url information gathering tool. Wepwawet gathers data from a variety of sources,
including Shodan, and more to come.

## Getting Started

### Prerequisites

- Python 3 is required

### Installing

Please note that Wepwawet is in alpha.

```
git clone https://github.com/Melk0rr/Wepwawet.git
cd Wepwawet
pip install  -r requirements.txt
pip install .
```

## Usage

      Usage:
        wepwawet (-t TARGET | -f FILE) [options]
        wepwawet -h
        wepwawet (-V | --version)

      Options:
        -h --help                       show this help message and exit
        -t --target                     set target (comma separated, no spaces, if multiple)
        -f --file                       set target (reads from file, one domain per line)
        -o --output=FILENAME            save to filename
        -s --shodan                     request shodan API for informations
        -S --silent                     simple output, one per line
        -v --verbose                    print debug info and full request output
        -V --version                    show version and exit
        --check-tls                     retrieve TLS version accepted by the target
        --export-csv=CSV                save results as csv
        --geo-locate                    geo locate the target
        --http-info                     perform basic request to the target

      Exemples:
        wepwawet -t https://www.google.com/ -s --export-csv ./test/wepoutput.csv
        wepwawet -f ./tests/targets.txt -s --geo-locate --http-info --export-csv ./test/wepoutput.csv
        wepwawet -t https://www.google.com/ --check-tls

      Help:
        For help using this tool, please open an issue on the Github repository:
        https://github.com/Melk0rr/Wepwawet
    
    
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
