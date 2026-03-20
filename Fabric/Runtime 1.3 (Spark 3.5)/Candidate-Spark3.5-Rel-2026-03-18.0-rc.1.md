# System Environment
*   **Product**: Fabric Runtime 1.3 (Spark 3.5)
*   **VHD Name**: d6844584311409.vhd
*   **Vhd Release**: Spark3.5-Rel-2026-03-18.0-rc.1
*   **Operating System**: CBL-Mariner 2.0.20260304
*   **Apache Spark**: 3.5.5
*   **Java**: 11.0.27
*   **Scala**: 2.12.18
*   **Python**: 3.11/1.0.2
*   **Delta Lake**: 3.2.1.20260303.1

# New Features
|Id|Component|Description|
|-----|-----|-----|
|1997016|Wildfire/spark35:1.10.51|New Spark 3.5 Release which includes changes in wildfire-spark|
|1974944|ServiceConfigurationTemplates:spark/3.5.0|Adds Spark storage decommission fallback storage configuration for trident clusters to support shuffle data migration during node decommission|
|1991230|FabricDWConnector:1.0.23|Add Batch Insert write strategies for Fabric DW Connector|
|1981688|Wildfire/spark35:1.10.50, Delta:3.2.1.20260303.1|Introduces Spark 3.5 Wildfire release with schema-less lakehouse fix requiring coordinated changes across Spark, Gluten, and Delta components to ensure compatibility and resolve cyclic dependencies.|
|1958699|Wildfire/spark35:1.10.49|Introduces Spark 3.5 release with updates to wildfire-spark and wildfire-livy.|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1994224|SparkSqlConnector:1.6.10|Remove excessive logging impacting performance. Fix bug involving writing Spark timestamp to sql server|
|1989904|CSparkMetricUpdate:1.0.17|Updates to release the latest Spark Runtime telemetry and redaction log utilities|
|1997016|Wildfire/spark35:1.10.51|New Spark 3.5 Release which includes changes in wildfire-spark|
|1974944|ServiceConfigurationTemplates:spark/3.5.0|Adds Spark storage decommission fallback storage configuration for trident clusters to support shuffle data migration during node decommission|
|1989272|Genesis:0.37.0, LibraryManager:1.0.26|This change improves LDS error classification and ensures meaningful errors are surfaced to the UI for easier troubleshooting. It also fine tunes the default LDS timeout value while also allowing it to be user configurable|
|1991230|FabricDWConnector:1.0.23|Add Batch Insert write strategies for Fabric DW Connector|
|1966034|ServiceConfigurationTemplates:Spark35|Updated Livy Spark 3.5 configuration to improve maintainability, add a 20-minute REPL driver idle timeout, and remove unsupported .NET settings while preserving Fabric safety checks.|
|1968489|FLTSparkExtensions:0.18.0|Introduces reliability, logging, and infrastructure improvements across MLV, FLT, and Shield components, enhancing error handling, observability, CI robustness, and performance validation in Spark 3.5.|
|1969403|OnelakeSparkCatalog: 0.4.7|Adds support for shared artifact scenarios in VNet environments, similar to public environments, controlled via a feature flag. Fixes private artifactType name resolution issues in the OneLake API endpoint.|
|1972561|SparkDiagnosticLibrary:1.0.32|Aligns fabricLivyId logic with updated behavior and adds a deprecation warning for legacy LA configurations in Spark 3.5.|
|1972838|TridentCore:1.3.4|Updates Trident-core to include new configurations for permanent UDF support and fixes a bug related to GUID handling in VNet scenarios.|
|1981688|Wildfire/spark35:1.10.50, Delta:3.2.1.20260303.1|Introduces Spark 3.5 Wildfire release with schema-less lakehouse fix requiring coordinated changes across Spark, Gluten, and Delta components to ensure compatibility and resolve cyclic dependencies.|
|1983775|SparkNativeParquetWriter:1.3.0-20260304.4|Updates to SparkNativeParquetWriter|
|1932364|KustoConnector:2.0.1|Upgrades Kusto Connector SDK to 7.0.3 to align with recent Kusto engine changes, preventing future issues in Synapse and Fabric Spark 3.5 environments.|
|1958699|Wildfire/spark35:1.10.49|Introduces Spark 3.5 release with updates to wildfire-spark and wildfire-livy.|
|1963756|Impulse:1.4.207202278|Upgrades Impulse library to version 1.4.207202278 for Spark 3.5, introducing enhanced error classification, telemetry improvements, sensitive-data scrubbing, and Java 17 build support.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1970926|KustoConnector:2.0.2|Improved connector compatibility with the Native Execution Engine (NEE) by ensuring SAS configuration is passed to Spark|
|1994031|FLTSparkExtensions:0.18.2|Update to resolve a refresh performance issue by upgrading the FLT-SparkExtensions version and correcting its artifact name|
|1965776|ServiceConfigurationTemplates/spark35|Removes deprecated Log4j2 package scanning configuration and an invalid ScrubberList attribute that caused ERROR and WARN messages in driver stdout logs.|
|1968489|FLTSparkExtensions:0.18.0|Introduces reliability, logging, and infrastructure improvements across MLV, FLT, and Shield components, enhancing error handling, observability, CI robustness, and performance validation in Spark 3.5.|
|1969225|Impulse:1.4.208330617|This PR updates Impulse version to `1.4.208330617`.|
|1969403|OnelakeSparkCatalog: 0.4.7|Adds support for shared artifact scenarios in VNet environments, similar to public environments, controlled via a feature flag. Fixes private artifactType name resolution issues in the OneLake API endpoint.|
|1972838|TridentCore:1.3.4|Updates Trident-core to include new configurations for permanent UDF support and fixes a bug related to GUID handling in VNet scenarios.|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|Auditd|0.0.2|NotebookUtils|1.1.63|
|AutoscaleProbe|3.9.9|OneLakeClientStarter|1.0.26.2|
|AzureMLExtensions|1.0.5|**OnelakeSparkCatalog**|**0.4.4 ⬆️ 0.4.8**|
|Conda|5.2.22|PostgreSQLJDBCDriver|1.0.3|
|**CSparkMetricUpdate**|**1.0.16 ⬆️ 1.0.17**|Python|3.11/1.0.2|
|**Delta**|**3.2.1.20260209.3 ⬆️ 3.2.1.20260303.1**|R|1.0.7|
|DSCopilot|1.3.2|SparkAdvisor|1.0.7|
|DSCopilotInstaller|1.0.0|**SparkDiagnosticsLibrary**|**1.0.31 ⬆️ 1.0.32**|
|Esri|1.0.0|SparkJobInsight|1.0.1|
|EventHubConnector|2.3.27|SparkLighter|2.0.4|
|EventStreamsFabricExtension|1.0.0|SparkLineage|0.0.4|
|**FabricDWConnector**|**1.0.21 ⬆️ 1.0.23**|SparklyrConnector|2.0.1|
|FLTSparkExtensions|0.18.2|**SparkNativeParquetWriter**|**1.3.0-20250828.2 ⬆️ 1.3.0-20260304.4**|
|FLTSparkUtils|0.3.0|SparkRPCHistoryServer|1.8.1|
|FsspecWrapper|1.0.7|**SparkSqlConnector**|**1.6.9 ⬆️ 1.6.10**|
|**Genesis**|**0.36.3 ⬆️ 0.37.0**|SQLServerODBCDriver|18.1.0|
|**GlutenUI**|**1.3.0-20260209.3 ⬆️ 1.3.0-20260303.5**|SStreamOnSparkJar|2.4.1|
|**HiveMetaStoreClient**|**1.1.21.3 ⬆️ 1.1.28**|TokenLibrary|4.3.9|
|**Impulse**|**1.3.198470504.1 ⬆️ 1.4.208330617**|**TridentCore**|**1.3.2 ⬆️ 1.3.4**|
|**KustoConnector**|**1.5.1 ⬆️ 2.0.2**|**TridentTokenLibrary**|**1.10.4 ⬆️ 1.11.2**|
|**LibraryManager**|**1.0.25 ⬆️ 1.0.26**|Vegas|3.5.10|
|LibraryMetadataCooker|2.0.5|VPaaSClient|3.5.03|
|MlflowLibrary|2.11.3.1|**Wildfire**|**1.10.48.1 ⬆️ 1.10.51.1**|
|MMLSpark|1.4.29|
|MySQLJavaConnector|1.0.3|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_libgcc_mutex|0.1|nbclassic|1.0.0|
|_openmp_mutex|5.1|nbclient|0.8.0|
|_py-xgboost-mutex|2.0|nbconvert|7.10.0|
|_sysroot_linux-64_curr_repodata_hack|3|nbformat|5.9.2|
|abseil-cpp|20211102.0|ncurses|6.4|
|aiohttp|3.9.3|nest-asyncio|1.6.0|
|aiosignal|1.2.0|networkx|3.1|
|alabaster|0.7.12|ninja|1.10.2|
|anyio|4.2.0|ninja-base|1.10.2|
|aom|3.6.0|nltk|3.8.1|
|appdirs|1.4.4|nose|1.3.7|
|archspec|0.2.3|notebook|7.0.8|
|argon2-cffi|21.3.0|notebook-shim|0.2.3|
|argon2-cffi-bindings|21.2.0|nspr|4.35|
|arrow|1.2.3|nss|3.89.1|
|arrow-cpp|14.0.2|numba|0.59.0|
|asgiref|3.5.2|numexpr|2.8.7|
|asn1crypto|1.5.1|numpy|1.26.4|
|astropy|5.3.4|numpy-base|1.26.4|
|asttokens|2.0.5|numpydoc|1.5.0|
|async-lru|2.0.4|oauthlib|3.2.2|
|async-timeout|4.0.3|olefile|0.46|
|async_generator|1.10|openjpeg|2.4.0|
|atk-1.0|2.36.0|openml|0.12.2|
|attrs|23.1.0|openpyxl|3.0.10|
|autopep8|2.0.4|openssl|3.0.13|
|aws-c-auth|0.6.19|orc|1.7.4|
|aws-c-cal|0.5.20|overrides|7.4.0|
|aws-c-common|0.8.5|packaging|23.1|
|aws-c-compression|0.2.16|pandas|2.1.4|
|aws-c-event-stream|0.2.15|pandasql|0.7.3|
|aws-c-http|0.6.25|pandocfilters|1.5.0|
|aws-c-io|0.13.10|pango|1.50.7|
|aws-c-mqtt|0.7.13|paramiko|2.8.1|
|aws-c-s3|0.1.51|parso|0.8.3|
|aws-c-sdkutils|0.1.6|partd|1.4.1|
|aws-checksums|0.1.13|patch|2.7.6|
|aws-crt-cpp|0.18.16|patchelf|0.17.2|
|aws-sdk-cpp|1.10.55|path|16.2.0|
|azure-identity|2023.12.01|path.py|12.5.0|
|azure-keyvault|2023.12.01|pathlib2|2.3.6|
|azure-storage|2023.12.01|pathspec|0.10.3|
|babel|2.11.0|patsy|0.5.3|
|backports|1.1|pcre2|10.42|
|backports.shutil_get_terminal_size|1.0.0|pep8|1.7.1|
|bcrypt|3.2.0|pexpect|4.8.0|
|beautifulsoup4|4.12.2|pickleshare|0.7.5|
|binaryornot|0.4.4|pillow|10.2.0|
|binutils_impl_linux-64|2.38|pip|23.3.1|
|binutils_linux-64|2.38.0|pixman|0.40.0|
|bitarray|2.5.1|pkginfo|1.9.6|
|bkcharts|0.2|platformdirs|3.10.0|
|black|23.11.0|plotly|5.22.0|
|blas|1.0|pluggy|1.0.0|
|bleach|4.1.0|ply|3.11|
|blinker|1.6.2|poppler|22.12.0|
|blosc|1.21.3|poppler-data|0.4.11|
|bokeh|3.3.4|portalocker|2.3.0|
|boltons|23.0.0|prettytable|3.5.0|
|boost-cpp|1.82.0|prometheus_client|0.14.1|
|boto|2.49.0|prompt-toolkit|3.0.43|
|bottleneck|1.3.7|prompt_toolkit|3.0.43|
|brotli|1.0.9|prophet|1.1.5|
|brotli-bin|1.0.9|protobuf|3.20.3|
|brotli-python|1.0.9|psutil|5.9.0|
|brunsli|0.1|ptyprocess|0.7.0|
|bzip2|1.0.8|pure_eval|0.2.2|
|c-ares|1.19.1|py-cpuinfo|9.0.0|
|c-blosc2|2.12.0|py-lief|0.12.3|
|ca-certificates|2023.12.12|py-xgboost|2.0.3|
|cached-property|1.5.2|pyarrow|14.0.2|
|cairo|1.16.0|pybind11-abi|4|
|catboost|1.2.3|pycodestyle|2.11.1|
|certifi|2024.2.2|pycosat|0.6.6|
|cffi|1.16.0|pycparser|2.21|
|cfitsio|3.470|pycurl|7.45.2|
|chardet|4.0.0|pydocstyle|6.3.0|
|charls|2.2.0|pyerfa|2.0.0|
|charset-normalizer|2.0.4|pyflakes|3.2.0|
|click|8.1.7|pygments|2.15.1|
|cloudpickle|2.2.1|pyjwt|2.4.0|
|clr_loader|0.2.5|pynacl|1.5.0|
|cmake|3.26.4|pyodbc|5.0.1|
|cmdstan|2.33.1|pyopenssl|24.0.0|
|cmdstanpy|1.1.0|pyparsing|3.0.9|
|colorama|0.4.6|pyqt|5.15.10|
|comm|0.2.1|pyqt5-sip|12.13.0|
|conda-package-handling|2.2.0|pyrsistent|0.20.0|
|conda-package-streaming|0.9.0|pysocks|1.7.1|
|configparser|5.0.2|pytables|3.9.2|
|contextlib2|21.6.0|pytest|7.4.0|
|contourpy|1.2.0|python|3.11.8|
|cookiecutter|2.5.0|python-dateutil|2.8.2|
|cryptography|42.0.2|python-fastjsonschema|2.16.2|
|curl|8.5.0|python-graphviz|0.20.1|
|cycler|0.11.0|python-json-logger|2.0.7|
|cyrus-sasl|2.1.28|python-libarchive-c|2.9|
|cython|3.0.8|python-lmdb|1.4.1|
|cytoolz|0.12.2|python-slugify|5.0.2|
|daal4py|2023.1.1|python-tzdata|2023.3|
|dal|2023.1.1|python-xxhash|2.0.2|
|dask|2023.11.0|pythonnet|3.0.1|
|dask-core|2023.11.0|pytorch|2.2.1|
|dataclasses|0.8|pytorch-lightning|2.0.3|
|datasets|2.19.1|pytorch-mutex|1.0|
|dav1d|1.2.1|pytz|2023.3.post1|
|dbus|1.13.18|pywavelets|1.5.0|
|debugpy|1.6.7|pyyaml|6.0.1|
|decorator|5.1.1|pyzmq|25.1.2|
|defusedxml|0.7.1|qdarkstyle|3.2.3|
|dill|0.3.8|qstylizer|0.2.2|
|distlib|0.3.8|qt|5.15.9|
|distributed|2023.11.0|qt-main|5.15.2|
|distro|1.8.0|qt-webengine|5.15.9|
|django|4.1|qtawesome|1.2.2|
|docutils|0.18.1|qtconsole|5.5.1|
|entrypoints|0.4|qtpy|2.4.1|
|et_xmlfile|1.1.0|re2|2022.04.01|
|executing|0.8.3|readline|8.2|
|expat|2.5.0|referencing|0.30.2|
|fastcache|1.1.0|regex|2023.10.3|
|flake8|7.0.0|reproc|14.2.4|
|flask|2.2.5|reproc-cpp|14.2.4|
|flit|3.9.0|requests|2.31.0|
|flit-core|3.9.0|requests-oauthlib|1.3.0|
|fmt|9.1.0|rfc3339-validator|0.1.4|
|font-ttf-dejavu-sans-mono|2.37|rfc3986-validator|0.1.1|
|font-ttf-inconsolata|2.001|rhash|1.4.3|
|font-ttf-source-code-pro|2.030|rich|13.3.5|
|font-ttf-ubuntu|0.83|ripgrep|13.0.0|
|fontconfig|2.14.1|rpds-py|0.10.6|
|fonts-anaconda|1|rtree|1.0.1|
|fonts-conda-ecosystem|1|ruamel.yaml|0.17.21|
|fonttools|4.25.0|ruamel.yaml.clib|0.2.7|
|freetype|2.12.1|ruamel_yaml|0.17.21|
|fribidi|1.0.10|s2n|1.3.27|
|frozenlist|1.4.0|safetensors|0.4.2|
|fsspec_wrapper|0.1.15|scikit-build|0.15.0|
|future|0.18.3|scikit-image|0.22.0|
|gcc_impl_linux-64|11.2.0|scikit-learn|1.2.2|
|gcc_linux-64|11.2.0|scikit-learn-intelex|2023.1.1|
|gdk-pixbuf|2.42.10|scipy|1.11.4|
|geographiclib|2.0|seaborn|0.12.2|
|geopy|2.4.1|secretstorage|3.3.1|
|get_terminal_size|1.0.0|send2trash|1.8.2|
|gevent|23.9.1|setuptools|68.2.2|
|gflags|2.2.2|shap|0.42.1|
|giflib|5.2.1|simplegeneric|0.8.1|
|gitdb|4.0.7|singledispatch|3.7.0|
|gitpython|3.1.43|sip|6.7.12|
|glib|2.78.4|six|1.16.0|
|glib-tools|2.78.4|slicer|0.0.7|
|glob2|0.7|smmap|4.0.0|
|glog|0.5.0|snappy|1.1.10|
|gmp|6.2.1|sniffio|1.3.0|
|gmpy2|2.1.2|snowballstemmer|2.2.0|
|gobject-introspection|1.78.1|sortedcollections|2.1.0|
|graphite2|1.3.14|sortedcontainers|2.4.0|
|graphviz|2.50.0|soupsieve|2.5|
|greenlet|3.0.1|sphinx|5.0.2|
|grpc-cpp|1.48.2|sphinxcontrib|1.0|
|gst-plugins-base|1.14.1|sphinxcontrib-applehelp|1.0.2|
|gstreamer|1.14.1|sphinxcontrib-devhelp|1.0.2|
|gtk2|2.24.33|sphinxcontrib-htmlhelp|2.0.0|
|gts|0.7.6|sphinxcontrib-jsmath|1.0.1|
|gxx_impl_linux-64|11.2.0|sphinxcontrib-qthelp|1.0.3|
|gxx_linux-64|11.2.0|sphinxcontrib-serializinghtml|1.1.5|
|harfbuzz|4.3.0|sphinxcontrib-websupport|1.2.4|
|hdf5|1.12.1|sqlalchemy|2.0.25|
|heapdict|1.0.1|sqlite|3.41.2|
|holidays|0.48|sqlparse|0.4.4|
|html5lib|1.1|stack_data|0.2.0|
|huggingface_hub|0.23.1|statsmodels|0.14.0|
|icu|73.1|sympy|1.12|
|idna|3.4|sysroot_linux-64|2.17|
|imagecodecs|2023.1.23|tbb|2021.8.0|
|imageio|2.33.1|tbb-devel|2021.8.0|
|imagesize|1.4.1|tbb4py|2021.8.0|
|importlib-metadata|7.0.1|tblib|1.7.0|
|importlib_metadata|7.0.1|tenacity|8.2.3|
|importlib_resources|6.4.0|terminado|0.17.1|
|inflection|0.5.1|testpath|0.6.0|
|iniconfig|1.1.1|text-unidecode|1.3|
|intel-openmp|2023.1.0|textdistance|4.2.1|
|intervaltree|3.1.0|threadpoolctl|2.2.0|
|ipykernel|6.28.0|tifffile|2023.4.12|
|ipython|8.20.0|tinycss2|1.2.1|
|ipython_genutils|0.2.0|tk|8.6.12|
|ipywidgets|8.1.2|tokenizers|0.15.1|
|isodate|0.6.1|toml|0.10.2|
|itsdangerous|2.0.1|tomli|2.0.1|
|jaraco.classes|3.2.1|tomli-w|1.0.0|
|jedi|0.18.1|toolz|0.12.0|
|jeepney|0.7.1|torchdata|0.7.1|
|jinja2|3.1.3|torchmetrics|1.4.0.post0|
|joblib|1.2.0|tornado|6.3.3|
|jpeg|9e|tqdm|4.65.0|
|json5|0.9.6|traitlets|5.7.1|
|jsonpatch|1.32|transformers|4.37.2|
|jsonpointer|2.1|truststore|0.8.0|
|jsonschema|4.19.2|typed-ast|1.5.5|
|jsonschema-specifications|2023.7.1|typing-extensions|4.9.0|
|jupyter-lsp|2.2.0|typing_extensions|4.9.0|
|jupyter_client|8.6.0|tzdata|2024a|
|jupyter_console|6.6.3|ujson|5.4.0|
|jupyter_core|5.5.0|unicodecsv|0.14.1|
|jupyter_events|0.8.0|unidecode|1.2.0|
|jupyter_server|2.10.0|unixodbc|2.3.11|
|jupyter_server_terminals|0.4.4|urllib3|2.1.0|
|jupyterlab|4.0.11|utf8proc|2.6.1|
|jupyterlab_pygments|0.1.2|virtualenv|20.26.1|
|jupyterlab_server|2.25.1|wcwidth|0.2.5|
|jupyterlab_widgets|3.0.10|webencodings|0.5.1|
|jxrlib|1.1|websocket-client|0.58.0|
|kernel-headers_linux-64|3.10.0|werkzeug|2.3.8|
|keyring|24.3.1|wheel|0.41.2|
|kiwisolver|1.4.4|whichcraft|0.6.1|
|krb5|1.20.1|widgetsnbextension|4.0.10|
|lazy-object-proxy|1.6.0|wrapt|1.14.1|
|lazy_loader|0.3|xgboost|2.0.3|
|lcms2|2.12|xlrd|2.0.1|
|ld_impl_linux-64|2.38|xlsxwriter|3.1.1|
|lerc|3.0|xlwt|1.3.0|
|liac-arff|2.5.0|xmltodict|0.13.0|
|libaec|1.0.4|xxhash|0.8.0|
|libarchive|3.6.2|xyzservices|2022.9.0|
|libavif|0.11.1|xz|5.4.6|
|libboost|1.82.0|yaml|0.2.5|
|libbrotlicommon|1.0.9|yaml-cpp|0.8.0|
|libbrotlidec|1.0.9|yapf|0.40.2|
|libbrotlienc|1.0.9|yarl|1.9.3|
|libclang|14.0.6|zeromq|4.3.5|
|libclang13|14.0.6|zfp|1.0.0|
|libcups|2.4.2|zict|3.0.0|
|libcurl|8.5.0|zipp|3.17.0|
|libdeflate|1.17|zlib|1.2.13|
|libedit|3.1.20230828|zlib-ng|2.0.7|
|libev|4.33|zope|1.0|
|libevent|2.1.12|zope.event|5.0|
|libffi|3.4.4|zope.interface|5.4.0|
|libgcc-devel_linux-64|11.2.0|zstandard|0.19.0|
|libgcc-ng|11.2.0|zstd|1.5.5|
|libgd|2.3.3|absl-py|2.1.0|
|libgfortran-ng|11.2.0|accelerate|0.30.1|
|libgfortran5|11.2.0|adlfs|2024.2.0|
|libglib|2.78.4|alembic|1.13.2|
|libgomp|11.2.0|astor|0.8.1|
|libiconv|1.16|azure-core|1.30.2|
|liblief|0.12.3|azure-datalake-store|0.0.53|
|libllvm14|14.0.6|azure-storage-blob|12.22.0|
|libmamba|1.5.6|azure-storage-file-datalake|12.16.0|
|libmambapy|1.5.6|azureml-synapse|0.0.1|
|libnghttp2|1.57.0|chat-magics|0.1.25.2.28|
|libpng|1.6.39|chat-magics-fabric|0.2.0.25.8.13|
|libpq|12.17|colorlog|6.8.2|
|libprotobuf|3.20.3|control-script|1.0.3|
|librsvg|2.54.4|convertdate|2.4.0|
|libsodium|1.0.18|dash|2.17.1|
|libsolv|0.7.24|dash-core-components|2.0.0|
|libspatialindex|1.9.3|dash-cytoscape|1.0.2|
|libssh2|1.10.0|dash-html-components|2.0.0|
|libstdcxx-devel_linux-64|11.2.0|dash-table|5.0.0|
|libstdcxx-ng|11.2.0|docker|7.0.0|
|libthrift|0.15.0|ds-copilot|0.1.25.2.28|
|libtiff|4.5.1|dscopilot-installer|0.0.7|
|libtool|2.4.6|fabric-connection|0.2.0|
|libuuid|1.41.5|filelock|3.11.0|
|libuv|1.44.2|flaml|2.5.0.post1|
|libwebp|1.3.2|flt-python|0.18.2|
|libwebp-base|1.3.2|fluent-logger|0.10.0|
|libxcb|1.15|fsspec|2024.6.1|
|libxgboost|2.0.3|geoanalytics-fabric|1.0.0|
|libxkbcommon|1.0.1|gson|0.0.4|
|libxml2|2.10.4|hcrystalball|0.1.10|
|libxslt|1.1.37|**impulse-python-handler**|**1.3.198470504 ⬆️ 1.4.208330617**|
|libzopfli|1.0.3|interpret|0.6.0|
|lightgbm|4.3.0|interpret-core|0.6.0|
|lightning-utilities|0.9.0|joblibspark|0.5.2|
|llvm-openmp|14.0.6|json-tricks|3.17.3|
|llvmlite|0.42.0|jupyter-ui-poll|1.0.0|
|locket|1.0.0|kqlmagiccustom|0.1.115+fabric.post26|
|lxml|4.9.3|library-metadata-cooker|3.6.0.1|
|lz4|4.3.2|lunardate|0.2.2|
|lz4-c|1.9.4|mako|1.3.5|
|lzo|2.10|mypy|1.4.1|
|make|4.2.1|nni|3.0|
|markdown|3.4.1|notebookutils|1.1.13.35.20260208.7|
|markdown-it-py|2.2.0|nvidia-ml-py|12.560.30|
|markupsafe|2.1.3|optuna|3.6.1|
|matplotlib|3.8.0|pandasnet|1.0|
|matplotlib-base|3.8.0|powerbiclient|3.1.1|
|matplotlib-inline|0.1.6|prose-pandas2pyspark|10.5.0rc2024121001|
|mccabe|0.7.0|prose-suggestions|10.4.1|
|mdurl|0.1.0|py4j|0.10.9.7|
|menuinst|2.0.2|pyluach|2.2.0|
|minio|7.1.0|pymeeus|0.5.12|
|mistune|2.0.4|pyperclip|1.8.2|
|mkl|2023.1.0|pyspark|3.5.1.5.4.20240407|
|mkl-service|2.4.0|pythonwebhdfs|0.2.3|
|mkl_fft|1.3.8|responses|0.25.3|
|mkl_random|1.2.4|retrying|1.3.4|
|mlflow-skinny|2.12.2|rgf-python|3.12.0|
|mock|4.0.3|rouge-score|0.1.2|
|more-itertools|10.1.0|salib|1.5.0|
|mpc|1.1.0|schema|0.7.7|
|mpfr|4.0.2|semantic-link-sempy|0.11.0|
|mpi|1.0|seqeval|1.2.2|
|mpich|4.1.1|simplejson|3.19.3|
|mpmath|1.3.0|spark-mssql-connector-fabric35|1.0.0|
|msal|2023.12.01|sqlanalyticsfabricconnectorpy|1.0.1|
|msal-extensions|2023.12.01|synapseml|1.1.1|
|msgpack-python|1.0.3|synapseml-internal|1.1.1.0|
|msrest|2023.12.01|synapseml-mlflow|1.0.31|
|multidict|6.0.4|synapseml-utils|1.1.6.post2|
|multipledispatch|0.6.0|tensorboardx|2.6.2.2|
|multiprocess|0.70.15|thop|0.1.1-2209072238|
|munkres|1.1.4|typeguard|4.1.2|
|mypy_extensions|1.0.0|websockets|12.0|
|mysql|5.7.24|workalendar|17.0.0|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|junit-jupiter-params|5.5.2|
|JLargeArrays|1.5|junit-platform-commons|1.5.2|
|JTransforms|3.1|junit-platform-engine|1.5.2|
|RoaringBitmap|0.9.45|juniversalchardet|2.4.0|
|ST4|4.0.4|kafka-clients|3.4.1|
|**SparkCustomEvents**|**3.5.0-1.0.16 ⬆️ 3.5.0-1.0.17**|kryo-shaded|4.0.2|
|TokenLibrary-assembly|4.3.8|**kusto-spark**|**3.0_2.12-5.2.2-SNAPSHOT ⬆️ 3.0_2.12-7.0.4**|
|VPaaSConnector|3.5.01|lapack|3.0.3|
|VegasConnector|3.5.10|leveldbjni-all|1.8|
|activation|1.1.1|libfb303|0.9.3|
|**aircompressor**|**0.27 ⬆️ 2.0.3**|libthrift|0.12.0|
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
|**arrow-memory-unsafe**|**12.0.1**|metrics-servlets|4.2.10|
|arrow-vector|12.0.1|metrics4-scala|2.12-4.2.9|
|audience-annotations|0.5.0|**microsoft-catalog-metastore-client**|**1.1.21 ⬆️ 1.1.28**|
|avro|1.11.4|microsoft-log4j-etwappender|1.0|
|avro-ipc|1.11.4|minlog|1.3.0|
|avro-mapred|1.11.4|mlflow-spark|2.12-2.11.3|
|aws-java-sdk-bundle|1.12.262|mysql-connector-java|8.0.18|
|azure-core|1.47.0|**netty-all**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-core-http-netty|1.14.1|**netty-buffer**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-data-lake-store-sdk|2.3.9|**netty-codec**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-eventhubs|3.3.0|netty-codec-dns|4.1.101.Final|
|azure-eventhubs-spark|2.12-2.3.22|**netty-codec-http**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-json|1.1.0|**netty-codec-http2**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-keyvault-core|1.0.0|**netty-codec-socks**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-storage|7.0.1|**netty-common**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-storage-blob|12.25.3|**netty-handler**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-storage-common|12.24.3|**netty-handler-proxy**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|azure-storage-internal-avro|12.10.3|**netty-resolver**|**4.1.96.Final ⬆️ 4.1.124.Final**|
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
|commons-codec|1.16.1|**netty-transport**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|commons-collections|3.2.2|**netty-transport-classes-epoll**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|commons-collections4|4.4|**netty-transport-classes-kqueue**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|commons-compiler|3.1.9|**netty-transport-native-epoll**|**4.1.96.Final-linux-aarch_64 ⬆️ 4.1.124.Final-linux-aarch_64**|
|commons-compress|1.23.0|**netty-transport-native-epoll**|**4.1.96.Final-linux-aarch_64 ⬆️ 4.1.124.Final-linux-riscv64**|
|commons-crypto|1.1.0|**netty-transport-native-epoll**|**4.1.96.Final-linux-aarch_64 ⬆️ 4.1.124.Final-linux-x86_64**|
|commons-dbcp|1.4|**netty-transport-native-kqueue**|**4.1.96.Final-osx-aarch_64 ⬆️ 4.1.124.Final-osx-aarch_64**|
|commons-io|2.11.0|**netty-transport-native-kqueue**|**4.1.96.Final-osx-aarch_64 ⬆️ 4.1.124.Final-osx-x86_64**|
|commons-io|2.18.0|**netty-transport-native-unix-common**|**4.1.96.Final ⬆️ 4.1.124.Final**|
|commons-lang|2.6|nimbus-jose-jwt|9.37.2|
|commons-lang3|3.12.0|notebook-utils|1.1.13-spark35-20260208.7|
|commons-logging|1.1.3|objenesis|3.3|
|commons-math3|3.6.1|onnx-protobuf|2.12-0.9.3|
|commons-pool|1.5.4|onnxruntime_gpu|1.8.1|
|commons-pool2|2.11.1|opencsv|2.3|
|commons-text|1.10.0|opencv|3.2.0-1|
|compress-lzf|1.1.2|openlineage-spark|2.12-1.26.0|
|curator-client|2.13.0|opentest4j|1.2.0|
|curator-framework|2.13.0|opentracing-api|0.33.0|
|curator-recipes|2.13.0|opentracing-noop|0.33.0|
|datanucleus-api-jdo|4.2.4|opentracing-util|0.33.0|
|datanucleus-core|4.1.17|orc-core|1.9.5-shaded-protobuf|
|datanucleus-rdbms|4.1.19|orc-mapreduce|1.9.5-shaded-protobuf|
|datasketches-java|3.3.0|orc-shims|1.9.5|
|datasketches-memory|2.1.0|oro|2.0.8|
|**delta-kernel-api**|**3.2.1.20260209.3 ⬆️ 3.2.1.20260303.1**|osgi-resource-locator|1.0.3|
|**delta-kernel-defaults**|**3.2.1.20260209.3 ⬆️ 3.2.1.20260303.1**|paranamer|2.8|
|**delta-spark**|**2.12-3.2.1.20260209.3 ⬆️ 2.12-3.2.1.20260303.1**|parquet-column|1.13.1|
|**delta-storage**|**3.2.1.20260209.3 ⬆️ 3.2.1.20260303.1**|parquet-common|1.13.1|
|derby|10.14.2.0|parquet-encoding|1.13.1|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|parquet-format-structures|1.13.1|
|fastutil|7.0.2|**parquet-hadoop-ms**|**3.5.5.5.4.20260211.1 ⬆️ 3.5.5.5.4.20260312.6**|
|flatbuffers-java|1.12.0|parquet-jackson|1.13.1|
|flt-spark-sql-extensions|0.18.2|pickle|1.3|
|fluent-logger|0.3.4-jar-with-dependencies-provided|postgresql|42.2.9|
|gcs-connector-hadoop3|2.2.14-shaded|profiler|1.1.1|
|**genesis-client**|**2.12-0.36.3-jar-with-dependencies ⬆️ 2.12-0.37.0-jar-with-dependencies**|proton-j|0.33.8|
|geoanalytics-fabric|2.12-1.0.0-msfabric-1.3|py4j|0.10.9.7|
|**gluten-velox-bundle-spark**|**2.12-mariner_2.0_x86_64-1.3.0-20260209.3 ⬆️ 2.12-mariner_2.0_x86_64-1.3.0-20260303.5**|qpid-proton-j-extensions|1.2.4|
|gson|2.8.9|reactive-streams|1.0.3|
|guava|14.0.1|reactor-core|3.4.34|
|h3|4.1.1|reactor-netty-core|1.0.40|
|**hadoop-aliyun**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|reactor-netty-http|1.0.40|
|**hadoop-annotations**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|rocksdbjni|8.3.2|
|**hadoop-aws**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scala-collection-compat|2.12-2.7.0|
|**hadoop-azure**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scala-compiler|2.12.18|
|**hadoop-azure-datalake**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scala-java8-compat|2.12-0.9.0|
|hadoop-azureml|1.0-fs|scala-library|2.12.18|
|**hadoop-client-api**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scala-parser-combinators|2.12-2.3.0|
|**hadoop-client-runtime**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scala-reflect|2.12.18|
|**hadoop-cloud-storage**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scala-xml|2.12-2.1.0|
|**hadoop-openstack**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scalactic|2.12-3.2.14|
|hadoop-shaded-guava|1.1.1|scalatra|2.12-3.0.0-M1|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.4.20260211.1 ⬆️ 3.3.4.5.4.20260312.6**|scalatra-common|2.12-3.0.0-M1|
|**hdinsight-spark-metrics**|**3.5.0-1.0.16 ⬆️ 3.5.0-1.0.17**|scalatra-metrics|2.12-3.0.0-M1|
|hive-common|2.3.9|shims|0.9.45|
|hive-exec|2.3.9-core|slf4j-api|2.0.7|
|hive-llap-common|2.3.9|snappy-java|1.1.10.5|
|hive-metastore|2.3.9|spark|3.5-advisor-core_2.12-1.0.18|
|hive-serde|2.3.9|spark|3.5-rpc-history-server-app-listener_2.12-1.0.0|
|hive-shims|0.23-2.3.9|spark|3.5-rpc-history-server-core_2.12-1.0.0|
|hive-shims|2.3.9|spark-avro|2.12-3.5.0|
|hive-shims-common|2.3.9|**spark-avro**|**2.12-3.5.0 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|hive-shims-scheduler|2.3.9|**spark-catalyst**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|hive-storage-api|2.8.1|**spark-common-utils**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|hk2-api|2.6.1|**spark-core**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|hk2-locator|2.6.1|**spark-enhancement**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|hk2-utils|2.6.1|spark-enhancementui|2.12-3.3.0|
|httpclient|4.5.14|spark-eventstream-extensions|1.0.5|
|httpclient5|5.1.3|spark-excel-thin|2.12-3.5.6_0.31.2|
|httpcore|4.4.16|**spark-graphx**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|httpmime|4.5.13|**spark-hadoop-cloud**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|httpmime|4.5.14|**spark-hive**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|**impulse-core_spark**|**2.12-1.3.198470504 ⬆️ 2.12-1.4.208330617**|spark-jobinsight|2.12-1.0.0-spark3.5|
|**impulse-exception_java11**|**2.12-1.3.198470504 ⬆️ 2.12-1.4.208330617**|**spark-kusto-synapse-connector**|**3.5_2.12-1.5.1 ⬆️ 3.5_2.12-2.0.2**|
|**impulse-telemetry-common**|**2.12-1.4.208330617**|**spark-kvstore**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|**impulse-telemetry-mds_spark**|**2.12-1.3.198470504 ⬆️ 2.12-1.4.208330617**|**spark-launcher**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|ini4j|0.5.4|spark-lighter-contract|2.12-2.1.0_spark-3.5.1_20240717.4|
|isolation-forest|3.5.0_2.12-3.0.5|spark-lighter-core|2.12-2.0.11_spark-3.5.1_20240717.4|
|istack-commons-runtime|3.0.8|**spark-microsoft-tools**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|ivy|2.5.1|**spark-mllib**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-annotations|2.15.2|**spark-mllib-local**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-core|2.15.2|**spark-mssql-connector-fabric35**|**1.6.9 ⬆️ 1.6.10**|
|jackson-core-asl|1.9.13|**spark-network-common**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-databind|2.15.2|**spark-network-shuffle**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-dataformat-cbor|2.15.2|**spark-onesecurity-client**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-dataformat-xml|2.12.7|**spark-onesecurity-common**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-datatype-jsr310|2.15.2|**spark-onesecurity-server**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-mapper-asl|1.9.13|**spark-repl**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-module-jaxb-annotations|2.15.2|**spark-sketch**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jackson-module-scala|2.12-2.15.2|**spark-sql**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.activation-api|1.2.2|**spark-sql-api**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.annotation-api|1.3.5|**spark-sql-kafka**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.inject|2.6.1|**spark-streaming**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.servlet-api|4.0.3|**spark-streaming-kafka**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.validation-api|2.0.2|**spark-tags**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.ws.rs-api|2.1.6|**spark-token-provider-kafka**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|jakarta.xml.bind-api|2.3.2|**spark-unsafe**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|janino|3.1.9|spark-xml|2.12-0.17.0|
|javassist|3.29.2-GA|**spark-yarn**|**2.12-3.5.5.5.4.20260211.1 ⬆️ 2.12-3.5.5.5.4.20260312.6**|
|javatuples|1.2|**spark_diagnostic_cli**|**2.1.7_spark-3.5.1_20250901.3-shaded ⬆️ 2.2.0_spark-3.5.1_20260223.3-shaded**|
|javax.jdo|3.2.0-m3|sparklyr-connector|3.5.1-1.0.0267535|
|javolution|5.5.1|**sparknativeparquetwriter**|**2.12-1.3.0-20250828.2 ⬆️ 2.12-1.3.0-20260304.4**|
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
|jersey-hk2|2.40|synapseml-cognitive|2.12-1.1.1|
|jersey-server|2.40|synapseml-core|2.12-1.1.1|
|jettison|1.1|synapseml-deep-learning|2.12-1.1.1|
|jetty-util|9.4.57.v20241219|synapseml-internal|2.12-1.1.1.0|
|jetty-util-ajax|9.4.57.v20241219|synapseml-lightgbm|2.12-1.1.1|
|jline|2.14.6|synapseml-opencv|2.12-1.1.1|
|joda-time|2.12.5|synapseml-vw|2.12-1.1.1|
|jodd-core|3.5.2|synfs|1.1.13-spark35-20260208.7|
|jsch|0.1.54|threeten-extra|1.7.1|
|json|1.8|tink|1.9.0|
|json|20231013|transaction-api|1.1|
|json-simple|1.1.1|transform-token-provider-utils|0.3.0|
|json-simple|1.1|**trident-core**|**1.3.2 ⬆️ 1.3.4**|
|json4s-ast|2.12-3.7.0-M11|**tridenttokenlibrary-assembly**|**1.10.4 ⬆️ 1.11.2**|
|json4s-core|2.12-3.7.0-M11|univocity-parsers|2.9.1|
|json4s-jackson|2.12-3.7.0-M11|vw-jni|9.3.0|
|json4s-scalap|2.12-3.7.0-M11|wildfly-openssl|1.0.7.Final|
|jsr305|3.0.0|woodstox-core|6.2.4|
|jta|1.1|xbean-asm9-shaded|4.23|
|jul-to-slf4j|2.0.7|xz|1.9|
|junit-jupiter|5.5.2|**zookeeper**|**3.6.3.5.4.20260211.1 ⬆️ 3.6.3.5.4.20260312.6**|
|junit-jupiter-api|5.5.2|**zookeeper-jute**|**3.6.3.5.4.20260211.1 ⬆️ 3.6.3.5.4.20260312.6**|
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
|V8|5.0.0|notebookutils|1.1.13.35.20260208.7|
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

