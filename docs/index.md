# Welcome to DocArray!

```{include} ../README.md
:start-after: <!-- start elevator-pitch -->
:end-before: <!-- end elevator-pitch -->
```

## Install

The latest version of DocArray is {{ env.config.version }}.

Make sure you have Python 3.7+ and `numpy` installed on Linux/Mac/Windows:

````{tab} Basic install

```bash
pip install docarray
```

No extra dependency will be installed.
````

````{tab} Full install

```bash
pip install "docarray[full]"
```

The following dependencies will be installed to enable additional features:

| Package | Used in |
|---|---|
| `protobuf` | advanced serialization |
| `lz4` | compression in seralization |
| `requests` | push/pull to Jina Cloud |
| `matplotlib` | visualizing image sprites |
| `Pillow` | image data-related IO |
| `rich` | push/pull to Jina Cloud, summary of Document, DocumentArray |
| `av` | video data-related IO |
| `trimesh`| 3D mesh data-related IO |
| `fastapi`| used in embedding projector of DocumentArray|

Alternatively, you can first do basic installation and then install missing dependencies on-demand. 
````

```pycon
>>> import docarray
>>> docarray.__version__
'0.1.0'
>>> from docarray import Document, DocumentArray
```


```{important}
Jina 3.x users do not need to install `docarray` separately, as it is shipped with Jina. To check your Jina version, type `jina -vf` in the console.

However, if the printed version is smaller than `0.1.0`, say `0.0.x`, then you are 
not installing `docarray` correctly. You are probably still using an old `docarray` shipped with Jina 2.x. 
```




```{include} ../README.md
:start-after: <!-- start support-pitch -->
:end-before: <!-- end support-pitch -->
```

```{toctree}
:caption: Get Started
:hidden:

get-started/what-is
```

```{toctree}
:caption: User Guides
:hidden:

fundamentals/document/index
fundamentals/documentarray/index
datatypes/index
```



```{toctree}
:caption: Developer References
:hidden:
:maxdepth: 1

api/docarray
proto/index
```


---
{ref}`genindex` | {ref}`modindex`

