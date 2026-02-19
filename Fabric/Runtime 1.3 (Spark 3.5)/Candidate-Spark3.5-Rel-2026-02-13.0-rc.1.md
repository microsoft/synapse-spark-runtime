# System Environment
*   **Product**: Fabric Runtime 1.3 (Spark 3.5)
*   **VHD Name**: 9a1208258cd4d7.vhd
*   **Vhd Release**: Spark3.5-Rel-2026-02-13.0-rc.1
*   **Operating System**: CBL-Mariner 2.0.20260203
*   **Apache Spark**: 3.5.5
*   **Java**: 11.0.27
*   **Scala**: 2.12.18
*   **Python**: 3.11/1.0.2
*   **Delta Lake**: 3.2.1.20260209.3

# New Features
|Id|Component|Description|
|-----|-----|-----|
|1955919|Wildfire/spark35:1.10.48.1|Introduces Spark 3.5 release with updates to wildfire-spark, including re-enabling NEE support for OneSecurity RLS and improved polling with exponential backoff.|
|1950924|OnelakeSparkCatalog:0.4.4, TridentCore:1.3.2, FLTSparkExtensions:0.16.0, Wildfire/spark35:1.10.46.2|Introduces temporary UDF support for schema-enabled lakehouses and unattached sessions. Enhances FLT reliability, error handling, constraint capabilities, and view definition support with partial namespaces for CI/CD and Notebook experiences.|
|1951126|NotebookUtils:1.1.63|Released NotebookUtils 1.1.13 with new features, bug fixes, and improvements including the Business Events API, Lightweight Environment support, concurrent notebook execution optimizations, and enhanced file handling logic.|
|1934945|FLTSparkExtensions:0.14.0|Updates FLT-SparkExtensions to version 0.14.0, including improvements for IR, enhancements for PySpark MLVs, and bug fixes.|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1955919|Wildfire/spark35:1.10.48.1|Introduces Spark 3.5 release with updates to wildfire-spark, including re-enabling NEE support for OneSecurity RLS and improved polling with exponential backoff.|
|1950375|MMLSpark:1.4.29|Updated the SynapseML distributed machine learning framework libraries shipped as part of Fabric VHD component. https://github.com/microsoft/SynapseML/releases/tag/v1.1.1|
|1951126|NotebookUtils:1.1.63|Released NotebookUtils 1.1.13 with new features, bug fixes, and improvements including the Business Events API, Lightweight Environment support, concurrent notebook execution optimizations, and enhanced file handling logic.|
|1936883|conda:5.2.22, AzureMLExtensions:4.3.9, Delta:3.2.1.20251125.5.1, FsspecWrapper:1.0.7, Impulse:1.3.198470504.1, LibraryMetadataCooker:2.0.5, MMLSpark:1.4.28, MachineLearningPredict:1.0.1, NotebookUtils:1.1.62, Python:3.11/1.0.2, TokenLibrary:4.3.9|Updates FLAML to 2.5.0.post1 in Spark 3.5, improving AutoML experiences and addressing bug fixes. Removes unsupported Synapse Python environments.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1950924|OnelakeSparkCatalog:0.4.4, TridentCore:1.3.2, FLTSparkExtensions:0.16.0, Wildfire/spark35:1.10.46.2|Introduces temporary UDF support for schema-enabled lakehouses and unattached sessions. Enhances FLT reliability, error handling, constraint capabilities, and view definition support with partial namespaces for CI/CD and Notebook experiences.|
|1951126|NotebookUtils:1.1.63|Released NotebookUtils 1.1.13 with new features, bug fixes, and improvements including the Business Events API, Lightweight Environment support, concurrent notebook execution optimizations, and enhanced file handling logic.|
|1953192|Delta:3.2.1.20260209.3|Updates Delta to 3.2.1.20260209.3, addressing auto-conflict handling logic in Optimize for DVs and resolving scan failures with DV-enabled Delta tables through Data Source V2 write paths.|
|1944199|Genesis:0.36.3|Updates Genesis to version 0.36.3 with bug fixes for the CLP hydration flow in Spark 3.5, addressing configuration issues and improving library installation reliability.|
|1934945|FLTSparkExtensions:0.14.0|Updates FLT-SparkExtensions to version 0.14.0, including improvements for IR, enhancements for PySpark MLVs, and bug fixes.|
|1936883|conda:5.2.22, AzureMLExtensions:4.3.9, Delta:3.2.1.20251125.5.1, FsspecWrapper:1.0.7, Impulse:1.3.198470504.1, LibraryMetadataCooker:2.0.5, MMLSpark:1.4.28, MachineLearningPredict:1.0.1, NotebookUtils:1.1.62, Python:3.11/1.0.2, TokenLibrary:4.3.9|Updates FLAML to 2.5.0.post1 in Spark 3.5, improving AutoML experiences and addressing bug fixes. Removes unsupported Synapse Python environments.|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|Auditd|0.0.2|**NotebookUtils**|**1.1.61 ⬆️ 1.1.63**|
|AutoscaleProbe|3.9.9|OneLakeClientStarter|1.0.26.2|
|**AzureMLExtensions**|**1.0.4 ⬆️ 1.0.5**|**OnelakeSparkCatalog**|**0.4.2 ⬆️ 0.4.4**|
|**Conda**|**5.2.21 ⬆️ 5.2.22**|PostgreSQLJDBCDriver|1.0.3|
|CSparkMetricUpdate|1.0.16|**Python**|**3.11/1.0.1 ⬆️ 3.11/1.0.2**|
|**Delta**|**3.2.1.20251125.5 ⬆️ 3.2.1.20260209.3**|R|1.0.7|
|DSCopilot|1.3.2|SparkAdvisor|1.0.7|
|DSCopilotInstaller|1.0.0|SparkDiagnosticsLibrary|1.0.31|
|Esri|1.0.0|SparkJobInsight|1.0.1|
|EventHubConnector|2.3.27|SparkLighter|2.0.4|
|EventStreamsFabricExtension|1.0.0|**SparkLineage**|**0.0.3 ⬆️ 0.0.4**|
|FabricDWConnector|1.0.21|SparklyrConnector|2.0.1|
|**FLTSparkExtensions**|**0.14.0 ⬆️ 0.16.0**|SparkNativeParquetWriter|1.3.0-20250828.2|
|FLTSparkUtils|0.3.0|SparkRPCHistoryServer|1.8.1|
|**FsspecWrapper**|**1.0.6 ⬆️ 1.0.7**|SparkSqlConnector|1.6.9|
|**Genesis**|**0.36.1 ⬆️ 0.36.3**|SQLServerODBCDriver|18.1.0|
|**GlutenUI**|**1.3.0-20260122.1 ⬆️ 1.3.0-20260209.3**|SStreamOnSparkJar|2.4.1|
|HiveMetaStoreClient|1.1.21.3|**TokenLibrary**|**4.3.8 ⬆️ 4.3.9**|
|**Impulse**|**1.3.198470504 ⬆️ 1.3.198470504.1**|**TridentCore**|**1.2.31 ⬆️ 1.3.2**|
|KustoConnector|1.5.1|TridentTokenLibrary|1.10.4|
|LibraryManager|1.0.25|Vegas|3.5.10|
|**LibraryMetadataCooker**|**2.0.4 ⬆️ 2.0.5**|VPaaSClient|3.5.03|
|MlflowLibrary|2.11.3.1|**Wildfire**|**1.10.46.1 ⬆️ 1.10.48.1**|
|**MMLSpark**|**1.4.27 ⬆️ 1.4.29**|
|MySQLJavaConnector|1.0.3|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_openmp_mutex|5.1|locket|1.0.0|
|_py-xgboost-mutex|2.0|lunardate|0.2.2|
|_sysroot_linux-64_curr_repodata_hack|3|lxml|4.9.3|
|abseil-cpp|20211102.0|lz4|4.3.2|
|absl-py|2.1.0|lz4-c|1.9.4|
|accelerate|0.30.1|lzo|2.10|
|adlfs|2024.2.0|make|4.2.1|
|aiohttp|3.9.3|mako|1.3.5|
|aiosignal|1.2.0|markdown|3.4.1|
|alabaster|0.7.12|markdown-it-py|2.2.0|
|alembic|1.13.2|markupsafe|2.1.3|
|anyio|4.2.0|matplotlib|3.8.0|
|aom|3.6.0|matplotlib-base|3.8.0|
|appdirs|1.4.4|matplotlib-inline|0.1.6|
|archspec|0.2.3|mccabe|0.7.0|
|argon2-cffi|21.3.0|mdurl|0.1.0|
|argon2-cffi-bindings|21.2.0|menuinst|2.0.2|
|arrow|1.2.3|minio|7.1.0|
|arrow-cpp|14.0.2|mistune|2.0.4|
|asgiref|3.5.2|mkl|2023.1.0|
|asn1crypto|1.5.1|mkl-service|2.4.0|
|astor|0.8.1|mkl_fft|1.3.8|
|astropy|5.3.4|mkl_random|1.2.4|
|asttokens|2.0.5|mlflow-skinny|2.12.2|
|async-lru|2.0.4|mock|4.0.3|
|async-timeout|4.0.3|more-itertools|10.1.0|
|async_generator|1.10|mpc|1.1.0|
|atk-1.0|2.36.0|mpfr|4.0.2|
|attrs|23.1.0|mpi|1.0|
|autopep8|2.0.4|mpich|4.1.1|
|aws-c-auth|0.6.19|mpmath|1.3.0|
|aws-c-cal|0.5.20|msal|2023.12.01|
|aws-c-common|0.8.5|msal-extensions|2023.12.01|
|aws-c-compression|0.2.16|msgpack-python|1.0.3|
|aws-c-event-stream|0.2.15|msrest|2023.12.01|
|aws-c-http|0.6.25|multidict|6.0.4|
|aws-c-io|0.13.10|multipledispatch|0.6.0|
|aws-c-mqtt|0.7.13|multiprocess|0.70.15|
|aws-c-s3|0.1.51|munkres|1.1.4|
|aws-c-sdkutils|0.1.6|mypy|1.4.1|
|aws-checksums|0.1.13|mypy_extensions|1.0.0|
|aws-crt-cpp|0.18.16|mysql|5.7.24|
|aws-sdk-cpp|1.10.55|nbclassic|1.0.0|
|azure-core|1.30.2|nbclient|0.8.0|
|azure-datalake-store|0.0.53|nbconvert|7.10.0|
|azure-identity|2023.12.01|nbformat|5.9.2|
|azure-keyvault|2023.12.01|ncurses|6.4|
|azure-storage|2023.12.01|nest-asyncio|1.6.0|
|azure-storage-blob|12.22.0|networkx|3.1|
|azure-storage-file-datalake|12.16.0|ninja|1.10.2|
|azureml-synapse|0.0.1|ninja-base|1.10.2|
|babel|2.11.0|nltk|3.8.1|
|backports|1.1|nni|3.0|
|backports.shutil_get_terminal_size|1.0.0|nose|1.3.7|
|bcrypt|3.2.0|notebook|7.0.8|
|beautifulsoup4|4.12.2|notebook-shim|0.2.3|
|binaryornot|0.4.4|**notebookutils**|**1.1.12.35 ⬆️ 1.1.13.35.20260208.7**|
|binutils_impl_linux-64|2.38|nspr|4.35|
|binutils_linux-64|2.38.0|nss|3.89.1|
|bitarray|2.5.1|numba|0.59.0|
|bkcharts|0.2|numexpr|2.8.7|
|black|23.11.0|numpy|1.26.4|
|blas|1.0|numpy-base|1.26.4|
|bleach|4.1.0|numpydoc|1.5.0|
|blinker|1.6.2|nvidia-ml-py|12.560.30|
|blosc|1.21.3|oauthlib|3.2.2|
|bokeh|3.3.4|olefile|0.46|
|boltons|23.0.0|openjpeg|2.4.0|
|boost-cpp|1.82.0|openml|0.12.2|
|boto|2.49.0|openpyxl|3.0.10|
|bottleneck|1.3.7|openssl|3.0.13|
|brotli|1.0.9|optuna|3.6.1|
|brotli-bin|1.0.9|orc|1.7.4|
|brotli-python|1.0.9|overrides|7.4.0|
|brunsli|0.1|packaging|23.1|
|bzip2|1.0.8|pandas|2.1.4|
|c-ares|1.19.1|pandasnet|1.0|
|c-blosc2|2.12.0|pandasql|0.7.3|
|ca-certificates|2023.12.12|pandocfilters|1.5.0|
|cached-property|1.5.2|pango|1.50.7|
|cairo|1.16.0|paramiko|2.8.1|
|catboost|1.2.3|parso|0.8.3|
|certifi|2024.2.2|partd|1.4.1|
|cffi|1.16.0|patch|2.7.6|
|cfitsio|3.470|patchelf|0.17.2|
|chardet|4.0.0|path|16.2.0|
|charls|2.2.0|path.py|12.5.0|
|charset-normalizer|2.0.4|pathlib2|2.3.6|
|chat-magics|0.1.25.2.28|pathspec|0.10.3|
|chat-magics-fabric|0.2.0.25.8.13|patsy|0.5.3|
|click|8.1.7|pcre2|10.42|
|cloudpickle|2.2.1|pep8|1.7.1|
|clr_loader|0.2.5|pexpect|4.8.0|
|cmake|3.26.4|pickleshare|0.7.5|
|cmdstan|2.33.1|pillow|10.2.0|
|cmdstanpy|1.1.0|pip|23.3.1|
|colorama|0.4.6|pixman|0.40.0|
|colorlog|6.8.2|pkginfo|1.9.6|
|comm|0.2.1|platformdirs|3.10.0|
|conda-package-handling|2.2.0|plotly|5.22.0|
|conda-package-streaming|0.9.0|pluggy|1.0.0|
|configparser|5.0.2|ply|3.11|
|contextlib2|21.6.0|poppler|22.12.0|
|contourpy|1.2.0|poppler-data|0.4.11|
|**control-script**|**1.0.3**|portalocker|2.3.0|
|convertdate|2.4.0|powerbiclient|3.1.1|
|cookiecutter|2.5.0|prettytable|3.5.0|
|cryptography|42.0.2|prometheus_client|0.14.1|
|curl|8.5.0|prompt-toolkit|3.0.43|
|cycler|0.11.0|prompt_toolkit|3.0.43|
|cyrus-sasl|2.1.28|prophet|1.1.5|
|cython|3.0.8|prose-pandas2pyspark|10.5.0rc2024121001|
|cytoolz|0.12.2|prose-suggestions|10.4.1|
|daal4py|2023.1.1|protobuf|3.20.3|
|dal|2023.1.1|psutil|5.9.0|
|dash|2.17.1|ptyprocess|0.7.0|
|dash-core-components|2.0.0|pure_eval|0.2.2|
|dash-cytoscape|1.0.2|py-cpuinfo|9.0.0|
|dash-html-components|2.0.0|py-lief|0.12.3|
|dash-table|5.0.0|py-xgboost|2.0.3|
|dask|2023.11.0|py4j|0.10.9.7|
|dask-core|2023.11.0|pyarrow|14.0.2|
|dataclasses|0.8|pybind11-abi|4|
|datasets|2.19.1|pycodestyle|2.11.1|
|dav1d|1.2.1|pycosat|0.6.6|
|dbus|1.13.18|pycparser|2.21|
|debugpy|1.6.7|pycurl|7.45.2|
|decorator|5.1.1|pydocstyle|6.3.0|
|defusedxml|0.7.1|pyerfa|2.0.0|
|dill|0.3.8|pyflakes|3.2.0|
|distlib|0.3.8|pygments|2.15.1|
|distributed|2023.11.0|pyjwt|2.4.0|
|distro|1.8.0|pyluach|2.2.0|
|django|4.1|pymeeus|0.5.12|
|docker|7.0.0|pynacl|1.5.0|
|docutils|0.18.1|pyodbc|5.0.1|
|ds-copilot|0.1.25.2.28|pyopenssl|24.0.0|
|dscopilot-installer|0.0.7|pyparsing|3.0.9|
|entrypoints|0.4|pyperclip|1.8.2|
|et_xmlfile|1.1.0|pyqt|5.15.10|
|executing|0.8.3|pyqt5-sip|12.13.0|
|expat|2.5.0|pyrsistent|0.20.0|
|fabric-connection|0.2.0|pysocks|1.7.1|
|fastcache|1.1.0|pyspark|3.5.1.5.4.20240407|
|filelock|3.11.0|pytables|3.9.2|
|flake8|7.0.0|pytest|7.4.0|
|**flaml**|**2.3.6.post1 ⬆️ 2.5.0.post1**|python|3.11.8|
|flask|2.2.5|python-dateutil|2.8.2|
|flit|3.9.0|python-fastjsonschema|2.16.2|
|flit-core|3.9.0|python-graphviz|0.20.1|
|**flt-python**|**0.14.0 ⬆️ 0.16.0**|python-json-logger|2.0.7|
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
|fsspec_wrapper|0.1.15|qdarkstyle|3.2.3|
|future|0.18.3|qstylizer|0.2.2|
|gcc_impl_linux-64|11.2.0|qt|5.15.9|
|gcc_linux-64|11.2.0|qt-main|5.15.2|
|gdk-pixbuf|2.42.10|qt-webengine|5.15.9|
|geoanalytics-fabric|1.0.0|qtawesome|1.2.2|
|geographiclib|2.0|qtconsole|5.5.1|
|geopy|2.4.1|qtpy|2.4.1|
|get_terminal_size|1.0.0|re2|2022.04.01|
|gevent|23.9.1|readline|8.2|
|gflags|2.2.2|referencing|0.30.2|
|giflib|5.2.1|regex|2023.10.3|
|gitdb|4.0.7|reproc|14.2.4|
|gitpython|3.1.43|reproc-cpp|14.2.4|
|glib|2.78.4|requests|2.31.0|
|glib-tools|2.78.4|requests-oauthlib|1.3.0|
|glob2|0.7|responses|0.25.3|
|glog|0.5.0|retrying|1.3.4|
|gmp|6.2.1|rfc3339-validator|0.1.4|
|gmpy2|2.1.2|rfc3986-validator|0.1.1|
|gobject-introspection|1.78.1|rgf-python|3.12.0|
|graphite2|1.3.14|rhash|1.4.3|
|graphviz|2.50.0|rich|13.3.5|
|greenlet|3.0.1|ripgrep|13.0.0|
|grpc-cpp|1.48.2|rouge-score|0.1.2|
|gson|0.0.4|rpds-py|0.10.6|
|gst-plugins-base|1.14.1|rtree|1.0.1|
|gstreamer|1.14.1|ruamel.yaml|0.17.21|
|gtk2|2.24.33|ruamel.yaml.clib|0.2.7|
|gts|0.7.6|ruamel_yaml|0.17.21|
|gxx_impl_linux-64|11.2.0|s2n|1.3.27|
|gxx_linux-64|11.2.0|safetensors|0.4.2|
|harfbuzz|4.3.0|salib|1.5.0|
|hcrystalball|0.1.10|schema|0.7.7|
|hdf5|1.12.1|scikit-build|0.15.0|
|heapdict|1.0.1|scikit-image|0.22.0|
|holidays|0.48|scikit-learn|1.2.2|
|html5lib|1.1|scikit-learn-intelex|2023.1.1|
|huggingface_hub|0.23.1|scipy|1.11.4|
|icu|73.1|seaborn|0.12.2|
|idna|3.4|secretstorage|3.3.1|
|imagecodecs|2023.1.23|semantic-link-sempy|0.11.0|
|imageio|2.33.1|send2trash|1.8.2|
|imagesize|1.4.1|seqeval|1.2.2|
|importlib-metadata|7.0.1|setuptools|68.2.2|
|importlib_metadata|7.0.1|shap|0.42.1|
|importlib_resources|6.4.0|simplegeneric|0.8.1|
|impulse-python-handler|1.3.198470504|simplejson|3.19.3|
|inflection|0.5.1|singledispatch|3.7.0|
|iniconfig|1.1.1|sip|6.7.12|
|intel-openmp|2023.1.0|six|1.16.0|
|interpret|0.6.0|slicer|0.0.7|
|interpret-core|0.6.0|smmap|4.0.0|
|intervaltree|3.1.0|snappy|1.1.10|
|ipykernel|6.28.0|sniffio|1.3.0|
|ipython|8.20.0|snowballstemmer|2.2.0|
|ipython_genutils|0.2.0|sortedcollections|2.1.0|
|ipywidgets|8.1.2|sortedcontainers|2.4.0|
|isodate|0.6.1|soupsieve|2.5|
|itsdangerous|2.0.1|spark-mssql-connector-fabric35|1.0.0|
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
|jsonpointer|2.1|sqlanalyticsfabricconnectorpy|1.0.1|
|jsonschema|4.19.2|sqlite|3.41.2|
|jsonschema-specifications|2023.7.1|sqlparse|0.4.4|
|jupyter-lsp|2.2.0|stack_data|0.2.0|
|jupyter-ui-poll|1.0.0|statsmodels|0.14.0|
|jupyter_client|8.6.0|sympy|1.12|
|jupyter_console|6.6.3|**synapseml**|**1.1.1**|
|jupyter_core|5.5.0|**synapseml-internal**|**1.1.0.0.dev1 ⬆️ 1.1.1.0**|
|jupyter_events|0.8.0|synapseml-mlflow|1.0.31|
|jupyter_server|2.10.0|synapseml-utils|1.1.6.post2|
|jupyter_server_terminals|0.4.4|sysroot_linux-64|2.17|
|jupyterlab|4.0.11|tbb|2021.8.0|
|jupyterlab_pygments|0.1.2|tbb-devel|2021.8.0|
|jupyterlab_server|2.25.1|tbb4py|2021.8.0|
|jupyterlab_widgets|3.0.10|tblib|1.7.0|
|jxrlib|1.1|tenacity|8.2.3|
|kernel-headers_linux-64|3.10.0|tensorboardx|2.6.2.2|
|keyring|24.3.1|terminado|0.17.1|
|kiwisolver|1.4.4|testpath|0.6.0|
|kqlmagiccustom|0.1.115+fabric.post26|text-unidecode|1.3|
|krb5|1.20.1|textdistance|4.2.1|
|lazy-object-proxy|1.6.0|thop|0.1.1-2209072238|
|lazy_loader|0.3|threadpoolctl|2.2.0|
|lcms2|2.12|tifffile|2023.4.12|
|ld_impl_linux-64|2.38|tinycss2|1.2.1|
|lerc|3.0|tk|8.6.12|
|liac-arff|2.5.0|tokenizers|0.15.1|
|libaec|1.0.4|toml|0.10.2|
|libarchive|3.6.2|tomli|2.0.1|
|libavif|0.11.1|tomli-w|1.0.0|
|libboost|1.82.0|toolz|0.12.0|
|libbrotlicommon|1.0.9|torchdata|0.7.1|
|libbrotlidec|1.0.9|torchmetrics|1.4.0.post0|
|libbrotlienc|1.0.9|tornado|6.3.3|
|libclang|14.0.6|tqdm|4.65.0|
|libclang13|14.0.6|traitlets|5.7.1|
|libcups|2.4.2|transformers|4.37.2|
|libcurl|8.5.0|truststore|0.8.0|
|libdeflate|1.17|typed-ast|1.5.5|
|libedit|3.1.20230828|typeguard|4.1.2|
|libev|4.33|typing-extensions|4.9.0|
|libevent|2.1.12|typing_extensions|4.9.0|
|libffi|3.4.4|tzdata|2024a|
|libgcc-devel_linux-64|11.2.0|ujson|5.4.0|
|libgcc-ng|11.2.0|unicodecsv|0.14.1|
|libgd|2.3.3|unidecode|1.2.0|
|libgfortran-ng|11.2.0|unixodbc|2.3.11|
|libgfortran5|11.2.0|urllib3|2.1.0|
|libglib|2.78.4|utf8proc|2.6.1|
|libgomp|11.2.0|virtualenv|20.26.1|
|libiconv|1.16|wcwidth|0.2.5|
|liblief|0.12.3|webencodings|0.5.1|
|libllvm14|14.0.6|websocket-client|0.58.0|
|libmamba|1.5.6|websockets|12.0|
|libmambapy|1.5.6|werkzeug|2.3.8|
|libnghttp2|1.57.0|wheel|0.41.2|
|libpng|1.6.39|whichcraft|0.6.1|
|libpq|12.17|widgetsnbextension|4.0.10|
|libprotobuf|3.20.3|workalendar|17.0.0|
|library-metadata-cooker|3.6.0.1|wrapt|1.14.1|
|librsvg|2.54.4|xgboost|2.0.3|
|libsodium|1.0.18|xlrd|2.0.1|
|libsolv|0.7.24|xlsxwriter|3.1.1|
|libspatialindex|1.9.3|xlwt|1.3.0|
|libssh2|1.10.0|xmltodict|0.13.0|
|libstdcxx-devel_linux-64|11.2.0|xxhash|0.8.0|
|libstdcxx-ng|11.2.0|xyzservices|2022.9.0|
|libthrift|0.15.0|xz|5.4.6|
|libtiff|4.5.1|yaml|0.2.5|
|libtool|2.4.6|yaml-cpp|0.8.0|
|libuuid|1.41.5|yapf|0.40.2|
|libuv|1.44.2|yarl|1.9.3|
|libwebp|1.3.2|zeromq|4.3.5|
|libwebp-base|1.3.2|zfp|1.0.0|
|libxcb|1.15|zict|3.0.0|
|libxgboost|2.0.3|zipp|3.17.0|
|libxkbcommon|1.0.1|zlib|1.2.13|
|libxml2|2.10.4|zlib-ng|2.0.7|
|libxslt|1.1.37|zope|1.0|
|libzopfli|1.0.3|zope.event|5.0|
|lightgbm|4.3.0|zope.interface|5.4.0|
|lightning-utilities|0.9.0|zstandard|0.19.0|
|llvm-openmp|14.0.6|zstd|1.5.5|
|llvmlite|0.42.0|**Unexpected error while decoding json = string indices must be integers
Unexpected error while decoding json = string indices must be integers
_libgcc_mutex**|**0.1**|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|junit-jupiter-params|5.5.2|
|JLargeArrays|1.5|junit-platform-commons|1.5.2|
|JTransforms|3.1|junit-platform-engine|1.5.2|
|RoaringBitmap|0.9.45|juniversalchardet|2.4.0|
|ST4|4.0.4|kafka-clients|3.4.1|
|SparkCustomEvents|3.5.0-1.0.16|kryo-shaded|4.0.2|
|TokenLibrary-assembly|4.3.8|kusto-spark|3.0_2.12-5.2.2-SNAPSHOT|
|VPaaSConnector|3.5.01|lapack|3.0.3|
|VegasConnector|3.5.10|leveldbjni-all|1.8|
|activation|1.1.1|libfb303|0.9.3|
|aircompressor|0.27|libthrift|0.12.0|
|algebra|2.12-2.0.1|lightgbmlib|3.3.510|
|aliyun-java-sdk-core|4.5.10|log4j|1.2-api-2.20.0|
|aliyun-java-sdk-kms|2.11.0|log4j-api|2.20.0|
|aliyun-java-sdk-ram|3.1.0|log4j-core|2.20.0|
|aliyun-sdk-oss|3.13.0|log4j-slf4j2-impl|2.20.0|
|annotations|17.0.0|lz4-java|1.8.0|
|antlr-runtime|3.5.2|mdsdclientdynamic|2.0|
|antlr4-runtime|4.9.3|metrics-core|4.2.19|
|aopalliance-repackaged|2.6.1|metrics-graphite|4.2.19|
|apiguardian-api|1.1.0|metrics-healthchecks|4.2.9|
|arpack|3.0.3|metrics-jmx|4.2.19|
|arpack_combined_all|0.1|metrics-json|4.2.19|
|arrow-format|12.0.1|metrics-jvm|4.2.19|
|arrow-memory-core|12.0.1|metrics-servlet|4.2.10|
|arrow-memory-netty|12.0.1|metrics-servlets|4.2.10|
|arrow-vector|12.0.1|metrics4-scala|2.12-4.2.9|
|audience-annotations|0.5.0|microsoft-catalog-metastore-client|1.1.21|
|avro|1.11.4|microsoft-log4j-etwappender|1.0|
|avro-ipc|1.11.4|minlog|1.3.0|
|avro-mapred|1.11.4|mlflow-spark|2.12-2.11.3|
|aws-java-sdk-bundle|1.12.262|mysql-connector-java|8.0.18|
|azure-core|1.47.0|netty-all|4.1.96.Final|
|azure-core-http-netty|1.14.1|netty-buffer|4.1.96.Final|
|azure-data-lake-store-sdk|2.3.9|netty-codec|4.1.96.Final|
|azure-eventhubs|3.3.0|netty-codec-dns|4.1.101.Final|
|azure-eventhubs-spark|2.12-2.3.22|netty-codec-http|4.1.96.Final|
|azure-json|1.1.0|netty-codec-http2|4.1.96.Final|
|azure-keyvault-core|1.0.0|netty-codec-socks|4.1.96.Final|
|azure-storage|7.0.1|netty-common|4.1.96.Final|
|azure-storage-blob|12.25.3|netty-handler|4.1.96.Final|
|azure-storage-common|12.24.3|netty-handler-proxy|4.1.96.Final|
|azure-storage-internal-avro|12.10.3|netty-resolver|4.1.96.Final|
|azure-synapse-ml-pandas|2.12-0.1.1|netty-resolver-dns|4.1.101.Final|
|blas|3.0.3|netty-resolver-dns-classes-macos|4.1.101.Final|
|bonecp|0.8.0.RELEASE|netty-resolver-dns-native-macos|4.1.101.Final-osx-x86_64|
|breeze|2.12-2.1.0|netty-tcnative-boringssl-static|2.0.62.Final-linux-aarch_64|
|breeze-macros|2.12-2.1.0|netty-tcnative-boringssl-static|2.0.62.Final-linux-x86_64|
|cats-kernel|2.12-2.1.1|netty-tcnative-boringssl-static|2.0.62.Final-osx-aarch_64|
|chill|2.12-0.10.0|netty-tcnative-boringssl-static|2.0.62.Final-osx-x86_64|
|chill-java|0.10.0|netty-tcnative-boringssl-static|2.0.62.Final-windows-x86_64|
|client-sdk|1.24.1|netty-tcnative-boringssl-static|2.0.62.Final|
|commons-cli|1.5.0|netty-tcnative-classes|2.0.62.Final|
|commons-codec|1.16.1|netty-transport|4.1.96.Final|
|commons-collections|3.2.2|netty-transport-classes-epoll|4.1.96.Final|
|commons-collections4|4.4|netty-transport-classes-kqueue|4.1.96.Final|
|commons-compiler|3.1.9|netty-transport-native-epoll|4.1.96.Final-linux-aarch_64|
|commons-compress|1.23.0|netty-transport-native-epoll|4.1.96.Final-linux-x86_64|
|commons-crypto|1.1.0|netty-transport-native-kqueue|4.1.96.Final-osx-aarch_64|
|commons-dbcp|1.4|netty-transport-native-kqueue|4.1.96.Final-osx-x86_64|
|commons-io|2.11.0|netty-transport-native-unix-common|4.1.96.Final|
|commons-io|2.18.0|nimbus-jose-jwt|9.37.2|
|commons-lang|2.6|**notebook-utils**|**1.1.12-spark35 ⬆️ 1.1.13-spark35-20260208.7**|
|commons-lang3|3.12.0|objenesis|3.3|
|commons-logging|1.1.3|onnx-protobuf|2.12-0.9.3|
|commons-math3|3.6.1|onnxruntime_gpu|1.8.1|
|commons-pool|1.5.4|opencsv|2.3|
|commons-pool2|2.11.1|opencv|3.2.0-1|
|commons-text|1.10.0|openlineage-spark|2.12-1.26.0|
|compress-lzf|1.1.2|opentest4j|1.2.0|
|curator-client|2.13.0|opentracing-api|0.33.0|
|curator-framework|2.13.0|opentracing-noop|0.33.0|
|curator-recipes|2.13.0|opentracing-util|0.33.0|
|datanucleus-api-jdo|4.2.4|orc-core|1.9.5-shaded-protobuf|
|datanucleus-core|4.1.17|orc-mapreduce|1.9.5-shaded-protobuf|
|datanucleus-rdbms|4.1.19|orc-shims|1.9.5|
|datasketches-java|3.3.0|oro|2.0.8|
|datasketches-memory|2.1.0|osgi-resource-locator|1.0.3|
|**delta-kernel-api**|**3.2.1.20251125.5 ⬆️ 3.2.1.20260209.3**|paranamer|2.8|
|**delta-kernel-defaults**|**3.2.1.20251125.5 ⬆️ 3.2.1.20260209.3**|parquet-column|1.13.1|
|**delta-spark**|**2.12-3.2.1.20251125.5 ⬆️ 2.12-3.2.1.20260209.3**|parquet-common|1.13.1|
|**delta-storage**|**3.2.1.20251125.5 ⬆️ 3.2.1.20260209.3**|parquet-encoding|1.13.1|
|derby|10.14.2.0|parquet-format-structures|1.13.1|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|**parquet-hadoop-ms**|**3.5.5.5.4.20260126.1 ⬆️ 3.5.5.5.4.20260211.1**|
|fastutil|7.0.2|parquet-jackson|1.13.1|
|flatbuffers-java|1.12.0|pickle|1.3|
|**flt-spark-sql-extensions**|**0.14.0 ⬆️ 0.16.0**|postgresql|42.2.9|
|fluent-logger|0.3.4-jar-with-dependencies-provided|profiler|1.1.1|
|gcs-connector-hadoop3|2.2.14-shaded|proton-j|0.33.8|
|**genesis-client**|**2.12-0.36.1-jar-with-dependencies ⬆️ 2.12-0.36.3-jar-with-dependencies**|py4j|0.10.9.7|
|geoanalytics-fabric|2.12-1.0.0-msfabric-1.3|qpid-proton-j-extensions|1.2.4|
|**gluten-velox-bundle-spark**|**2.12-mariner_2.0_x86_64-1.3.0-20260122.1 ⬆️ 2.12-mariner_2.0_x86_64-1.3.0-20260209.3**|reactive-streams|1.0.3|
|gson|2.8.9|reactor-core|3.4.34|
|guava|14.0.1|reactor-netty-core|1.0.40|
|h3|4.1.1|reactor-netty-http|1.0.40|
|**hadoop-aliyun**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|rocksdbjni|8.3.2|
|**hadoop-annotations**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scala-collection-compat|2.12-2.7.0|
|**hadoop-aws**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scala-compiler|2.12.18|
|**hadoop-azure**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scala-java8-compat|2.12-0.9.0|
|**hadoop-azure-datalake**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scala-library|2.12.18|
|hadoop-azureml|1.0-fs|scala-parser-combinators|2.12-2.3.0|
|**hadoop-client-api**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scala-reflect|2.12.18|
|**hadoop-client-runtime**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scala-xml|2.12-2.1.0|
|**hadoop-cloud-storage**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scalactic|2.12-3.2.14|
|**hadoop-openstack**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scalatra|2.12-3.0.0-M1|
|hadoop-shaded-guava|1.1.1|scalatra-common|2.12-3.0.0-M1|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.4.20260126.1 ⬆️ 3.3.4.5.4.20260211.1**|scalatra-metrics|2.12-3.0.0-M1|
|hdinsight-spark-metrics|3.5.0-1.0.16|shims|0.9.45|
|hive-common|2.3.9|slf4j-api|2.0.7|
|hive-exec|2.3.9-core|snappy-java|1.1.10.5|
|hive-llap-common|2.3.9|spark|3.5-advisor-core_2.12-1.0.18|
|hive-metastore|2.3.9|spark|3.5-rpc-history-server-app-listener_2.12-1.0.0|
|hive-serde|2.3.9|spark|3.5-rpc-history-server-core_2.12-1.0.0|
|hive-shims|0.23-2.3.9|spark-avro|2.12-3.5.0|
|hive-shims|2.3.9|**spark-avro**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|hive-shims-common|2.3.9|**spark-catalyst**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|hive-shims-scheduler|2.3.9|**spark-common-utils**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|hive-storage-api|2.8.1|**spark-core**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|hk2-api|2.6.1|**spark-enhancement**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|hk2-locator|2.6.1|spark-enhancementui|2.12-3.3.0|
|hk2-utils|2.6.1|spark-eventstream-extensions|1.0.5|
|httpclient|4.5.14|spark-excel-thin|2.12-3.5.6_0.31.2|
|httpclient5|5.1.3|**spark-graphx**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|httpcore|4.4.16|**spark-hadoop-cloud**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|httpmime|4.5.13|**spark-hive**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|httpmime|4.5.14|spark-jobinsight|2.12-1.0.0-spark3.5|
|impulse-core_spark|2.12-1.3.198470504|spark-kusto-synapse-connector|3.5_2.12-1.5.1|
|impulse-exception_java11|2.12-1.3.198470504|**spark-kvstore**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|impulse-telemetry-mds_spark|2.12-1.3.198470504|**spark-launcher**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|ini4j|0.5.4|spark-lighter-contract|2.12-2.1.0_spark-3.5.1_20240717.4|
|isolation-forest|3.5.0_2.12-3.0.5|spark-lighter-core|2.12-2.0.11_spark-3.5.1_20240717.4|
|istack-commons-runtime|3.0.8|**spark-microsoft-tools**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|ivy|2.5.1|**spark-mllib**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-annotations|2.15.2|**spark-mllib-local**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-core|2.15.2|spark-mssql-connector-fabric35|1.6.9|
|jackson-core-asl|1.9.13|**spark-network-common**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-databind|2.15.2|**spark-network-shuffle**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-dataformat-cbor|2.15.2|**spark-onesecurity-client**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-dataformat-xml|2.12.7|**spark-onesecurity-common**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-datatype-jsr310|2.15.2|**spark-onesecurity-server**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-mapper-asl|1.9.13|**spark-repl**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-module-jaxb-annotations|2.15.2|**spark-sketch**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jackson-module-scala|2.12-2.15.2|**spark-sql**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.activation-api|1.2.2|**spark-sql-api**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.annotation-api|1.3.5|**spark-sql-kafka**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.inject|2.6.1|**spark-streaming**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.servlet-api|4.0.3|**spark-streaming-kafka**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.validation-api|2.0.2|**spark-tags**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.ws.rs-api|2.1.6|**spark-token-provider-kafka**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|jakarta.xml.bind-api|2.3.2|**spark-unsafe**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|janino|3.1.9|spark-xml|2.12-0.17.0|
|javassist|3.29.2-GA|**spark-yarn**|**2.12-3.5.5.5.4.20260126.1 ⬆️ 2.12-3.5.5.5.4.20260211.1**|
|javatuples|1.2|spark_diagnostic_cli|2.1.7_spark-3.5.1_20250901.3-shaded|
|javax.jdo|3.2.0-m3|sparklyr-connector|3.5.1-1.0.0267535|
|javolution|5.5.1|sparknativeparquetwriter|2.12-1.3.0-20250828.2|
|jaxb-api|2.2.11|spire|2.12-0.17.0|
|jaxb-runtime|2.3.2|spire-macros|2.12-0.17.0|
|jcip-annotations|1.0-1|spire-platform|2.12-0.17.0|
|jcl-over-slf4j|2.0.7|spire-util|2.12-0.17.0|
|jdo-api|3.0.1|spray-json|2.12-1.3.5|
|jdom2|2.0.6|stax-api|1.0.1|
|jersey-client|2.40|stax2-api|4.2.1|
|jersey-common|2.40|stream|2.9.6|
|jersey-container-servlet|2.40|structuredstream|2.12-2.4.1|
|jersey-container-servlet-core|2.40|structuredstreamforspark|2.12-2.4.1|
|jersey-hk2|2.40|**synapseml-cognitive**|**2.12-1.1.0 ⬆️ 2.12-1.1.1**|
|jersey-server|2.40|**synapseml-core**|**2.12-1.1.0 ⬆️ 2.12-1.1.1**|
|jettison|1.1|**synapseml-deep-learning**|**2.12-1.1.0 ⬆️ 2.12-1.1.1**|
|jetty-util|9.4.57.v20241219|**synapseml-internal**|**2.12-1.1.0.0-spark3.5 ⬆️ 2.12-1.1.1.0**|
|jetty-util-ajax|9.4.57.v20241219|**synapseml-lightgbm**|**2.12-1.1.0 ⬆️ 2.12-1.1.1**|
|jline|2.14.6|**synapseml-opencv**|**2.12-1.1.0 ⬆️ 2.12-1.1.1**|
|joda-time|2.12.5|**synapseml-vw**|**2.12-1.1.0 ⬆️ 2.12-1.1.1**|
|jodd-core|3.5.2|**synfs**|**1.1.12-spark35 ⬆️ 1.1.13-spark35-20260208.7**|
|jsch|0.1.54|threeten-extra|1.7.1|
|json|1.8|tink|1.9.0|
|json|20231013|transaction-api|1.1|
|json-simple|1.1.1|transform-token-provider-utils|0.3.0|
|json-simple|1.1|**trident-core**|**1.2.31 ⬆️ 1.3.2**|
|json4s-ast|2.12-3.7.0-M11|tridenttokenlibrary-assembly|1.10.4|
|json4s-core|2.12-3.7.0-M11|univocity-parsers|2.9.1|
|json4s-jackson|2.12-3.7.0-M11|vw-jni|9.3.0|
|json4s-scalap|2.12-3.7.0-M11|wildfly-openssl|1.0.7.Final|
|jsr305|3.0.0|woodstox-core|6.2.4|
|jta|1.1|xbean-asm9-shaded|4.23|
|jul-to-slf4j|2.0.7|xz|1.9|
|junit-jupiter|5.5.2|**zookeeper**|**3.6.3.5.4.20260126.1 ⬆️ 3.6.3.5.4.20260211.1**|
|junit-jupiter-api|5.5.2|**zookeeper-jute**|**3.6.3.5.4.20260126.1 ⬆️ 3.6.3.5.4.20260211.1**|
|junit-jupiter-engine|5.5.2|zstd-jni|1.5.5-4|

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
|R.oo|1.27.1|mgcv|1.9-1|
|R.utils|2.13.0|mime|0.12|
|R6|2.5.1|miniUI|0.1.1.1|
|R6P|0.3.0|modeldata|1.4.0|
|RColorBrewer|1.1-3|modelenv|0.1.1|
|RODBC|1.3-23|modelr|0.1.11|
|Rcpp|1.0.13|munsell|0.5.1|
|SQUAREM|2021.1|nlme|3.1-165|
|TTR|0.24.4|nnet|7.3-19|
|V8|5.0.0|**notebookutils**|**1.1.12.35 ⬆️ 1.1.13.35.20260208.7**|
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

