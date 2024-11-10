# DLTJ-PLUGIN

Utilities and macros specific to the DLTJ blog

## Installation

This plugin can be installed via:

    python -m pip install git+https://github.com/dltj/pelican-dltj-plugin

If you haven't added a PLUGINS setting to your Pelican settings file, the newly-installed plugin should be automatically detected and enabled. 
Otherwise, add zygote-reader to your existing PLUGINS list. For more information, see the [How to Use Plugins](https://docs.getpelican.com/en/latest/plugins.html#how-to-use-plugins) documentation.

## Usage

To use the macros in all content pages, add them to your pelicanconf.py file as `JINJA_GLOBALS`:

```python
# These macros are available on all content pages
JINJA_GLOBALS = {
    "image": macros.image,
    "robustlink": macros.robustlink,
    "note": macros.note,
    "thursday_threads_header": macros.thursday_threads_header,
    "thursday_threads_quote": macros.thursday_threads_quote,
    "captioned": macros.captioned,
}
```