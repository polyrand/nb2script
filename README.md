# nb2script

> Convert Jupyter notebooks to Python scripts or modules.

## Installation

This is a single script with 0 dependencies, so the best way to install may be just copying it to wherever you like. Then you can run it:

```sh
python3 nb2script.py --help
```

## Usage example

```sh
python3 nb2script.py -n nb2script.ipynb -s nb2s.py --cli
```

If you use the `--cli` option, the file will begin with a shebang. Otherwise, it will be converted to a standard Python module.

* `-n`: Path to the notebook to convert.
* `-s`: Path to where the script will be saved.
* `--replace`: Replace file if it exists.
* `--cli`: Export adding a shebang. Useful when creating CLI scripts, like this one.

## Alternatives

I made this after using [nbdev](https://github.com/fastai/nbdev/). Nbdev is a library that allows you to develop a python library in Jupyter Notebooks, putting all your code, tests, and documentation in one place. I have used it many times and I absolutely love it. However, it makes you use the library for the whole workflow. I wanted to create something without dependencies, simple and that I could use in any project, without having to install nbdev.

I have even kept the line that they add to every exported file:

```
# AUTOGENERATED! DO NOT EDIT! File to edit: notebook.ipynb (unless otherwise specified).
```

## Development setup

The script is created from a Jupyter notebook that can convert itself to a CLI script. The development is done in the notebook, which is the converted to a script.

## Release History

* 1.0
    * Initial release

## Meta


Ricardo Ander-Egg Aguilar – [@ricardoanderegg](https://twitter.com/ricardoanderegg) –

- [ricardoanderegg.com](http://ricardoanderegg.com/)
- [github.com/polyrand](https://github.com/polyrand/)
- [linkedin.com/in/ricardoanderegg](http://linkedin.com/in/ricardoanderegg)

Distributed under the MIT license. See ``LICENSE`` for more information.

## Contributing

1. Fork it (<https://github.com/polyrand/nb2script/fork>)
2. Create your feature branch (`git checkout -b feature/foobar`)
3. Commit your changes (`git commit -am 'Add some foobar'`)
4. Push to the branch (`git push origin feature/foobar`)
5. Create a new Pull Request
