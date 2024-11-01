# System Environment
*   **Product**: Fabric Runtime 1.3 (Spark 3.5)
*   **Vhd Release**: Spark3.5-Rel-2024-09-25.0-rc.1
*   **Operating System**: CBL-Mariner 2.0.20240829
*   **Apache Spark**: 3.5.1
*   **Java**: 11.0.24
*   **Scala**: 2.12.18
*   **Python**: 3.11/1.0.1
*   **Delta Lake**: 3.2.0.5

# New Features
|Id|Component|Description|
|-----|-----|-----|
|1458780|TokenLibrary:4.3.3, ServiceConfigurationTemplates:spark35|Enabling Reading and Writing Internal Log Files to SystemStorage account with shorter lived tokens|
|1451941|ServiceConfigurationTemplates/spark/3.5.0:various|Set the Spark property to allow special characters in table names for Spark in Fabric.|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1466640|Wildfire/spark35:1.10.10|New Spark 3.5 component release, including improvements and fixes in Hadoop, Spark and Livy including security fix.|
|1464212|ComponentName:ComponentVersion|Enhance security for library snapshot sas token by encrypting it before passing it library management scripts|
|1458213|AutoscaleProbe:3.9.3|Update to new Autoscale Version contains autoscale reliability fixes to reduce TJS and token library errors.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1466640|Wildfire/spark35:1.10.10|New Spark 3.5 component release, including improvements and fixes in Hadoop, Spark and Livy including security fix.|
|1455532|LibraryMetadataCooker:2.0.3|Fix bug that LMC would stop for empty folders|
|1455163|LibraryManager:1.0.6|Library manager bug fix for library metadata cooker timeout issue|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|**AutoscaleProbe**|**3.9.2 ⬆️ 3.9.3**|SQLServerODBCDriver|18.1.0|
|AzureMLExtensions|1.0.4|SparkAdvisor|1.0.3|
|CSparkMetricUpdate|1.0.5|SparkDiagnosticsLibrary|1.0.24|
|Conda|5.0.1|SparkLighter|2.0.4|
|DSCopilotInstaller|1.0.0|SparkNativeParquetWriter|0.21.0|
|Delta|3.2.0.5|SparkRPCHistoryServer|1.2.0|
|EventHubConnector|2.3.27|SparklyrConnector|2.0.1|
|FabricDWConnector|1.0.10|**TokenLibrary**|**4.2.2 ⬆️ 4.3.3**|
|FsspecWrapper|1.0.3|TridentCore|1.2.16|
|**Genesis**|**0.30.0 ⬆️ 0.32.1**|TridentTokenLibrary|1.9.5|
|GlutenUI|1.0.0|Vegas|3.5.09.01|
|HiveMetaStoreClient|1.1.21|**Wildfire**|**1.10.9 ⬆️ 1.10.10**|
|Impulse|1.2.4|
|KustoConnector|1.5.1|
|**LibraryManager**|**1.0.4 ⬆️ 1.0.7**|
|**LibraryMetadataCooker**|**2.0.2 ⬆️ 2.0.3**|
|MMLSpark|1.4.17|
|MlflowLibrary|2.11.3.1|
|MySQLJavaConnector|1.0.3|
|NotebookUtils|1.1.52|
|OneLakeClientStarter|1.0.23|
|OnelakeSparkCatalog|0.1.13|
|PostgreSQLJDBCDriver|1.0.3|
|Python|3.11/1.0.1|
|R|1.0.6|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_openmp_mutex|5.1|make|4.2.1|
|_py-xgboost-mutex|2.0|mako|1.3.5|
|_sysroot_linux-64_curr_repodata_hack|3|markdown|3.4.1|
|abseil-cpp|20211102.0|markdown-it-py|2.2.0|
|absl-py|2.1.0|markupsafe|2.1.3|
|accelerate|0.30.1|matplotlib|3.8.0|
|adlfs|2024.2.0|matplotlib-base|3.8.0|
|aiohttp|3.9.3|matplotlib-inline|0.1.6|
|aiosignal|1.2.0|mccabe|0.7.0|
|alabaster|0.7.12|mdurl|0.1.0|
|alembic|1.13.2|menuinst|2.0.2|
|anyio|4.2.0|minio|7.1.0|
|aom|3.6.0|mistune|2.0.4|
|appdirs|1.4.4|mkl|2023.1.0|
|archspec|0.2.3|mkl-service|2.4.0|
|argon2-cffi|21.3.0|mkl_fft|1.3.8|
|argon2-cffi-bindings|21.2.0|mkl_random|1.2.4|
|arrow|1.2.3|mlflow-skinny|2.12.2|
|arrow-cpp|14.0.2|mock|4.0.3|
|asgiref|3.5.2|more-itertools|10.1.0|
|asn1crypto|1.5.1|mpc|1.1.0|
|astor|0.8.1|mpfr|4.0.2|
|astropy|5.3.4|mpi|1.0|
|asttokens|2.0.5|mpich|4.1.1|
|async-lru|2.0.4|mpmath|1.3.0|
|async-timeout|4.0.3|msal|2023.12.01|
|async_generator|1.10|msal-extensions|2023.12.01|
|atk-1.0|2.36.0|msgpack-python|1.0.3|
|attrs|23.1.0|msrest|2023.12.01|
|autopep8|2.0.4|multidict|6.0.4|
|aws-c-auth|0.6.19|multipledispatch|0.6.0|
|aws-c-cal|0.5.20|multiprocess|0.70.15|
|aws-c-common|0.8.5|munkres|1.1.4|
|aws-c-compression|0.2.16|mypy|1.4.1|
|aws-c-event-stream|0.2.15|mypy_extensions|1.0.0|
|aws-c-http|0.6.25|mysql|5.7.24|
|aws-c-io|0.13.10|nbclassic|1.0.0|
|aws-c-mqtt|0.7.13|nbclient|0.8.0|
|aws-c-s3|0.1.51|nbconvert|7.10.0|
|aws-c-sdkutils|0.1.6|nbformat|5.9.2|
|aws-checksums|0.1.13|ncurses|6.4|
|aws-crt-cpp|0.18.16|nest-asyncio|1.6.0|
|aws-sdk-cpp|1.10.55|networkx|3.1|
|azure-core|1.30.2|ninja|1.10.2|
|azure-datalake-store|0.0.53|ninja-base|1.10.2|
|azure-identity|2023.12.01|nltk|3.8.1|
|azure-keyvault|2023.12.01|nni|3.0|
|azure-storage|2023.12.01|nose|1.3.7|
|azure-storage-blob|12.22.0|notebook|7.0.8|
|azure-storage-file-datalake|12.16.0|notebook-shim|0.2.3|
|azureml-synapse|0.0.1|notebookutils|1.1.3.35|
|babel|2.11.0|nspr|4.35|
|backports|1.1|nss|3.89.1|
|backports.shutil_get_terminal_size|1.0.0|numba|0.59.0|
|bcrypt|3.2.0|numexpr|2.8.7|
|beautifulsoup4|4.12.2|numpy|1.26.4|
|binaryornot|0.4.4|numpy-base|1.26.4|
|binutils_impl_linux-64|2.38|numpydoc|1.5.0|
|binutils_linux-64|2.38.0|nvidia-ml-py|12.560.30|
|bitarray|2.5.1|oauthlib|3.2.2|
|bkcharts|0.2|olefile|0.46|
|black|23.11.0|openjpeg|2.4.0|
|blas|1.0|openml|0.12.2|
|bleach|4.1.0|openpyxl|3.0.10|
|blinker|1.6.2|openssl|3.0.13|
|blosc|1.21.3|optuna|3.6.1|
|bokeh|3.3.4|orc|1.7.4|
|boltons|23.0.0|overrides|7.4.0|
|boost-cpp|1.82.0|packaging|23.1|
|boto|2.49.0|pandas|2.1.4|
|bottleneck|1.3.7|pandasnet|1.0|
|brotli|1.0.9|pandasql|0.7.3|
|brotli-bin|1.0.9|pandocfilters|1.5.0|
|brotli-python|1.0.9|pango|1.50.7|
|brunsli|0.1|paramiko|2.8.1|
|bzip2|1.0.8|parso|0.8.3|
|c-ares|1.19.1|partd|1.4.1|
|c-blosc2|2.12.0|patch|2.7.6|
|ca-certificates|2023.12.12|patchelf|0.17.2|
|cached-property|1.5.2|path|16.2.0|
|cairo|1.16.0|path.py|12.5.0|
|catboost|1.2.3|pathlib2|2.3.6|
|certifi|2024.2.2|pathspec|0.10.3|
|cffi|1.16.0|patsy|0.5.3|
|cfitsio|3.470|pcre2|10.42|
|chardet|4.0.0|pep8|1.7.1|
|charls|2.2.0|pexpect|4.8.0|
|charset-normalizer|2.0.4|pickleshare|0.7.5|
|click|8.1.7|pillow|10.2.0|
|cloudpickle|2.2.1|pip|23.3.1|
|clr_loader|0.2.5|pixman|0.40.0|
|cmake|3.26.4|pkginfo|1.9.6|
|cmdstan|2.33.1|platformdirs|3.10.0|
|cmdstanpy|1.1.0|plotly|5.22.0|
|colorama|0.4.6|pluggy|1.0.0|
|colorlog|6.8.2|ply|3.11|
|comm|0.2.1|poppler|22.12.0|
|conda-package-handling|2.2.0|poppler-data|0.4.11|
|conda-package-streaming|0.9.0|portalocker|2.3.0|
|configparser|5.0.2|powerbiclient|3.1.1|
|contextlib2|21.6.0|prettytable|3.5.0|
|contourpy|1.2.0|prometheus_client|0.14.1|
|convertdate|2.4.0|prompt-toolkit|3.0.43|
|cookiecutter|2.5.0|prompt_toolkit|3.0.43|
|cryptography|42.0.2|prophet|1.1.5|
|curl|8.5.0|prose-pandas2pyspark|8.35.0rc20240513101|
|cycler|0.11.0|prose-suggestions|9.0.0|
|cyrus-sasl|2.1.28|protobuf|3.20.3|
|cython|3.0.8|psutil|5.9.0|
|cytoolz|0.12.2|ptyprocess|0.7.0|
|daal4py|2023.1.1|pure_eval|0.2.2|
|dal|2023.1.1|py-cpuinfo|9.0.0|
|dash|2.17.1|py-lief|0.12.3|
|dash-core-components|2.0.0|py-xgboost|2.0.3|
|dash-cytoscape|1.0.2|py4j|0.10.9.7|
|dash-html-components|2.0.0|pyarrow|14.0.2|
|dash-table|5.0.0|pybind11-abi|4|
|dask|2023.11.0|pycodestyle|2.11.1|
|dask-core|2023.11.0|pycosat|0.6.6|
|dataclasses|0.8|pycparser|2.21|
|datasets|2.19.1|pycurl|7.45.2|
|dav1d|1.2.1|pydocstyle|6.3.0|
|dbus|1.13.18|pyerfa|2.0.0|
|debugpy|1.6.7|pyflakes|3.2.0|
|decorator|5.1.1|pygments|2.15.1|
|defusedxml|0.7.1|pyjwt|2.4.0|
|dill|0.3.8|pyluach|2.2.0|
|distlib|0.3.8|pymeeus|0.5.12|
|distributed|2023.11.0|pynacl|1.5.0|
|distro|1.8.0|pyodbc|5.0.1|
|django|4.1|pyopenssl|24.0.0|
|docker|7.0.0|pyparsing|3.0.9|
|docutils|0.18.1|pyperclip|1.8.2|
|dscopilot-installer|0.0.7|pyqt|5.15.10|
|entrypoints|0.4|pyqt5-sip|12.13.0|
|et_xmlfile|1.1.0|pyrsistent|0.20.0|
|executing|0.8.3|pysocks|1.7.1|
|expat|2.5.0|pyspark|3.5.1.5.4.20240407|
|fastcache|1.1.0|pytables|3.9.2|
|filelock|3.11.0|pytest|7.4.0|
|flake8|7.0.0|python|3.11.8|
|flaml|2.3.0.post2|python-dateutil|2.8.2|
|flask|2.2.5|python-fastjsonschema|2.16.2|
|flit|3.9.0|python-graphviz|0.20.1|
|flit-core|3.9.0|python-json-logger|2.0.7|
|fluent-logger|0.10.0|python-libarchive-c|2.9|
|fmt|9.1.0|python-lmdb|1.4.1|
|font-ttf-dejavu-sans-mono|2.37|python-slugify|5.0.2|
|font-ttf-inconsolata|2.001|python-tzdata|2023.3|
|font-ttf-source-code-pro|2.030|python-xxhash|2.0.2|
|font-ttf-ubuntu|0.83|pythonnet|3.0.1|
|fontconfig|2.14.1|pythonwebhdfs|0.2.3|
|fonts-anaconda|1|pytorch|2.2.1|
|fonts-conda-ecosystem|1|pytorch-lightning|2.0.3|
|fonttools|4.25.0|pytorch-mutex|1.0|
|freetype|2.12.1|pytz|2023.3.post1|
|fribidi|1.0.10|pywavelets|1.5.0|
|frozenlist|1.4.0|pyyaml|6.0.1|
|fsspec|2024.6.1|pyzmq|25.1.2|
|fsspec_wrapper|0.1.14|qdarkstyle|3.2.3|
|future|0.18.3|qstylizer|0.2.2|
|gcc_impl_linux-64|11.2.0|qt|5.15.9|
|gcc_linux-64|11.2.0|qt-main|5.15.2|
|gdk-pixbuf|2.42.10|qt-webengine|5.15.9|
|geographiclib|2.0|qtawesome|1.2.2|
|geopy|2.4.1|qtconsole|5.5.1|
|get_terminal_size|1.0.0|qtpy|2.4.1|
|gevent|23.9.1|re2|2022.04.01|
|gflags|2.2.2|readline|8.2|
|giflib|5.2.1|referencing|0.30.2|
|gitdb|4.0.7|regex|2023.10.3|
|gitpython|3.1.43|reproc|14.2.4|
|glib|2.78.4|reproc-cpp|14.2.4|
|glib-tools|2.78.4|requests|2.31.0|
|glob2|0.7|requests-oauthlib|1.3.0|
|glog|0.5.0|responses|0.25.3|
|gmp|6.2.1|retrying|1.3.4|
|gmpy2|2.1.2|rfc3339-validator|0.1.4|
|gobject-introspection|1.78.1|rfc3986-validator|0.1.1|
|graphite2|1.3.14|rgf-python|3.12.0|
|graphviz|2.50.0|rhash|1.4.3|
|greenlet|3.0.1|rich|13.3.5|
|grpc-cpp|1.48.2|ripgrep|13.0.0|
|gson|0.0.4|rouge-score|0.1.2|
|gst-plugins-base|1.14.1|rpds-py|0.10.6|
|gstreamer|1.14.1|rtree|1.0.1|
|gtk2|2.24.33|ruamel.yaml|0.17.21|
|gts|0.7.6|ruamel.yaml.clib|0.2.7|
|gxx_impl_linux-64|11.2.0|ruamel_yaml|0.17.21|
|gxx_linux-64|11.2.0|s2n|1.3.27|
|harfbuzz|4.3.0|safetensors|0.4.2|
|hcrystalball|0.1.10|salib|1.5.0|
|hdf5|1.12.1|schema|0.7.7|
|heapdict|1.0.1|scikit-build|0.15.0|
|holidays|0.48|scikit-image|0.22.0|
|html5lib|1.1|scikit-learn|1.2.2|
|huggingface_hub|0.23.1|scikit-learn-intelex|2023.1.1|
|icu|73.1|scipy|1.11.4|
|idna|3.4|seaborn|0.12.2|
|imagecodecs|2023.1.23|secretstorage|3.3.1|
|imageio|2.33.1|semantic-link-sempy|0.7.7|
|imagesize|1.4.1|send2trash|1.8.2|
|importlib-metadata|7.0.1|seqeval|1.2.2|
|importlib_metadata|7.0.1|setuptools|68.2.2|
|importlib_resources|6.4.0|shap|0.42.1|
|impulse-python-handler|1.0.22.1.0.0|simplegeneric|0.8.1|
|inflection|0.5.1|simplejson|3.19.3|
|iniconfig|1.1.1|singledispatch|3.7.0|
|intel-openmp|2023.1.0|sip|6.7.12|
|interpret|0.6.0|six|1.16.0|
|interpret-core|0.6.0|slicer|0.0.7|
|intervaltree|3.1.0|smmap|4.0.0|
|ipykernel|6.28.0|snappy|1.1.10|
|ipython|8.20.0|sniffio|1.3.0|
|ipython_genutils|0.2.0|snowballstemmer|2.2.0|
|ipywidgets|8.1.2|sortedcollections|2.1.0|
|isodate|0.6.1|sortedcontainers|2.4.0|
|itsdangerous|2.0.1|soupsieve|2.5|
|jaraco.classes|3.2.1|sphinx|5.0.2|
|jedi|0.18.1|sphinxcontrib|1.0|
|jeepney|0.7.1|sphinxcontrib-applehelp|1.0.2|
|jinja2|3.1.3|sphinxcontrib-devhelp|1.0.2|
|joblib|1.2.0|sphinxcontrib-htmlhelp|2.0.0|
|joblibspark|0.5.2|sphinxcontrib-jsmath|1.0.1|
|jpeg|9e|sphinxcontrib-qthelp|1.0.3|
|json-tricks|3.17.3|sphinxcontrib-serializinghtml|1.1.5|
|json5|0.9.6|sphinxcontrib-websupport|1.2.4|
|jsonpatch|1.32|sqlalchemy|2.0.25|
|jsonpointer|2.1|sqlanalyticsfabricconnectorpy|1.0.0|
|jsonschema|4.19.2|sqlite|3.41.2|
|jsonschema-specifications|2023.7.1|sqlparse|0.4.4|
|jupyter-lsp|2.2.0|stack_data|0.2.0|
|jupyter-ui-poll|1.0.0|statsmodels|0.14.0|
|jupyter_client|8.6.0|sympy|1.12|
|jupyter_console|6.6.3|synapseml-cognitive|1.0.4.dev1|
|jupyter_core|5.5.0|synapseml-core|1.0.4.dev1|
|jupyter_events|0.8.0|synapseml-deep-learning|1.0.4.dev1|
|jupyter_server|2.10.0|synapseml-internal|1.0.4.0.dev1|
|jupyter_server_terminals|0.4.4|synapseml-lightgbm|1.0.4.dev1|
|jupyterlab|4.0.11|synapseml-mlflow|1.0.26|
|jupyterlab_pygments|0.1.2|synapseml-opencv|1.0.4.dev1|
|jupyterlab_server|2.25.1|synapseml-utils|1.0.22.post1|
|jupyterlab_widgets|3.0.10|synapseml-vw|1.0.4.dev1|
|jxrlib|1.1|sysroot_linux-64|2.17|
|kernel-headers_linux-64|3.10.0|tbb|2021.8.0|
|keyring|24.3.1|tbb-devel|2021.8.0|
|kiwisolver|1.4.4|tbb4py|2021.8.0|
|kqlmagiccustom|0.1.114.post25|tblib|1.7.0|
|krb5|1.20.1|tenacity|8.2.3|
|lazy-object-proxy|1.6.0|tensorboardx|2.6.2.2|
|lazy_loader|0.3|terminado|0.17.1|
|lcms2|2.12|testpath|0.6.0|
|ld_impl_linux-64|2.38|text-unidecode|1.3|
|lerc|3.0|textdistance|4.2.1|
|liac-arff|2.5.0|thop|0.1.1-2209072238|
|libaec|1.0.4|threadpoolctl|2.2.0|
|libarchive|3.6.2|tifffile|2023.4.12|
|libavif|0.11.1|tinycss2|1.2.1|
|libboost|1.82.0|tk|8.6.12|
|libbrotlicommon|1.0.9|tokenizers|0.15.1|
|libbrotlidec|1.0.9|toml|0.10.2|
|libbrotlienc|1.0.9|tomli|2.0.1|
|libclang|14.0.6|tomli-w|1.0.0|
|libclang13|14.0.6|toolz|0.12.0|
|libcups|2.4.2|torchdata|0.7.1|
|libcurl|8.5.0|torchmetrics|1.4.0.post0|
|libdeflate|1.17|tornado|6.3.3|
|libedit|3.1.20230828|tqdm|4.65.0|
|libev|4.33|traitlets|5.7.1|
|libevent|2.1.12|transformers|4.37.2|
|libffi|3.4.4|truststore|0.8.0|
|libgcc-devel_linux-64|11.2.0|typed-ast|1.5.5|
|libgcc-ng|11.2.0|typeguard|4.1.2|
|libgd|2.3.3|typing-extensions|4.9.0|
|libgfortran-ng|11.2.0|typing_extensions|4.9.0|
|libgfortran5|11.2.0|tzdata|2024a|
|libglib|2.78.4|ujson|5.4.0|
|libgomp|11.2.0|unicodecsv|0.14.1|
|libiconv|1.16|unidecode|1.2.0|
|liblief|0.12.3|unixodbc|2.3.11|
|libllvm14|14.0.6|urllib3|2.1.0|
|libmamba|1.5.6|utf8proc|2.6.1|
|libmambapy|1.5.6|virtualenv|20.26.1|
|libnghttp2|1.57.0|wcwidth|0.2.5|
|libpng|1.6.39|webencodings|0.5.1|
|libpq|12.17|websocket-client|0.58.0|
|libprotobuf|3.20.3|websockets|12.0|
|**library-metadata-cooker**|**3.5.0.0 ⬆️ 3.5.0.1**|werkzeug|2.3.8|
|librsvg|2.54.4|wheel|0.41.2|
|libsodium|1.0.18|whichcraft|0.6.1|
|libsolv|0.7.24|widgetsnbextension|4.0.10|
|libspatialindex|1.9.3|workalendar|17.0.0|
|libssh2|1.10.0|wrapt|1.14.1|
|libstdcxx-devel_linux-64|11.2.0|xgboost|2.0.3|
|libstdcxx-ng|11.2.0|xlrd|2.0.1|
|libthrift|0.15.0|xlsxwriter|3.1.1|
|libtiff|4.5.1|xlwt|1.3.0|
|libtool|2.4.6|xmltodict|0.13.0|
|libuuid|1.41.5|xxhash|0.8.0|
|libuv|1.44.2|xyzservices|2022.9.0|
|libwebp|1.3.2|xz|5.4.6|
|libwebp-base|1.3.2|yaml|0.2.5|
|libxcb|1.15|yaml-cpp|0.8.0|
|libxgboost|2.0.3|yapf|0.40.2|
|libxkbcommon|1.0.1|yarl|1.9.3|
|libxml2|2.10.4|zeromq|4.3.5|
|libxslt|1.1.37|zfp|1.0.0|
|libzopfli|1.0.3|zict|3.0.0|
|lightgbm|4.3.0|zipp|3.17.0|
|lightning-utilities|0.9.0|zlib|1.2.13|
|llvm-openmp|14.0.6|zlib-ng|2.0.7|
|llvmlite|0.42.0|zope|1.0|
|locket|1.0.0|zope.event|5.0|
|lunardate|0.2.2|zope.interface|5.4.0|
|lxml|4.9.3|zstandard|0.19.0|
|lz4|4.3.2|zstd|1.5.5|
|lz4-c|1.9.4|_libgcc_mutex|0.1|
|lzo|2.10|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|jta|1.1|
|JLargeArrays|1.5|jul-to-slf4j|2.0.7|
|JTransforms|3.1|junit-jupiter|5.5.2|
|RoaringBitmap|0.9.45|junit-jupiter-api|5.5.2|
|ST4|4.0.4|junit-jupiter-engine|5.5.2|
|SparkCustomEvents|3.5.0-1.0.5|junit-jupiter-params|5.5.2|
|**TokenLibrary-assembly**|**4.2.2 ⬆️ 4.3.3**|junit-platform-commons|1.5.2|
|VegasConnector|3.5.09|junit-platform-engine|1.5.2|
|activation|1.1.1|kafka-clients|3.4.1|
|aircompressor|0.26|kryo-shaded|4.0.2|
|algebra|2.12-2.0.1|kusto-spark|3.0_2.12-5.2.2-SNAPSHOT|
|aliyun-java-sdk-core|4.5.10|lapack|3.0.3|
|aliyun-java-sdk-kms|2.11.0|leveldbjni-all|1.8|
|aliyun-java-sdk-ram|3.1.0|libfb303|0.9.3|
|aliyun-sdk-oss|3.13.0|libthrift|0.12.0|
|annotations|7.0.0|lightgbmlib|3.3.510|
|antlr-runtime|3.5.2|log4j|1.2-api-2.20.0|
|antlr4-runtime|4.9.3|log4j-api|2.20.0|
|aopalliance-repackaged|2.6.1|log4j-core|2.20.0|
|apiguardian-api|1.1.0|log4j-slf4j2-impl|2.20.0|
|arpack|3.0.3|lz4-java|1.8.0|
|arpack_combined_all|0.1|mdsdclientdynamic|2.0|
|arrow-format|2.0.1|metrics-core|4.2.19|
|arrow-memory-core|2.0.1|metrics-graphite|4.2.19|
|arrow-memory-netty|2.0.1|metrics-jmx|4.2.19|
|arrow-vector|2.0.1|metrics-json|4.2.19|
|audience-annotations|0.5.0|metrics-jvm|4.2.19|
|avro|1.11.3|microsoft-catalog-metastore-client|1.1.21|
|avro-ipc|1.11.3|microsoft-log4j-etwappender|1.0|
|avro-mapred|1.11.3|minlog|1.3.0|
|aws-java-sdk-bundle|1.12.262|mlflow-spark|2.12-2.11.3|
|azure-core|1.47.0|mysql-connector-java|8.0.18|
|azure-core-http-netty|1.14.1|netty-all|4.1.96.Final|
|azure-data-lake-store-sdk|2.3.9|netty-buffer|4.1.96.Final|
|azure-eventhubs|3.3.0|netty-codec|4.1.96.Final|
|azure-eventhubs-spark|2.12-2.3.22|netty-codec-dns|4.1.101.Final|
|azure-json|1.1.0|netty-codec-http|4.1.96.Final|
|azure-keyvault-core|1.0.0|netty-codec-http2|4.1.96.Final|
|azure-storage|7.0.1|netty-codec-socks|4.1.96.Final|
|azure-storage-blob|2.25.3|netty-common|4.1.96.Final|
|azure-storage-common|2.24.3|netty-handler|4.1.96.Final|
|azure-storage-internal-avro|2.10.3|netty-handler-proxy|4.1.96.Final|
|azure-synapse-ml-pandas|2.12-0.1.1|netty-resolver|4.1.96.Final|
|blas|3.0.3|netty-resolver-dns|4.1.101.Final|
|bonecp|0.8.0.RELEASE|netty-resolver-dns-classes-macos|4.1.101.Final|
|breeze|2.12-2.1.0|netty-resolver-dns-native-macos|4.1.101.Final-osx-x86_64|
|breeze-macros|2.12-2.1.0|netty-tcnative-boringssl-static|2.0.62.Final-windows-x86_64|
|cats-kernel|2.12-2.1.1|netty-tcnative-boringssl-static|2.0.62.Final-osx-x86_64|
|chill|2.12-0.10.0|netty-tcnative-boringssl-static|2.0.62.Final-osx-aarch_64|
|chill-java|0.10.0|netty-tcnative-boringssl-static|2.0.62.Final-linux-x86_64|
|client-sdk|1.24.1|netty-tcnative-boringssl-static|2.0.62.Final-linux-aarch_64|
|commons-cli|1.5.0|netty-tcnative-boringssl-static|2.0.62.Final|
|commons-codec|1.16.0|netty-tcnative-classes|2.0.62.Final|
|commons-collections|3.2.2|netty-transport|4.1.96.Final|
|commons-collections4|4.4|netty-transport-classes-epoll|4.1.96.Final|
|commons-compiler|3.1.9|netty-transport-classes-kqueue|4.1.96.Final|
|commons-compress|1.23.0|netty-transport-native-epoll|4.1.96.Final-linux-aarch_64|
|commons-crypto|1.1.0|netty-transport-native-epoll|4.1.96.Final-linux-x86_64|
|commons-dbcp|1.4|netty-transport-native-kqueue|4.1.96.Final-osx-aarch_64|
|commons-io|2.11.0|netty-transport-native-kqueue|4.1.96.Final-osx-x86_64|
|commons-io|2.13.0|netty-transport-native-unix-common|4.1.96.Final|
|commons-lang|2.6|notebook-utils|1.1.3-spark35|
|commons-lang3|3.12.0|objenesis|3.3|
|commons-logging|1.1.3|onnx-protobuf|2.12-0.9.3|
|commons-math3|3.6.1|onnxruntime_gpu|1.8.1|
|commons-pool|1.5.4|opencsv|2.3|
|commons-pool2|2.11.1|opencv|3.2.0-1|
|commons-text|1.10.0|opentest4j|1.2.0|
|compress-lzf|1.1.2|opentracing-api|0.33.0|
|curator-client|2.13.0|opentracing-noop|0.33.0|
|curator-framework|2.13.0|opentracing-util|0.33.0|
|curator-recipes|2.13.0|orc-core|1.9.2-shaded-protobuf|
|datanucleus-api-jdo|4.2.4|orc-mapreduce|1.9.2-shaded-protobuf|
|datanucleus-core|4.1.17|orc-shims|1.9.2|
|datanucleus-rdbms|4.1.19|oro|2.0.8|
|datasketches-java|3.3.0|osgi-resource-locator|1.0.3|
|datasketches-memory|2.1.0|paranamer|2.8|
|delta-spark|2.12-3.2.0.5|parquet-column|1.13.1|
|delta-storage|3.2.0.5|parquet-common|1.13.1|
|derby|0.14.2.0|parquet-encoding|1.13.1|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|parquet-format-structures|1.13.1|
|flatbuffers-java|1.12.0|**parquet-hadoop-ms**|**3.5.1.5.4.20240830.3 ⬆️ 3.5.1.5.4.20240924.1**|
|fluent-logger|0.3.4-jar-with-dependencies-provided|parquet-jackson|1.13.1|
|gcs-connector-hadoop3|2.2.14-shaded|pickle|1.3|
|**genesis-client**|**2.12-0.28.0-jar-with-dependencies ⬆️ 2.12-0.32.1-jar-with-dependencies**|postgresql|2.2.9|
|gson|2.8.9|proton-j|0.33.8|
|guava|4.0.1|py4j|0.10.9.7|
|**hadoop-aliyun**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|qpid-proton-j-extensions|1.2.4|
|**hadoop-annotations**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|reactive-streams|1.0.3|
|**hadoop-aws**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|reactor-core|3.4.34|
|**hadoop-azure**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|reactor-netty-core|1.0.40|
|**hadoop-azure-datalake**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|reactor-netty-http|1.0.40|
|hadoop-azureml|1.0-fs|rocksdbjni|8.3.2|
|**hadoop-client-api**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|scala-collection-compat|2.12-2.7.0|
|**hadoop-client-runtime**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|scala-compiler|2.12.18|
|**hadoop-cloud-storage**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|scala-java8-compat|2.12-0.9.0|
|**hadoop-openstack**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|scala-library|2.12.18|
|hadoop-shaded-guava|1.1.1|scala-parser-combinators|2.12-2.3.0|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.4.20240830.3 ⬆️ 3.3.4.5.4.20240924.1**|scala-reflect|2.12.18|
|hdinsight-spark-metrics|3.5.0-1.0.5|scala-xml|2.12-2.1.0|
|hive-common|2.3.9|scalactic|2.12-3.2.14|
|hive-exec|2.3.9-core|shims|0.9.45|
|hive-llap-common|2.3.9|slf4j-api|2.0.7|
|hive-metastore|2.3.9|snappy-java|1.1.10.5|
|hive-serde|2.3.9|spark|3.5-rpc-history-server-app-listener_2.12-1.0.0|
|hive-shims|2.3.9|spark|3.5-rpc-history-server-core_2.12-1.0.0|
|hive-shims|0.23-2.3.9|spark|3.5-advisor-core_2.12-1.0.18|
|hive-shims-common|2.3.9|spark-avro|2.12-3.5.0|
|hive-shims-scheduler|2.3.9|**spark-avro**|**2.12-3.5.0 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|hive-storage-api|2.8.1|**spark-catalyst**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|hk2-api|2.6.1|**spark-common-utils**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|hk2-locator|2.6.1|**spark-core**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|hk2-utils|2.6.1|**spark-enhancement**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|httpclient|4.5.14|spark-enhancementui|2.12-3.3.0|
|httpclient5|5.1.3|**spark-graphx**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|httpcore|4.4.16|**spark-hadoop-cloud**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|httpmime|4.5.13|**spark-hive**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|httpmime|4.5.14|spark-kusto-synapse-connector|3.5_2.12-1.5.1|
|impulse-core_spark|3.5_2.12-1.0.22|**spark-kvstore**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|impulse-telemetry-mds_spark|3.5_2.12-1.0.22|**spark-launcher**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|ini4j|0.5.4|spark-lighter-contract|2.12-2.1.0_spark-3.5.1_20240717.4|
|isolation-forest|3.5.0_2.12-3.0.5|spark-lighter-core|2.12-2.0.11_spark-3.5.1_20240717.4|
|istack-commons-runtime|3.0.8|**spark-microsoft-tools**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|ivy|2.5.1|**spark-mllib**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-annotations|2.15.2|**spark-mllib-local**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-core|2.15.2|**spark-network-common**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-core-asl|1.9.13|**spark-network-shuffle**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-databind|2.15.2|**spark-repl**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-dataformat-cbor|2.15.2|**spark-sketch**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-dataformat-xml|2.12.7|**spark-sql**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-datatype-jsr310|2.15.2|**spark-sql-api**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-mapper-asl|1.9.13|**spark-sql-kafka**|**0_2.12-3.5.1.5.4.20240830.3 ⬆️ 0_2.12-3.5.1.5.4.20240924.1**|
|jackson-module-jaxb-annotations|2.15.2|**spark-streaming**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jackson-module-scala|2.12-2.15.2|**spark-streaming-kafka**|**0_2.12-3.5.1.5.4.20240830.3 ⬆️ 0_2.12-3.5.1.5.4.20240924.1**|
|jakarta.activation-api|1.2.2|**spark-streaming-kafka**|**0_2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jakarta.annotation-api|1.3.5|**spark-tags**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jakarta.inject|2.6.1|**spark-token-provider-kafka**|**0_2.12-3.5.1.5.4.20240830.3 ⬆️ 0_2.12-3.5.1.5.4.20240924.1**|
|jakarta.servlet-api|4.0.3|**spark-unsafe**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jakarta.validation-api|2.0.2|**spark-yarn**|**2.12-3.5.1.5.4.20240830.3 ⬆️ 2.12-3.5.1.5.4.20240924.1**|
|jakarta.ws.rs-api|2.1.6|spark_diagnostic_cli|2.1.1_spark-3.5.1_20240801.2|
|jakarta.xml.bind-api|2.3.2|sparklyr-connector|3.5.1-1.0.0267535|
|janino|3.1.9|sparknativeparquetwriter|2.12-0.21.0|
|javassist|3.29.2-GA|spire|2.12-0.17.0|
|javatuples|1.2|spire-macros|2.12-0.17.0|
|javax.jdo|3.2.0-m3|spire-platform|2.12-0.17.0|
|javolution|5.5.1|spire-util|2.12-0.17.0|
|jaxb-api|2.2.11|spray-json|2.12-1.3.5|
|jaxb-runtime|2.3.2|stax-api|1.0.1|
|jcl-over-slf4j|2.0.7|stax2-api|4.2.1|
|jdo-api|3.0.1|stream|2.9.6|
|jdom2|2.0.6|synapseml-cognitive|2.12-1.0.4-spark3.5|
|jersey-client|2.40|synapseml-core|2.12-1.0.4-spark3.5|
|jersey-common|2.40|synapseml-deep-learning|2.12-1.0.4-spark3.5|
|jersey-container-servlet|2.40|synapseml-internal|2.12-1.0.4.0-spark3.5|
|jersey-container-servlet-core|2.40|synapseml-lightgbm|2.12-1.0.4-spark3.5|
|jersey-hk2|2.40|synapseml-opencv|2.12-1.0.4-spark3.5|
|jersey-server|2.40|synapseml-vw|2.12-1.0.4-spark3.5|
|jettison|1.1|synfs|1.1.3-spark35|
|jetty-util|9.4.53.v20231009|threeten-extra|1.7.1|
|jetty-util-ajax|9.4.53.v20231009|tink|1.9.0|
|jline|2.14.6|transaction-api|1.1|
|joda-time|2.12.5|trident-core|1.2.16|
|jodd-core|3.5.2|tridenttokenlibrary-assembly|1.9.5|
|jsch|0.1.54|univocity-parsers|2.9.1|
|json|1.8|vw-jni|9.3.0|
|json|3|wildfly-openssl|1.0.7.Final|
|json-simple|1.1.1|woodstox-core|6.2.4|
|json-simple|1.1|xbean-asm9-shaded|4.23|
|json4s-ast|2.12-3.7.0-M11|xz|1.9|
|json4s-core|2.12-3.7.0-M11|**zookeeper**|**3.6.3.5.4.20240830.3 ⬆️ 3.6.3.5.4.20240924.1**|
|json4s-jackson|2.12-3.7.0-M11|**zookeeper-jute**|**3.6.3.5.4.20240830.3 ⬆️ 3.6.3.5.4.20240924.1**|
|json4s-scalap|2.12-3.7.0-M11|zstd-jni|1.5.5-4|
|jsr305|3.0.0|

# R Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|DBI|1.2.3|lightgbm|4.5.0|
|DiceDesign|1.10|listenv|0.9.1|
|FabricTelemetry|1.0.2|lobstr|1.1.2|
|GPfit|1.0-8|lubridate|1.9.3|
|KernSmooth|2.23-24|magrittr|2.0.3|
|MASS|7.3-60.0.1|maps|3.4.2|
|Matrix|1.6-5|markdown|1.13|
|ModelMetrics|1.2.2.2|memoise|2.0.1|
|R.methodsS3|1.8.2|methods|4.4.1|
|R.oo|1.26.0|mgcv|1.9-1|
|R.utils|2.12.3|mime|0.12|
|R6|2.5.1|miniUI|0.1.1.1|
|R6P|0.3.0|modeldata|1.4.0|
|RColorBrewer|1.1-3|modelenv|0.1.1|
|RODBC|1.3-23|modelr|0.1.11|
|Rcpp|1.0.13|munsell|0.5.1|
|SQUAREM|2021.1|nlme|3.1-165|
|TTR|0.24.4|nnet|7.3-19|
|V8|5.0.0|notebookutils|1.1.3.35|
|XML|3.99-0.17|numDeriv|2016.8-1.1|
|arrow|17.0.0|openssl|2.2.1|
|askpass|1.2.0|pROC|1.18.5|
|assertthat|0.2.1|parallel|4.4.1|
|backports|1.5.0|parallelly|1.38.0|
|base|4.4.1|parsnip|1.2.1|
|base64enc|0.1-3|patchwork|1.2.0|
|bigD|0.2.0|pillar|1.9.0|
|bit|4.0.5|pkgbuild|1.4.4|
|bit64|4.0.5|pkgconfig|2.0.3|
|bitops|1.0-8|pkgdown|2.1.0|
|blob|1.2.4|pkgload|1.4.0|
|brew|1.0-10|plotly|4.10.4|
|brio|1.1.5|plyr|1.8.9|
|broom|1.0.6|praise|1.0.0|
|bslib|0.8.0|prettyunits|1.2.0|
|cachem|1.1.0|processx|3.8.4|
|callr|3.7.6|prodlim|2024.06.25|
|cards|0.2.1|profvis|0.3.8|
|caret|6.0-94|progress|1.2.3|
|cellranger|1.1.0|progressr|0.14.0|
|class|7.3-22|promises|1.3.0|
|classInt|0.4-10|proxy|0.4-27|
|cli|3.6.3|pryr|0.1.6|
|clipr|0.8.0|ps|1.7.7|
|clock|0.7.1|purrr|1.0.2|
|codetools|0.2-20|quantmod|0.4.26|
|collections|0.3.7|ragg|1.3.2|
|colorspace|2.1-1|rappdirs|0.3.3|
|commonmark|1.9.1|rbokeh|0.5.2|
|compiler|4.4.1|rcmdcheck|1.4.0|
|config|0.3.2|reactR|0.6.0|
|conflicted|1.2.0|reactable|0.4.4|
|coro|1.0.4|readr|2.1.5|
|cpp11|0.4.7|readxl|1.4.3|
|crayon|1.5.3|recipes|1.1.0|
|credentials|2.0.1|rematch|2.0.0|
|crosstalk|1.2.1|rematch2|2.1.2|
|crul|1.5.0|remotes|2.5.0|
|curl|5.2.1|reprex|2.1.1|
|data.table|1.15.4|reshape2|1.4.4|
|datasets|4.4.1|rjson|0.2.21|
|dbplyr|2.5.0|rlang|1.1.4|
|desc|1.4.3|rlist|0.4.6.2|
|devtools|2.4.5|rmarkdown|2.27|
|diagram|1.6.5|roxygen2|7.3.2|
|dials|1.3.0|rpart|4.1.23|
|diffobj|0.3.5|rprojroot|2.0.4|
|digest|0.6.36|rsample|1.2.1|
|doFuture|1.0.1|rstudioapi|0.16.0|
|downlit|0.4.4|rversions|2.1.2|
|dplyr|1.1.4|rvest|1.0.4|
|dtplyr|1.3.1|s2|1.1.7|
|e1071|1.7-14|safetensors|0.1.2|
|ellipsis|0.3.2|sass|0.4.9|
|evaluate|0.24.0|scales|1.3.0|
|fansi|1.0.6|selectr|0.4-2|
|farver|2.1.2|sessioninfo|1.2.2|
|fastmap|1.2.0|sf|1.0-16|
|fontawesome|0.5.2|sfd|0.1.0|
|forcats|1.0.0|shape|1.4.6.1|
|foreach|1.5.2|shiny|1.9.1|
|fs|1.6.4|slider|0.3.1|
|furrr|0.3.1|sourcetools|0.1.7-1|
|future|1.34.0|sparklyr|1.8.6|
|future.apply|1.11.2|splines|4.4.1|
|gargle|1.5.2|stats|4.4.1|
|generics|0.1.3|stats4|4.4.1|
|gert|2.1.1|stringi|1.8.4|
|ggplot2|3.5.1|stringr|1.5.1|
|gh|1.4.1|survival|3.7-0|
|gistr|0.9.0|sys|3.4.2|
|gitcreds|0.1.2|systemfonts|1.1.0|
|globals|0.16.3|tcltk|4.4.1|
|glue|1.7.0|testthat|3.2.1.1|
|googledrive|2.1.1|textshaping|0.4.0|
|googlesheets4|1.1.1|tibble|3.2.1|
|gower|1.0.1|tidymodels|1.2.0|
|grDevices|4.4.1|tidyr|1.3.1|
|graphics|4.4.1|tidyselect|1.2.1|
|grid|4.4.1|tidyverse|2.0.0|
|gsl|2.1-8|timeDate|4032.109|
|gt|0.11.0|timechange|0.3.0|
|gtable|0.3.5|tinytex|0.52|
|gtsummary|2.0.0|tools|4.4.1|
|hardhat|1.4.0|torch|0.13.0|
|haven|2.5.4|triebeard|0.4.1|
|hexbin|1.28.3|tune|1.2.1|
|highcharter|0.9.4|tzdb|0.4.0|
|highr|0.11|units|0.8-5|
|hms|1.1.3|urlchecker|1.0.1|
|htmltools|0.5.8.1|urltools|1.7.3|
|htmlwidgets|1.6.4|usethis|3.0.0|
|httpcode|0.3.0|utf8|1.2.4|
|httpuv|1.6.15|utils|4.4.1|
|httr|1.4.7|uuid|1.2-1|
|httr2|1.0.2|vctrs|0.6.5|
|ids|1.0.1|viridisLite|0.4.2|
|igraph|2.0.3|vroom|1.6.5|
|infer|1.0.7|waldo|0.5.2|
|ini|0.3.1|warp|0.2.1|
|ipred|0.9-15|whisker|0.4.1|
|isoband|0.2.7|withr|3.0.1|
|iterators|1.0.14|wk|0.9.2|
|jose|1.2.0|workflows|1.1.4|
|jquerylib|0.1.4|workflowsets|1.1.0|
|jsonlite|1.8.8|xfun|0.47|
|juicyjuice|0.1.0|xgboost|1.7.8.1|
|knitr|1.48|xml2|1.3.6|
|labeling|0.4.3|xopen|1.0.1|
|later|1.3.2|xtable|1.8-4|
|lattice|0.22-6|xts|0.14.0|
|lava|1.7.3|yaml|2.3.10|
|lazyeval|0.2.2|yardstick|1.3.1|
|lhs|1.2.0|zip|2.3.1|
|lifecycle|1.0.4|zoo|1.8-12|

