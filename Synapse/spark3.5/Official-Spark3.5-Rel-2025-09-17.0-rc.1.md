# System Environment
*   **Product**: Synapse Spark 3.5
*   **VHD Name**: 42780494f2ba25.vhd
*   **Vhd Release**: Spark3.5-Rel-2025-09-17.0-rc.1
*   **Operating System**: Azure Linux 3.0
*   **Apache Spark**: 3.5.5
*   **Java**: 11.0.28
*   **Scala**: 2.12.18
*   **Python**: 3.11/1.0.0
*   **Delta Lake**: 3.2.0.20250917.1

# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1805912|Delta/spark35:3.2.0.20250917.1|Delta 3.2.0.20250917.1 brings improvements over the previous version.|
|1797793|Wildfire:1.11.1|Upgrade to spark 3.5.5 and other changes.|
|1797823|ServiceConfigurationTemplates:spark/3.5.0|Increase spark.yarn.am.waitTime to ensure spark context has enough time for initialization.|
|1802442|Wildfire/spark35:1.11.2|Reuse exchange fix. Reuse exchange was not happening in spark 3.5|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1786730|Wildfire/spark35:1.11.3|Improvement in internal logs to identify spark submit failures.|
|1788476|SparkDiagnosticsLibrary:1.0.32|Runtime environment dependency management stability improvement for module upgrades|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|AutoscaleProbe|3.9.5|OneLakeClientStarter|1.0.25|
|AzureMLExtensions|1.0.4|OnelakeSparkCatalog|0.2.7|
|Conda|2.0.0|PostgreSQLJDBCDriver|1.0.3|
|CosmosDBConnector|2.2.5|Python|3.11/1.0.0|
|CSparkMetricUpdate|1.0.11|R|1.0.0|
|**Delta**|**3.2.0.21 ⬆️ 3.2.0.20250917.1**|SparkAdvisor|1.0.5|
|DSCopilot|1.3.0|**SparkDiagnosticsLibrary**|**1.0.31 ⬆️ 1.0.32**|
|DSCopilotInstaller|1.0.0|SparkJobInsight|1.0.0|
|DWConnector|1.0.0|SparkLighter|2.0.4|
|EventHubConnector|2.3.27|SparkLineage|1.26.3|
|ExternalHiveMetastoreLibraries|0.0.7|SparklyrConnector|2.0.1|
|FabricDWConnector|1.0.13|SparkNativeParquetWriter|0.40.0|
|FLTSparkUtils|1.0.1|SparkRPCHistoryServer|1.6.0|
|FsspecWrapper|0.1.14|SparkSqlConnector|1.6.9|
|Genesis|0.33.1|SQLServerODBCDriver|18.1.0|
|GlutenUI|1.0.8|SStreamOnSparkJar|2.4.1|
|HiveMetaStoreClient|1.1.21.2|TokenLibrary|4.3.8|
|Impulse|1.0.30|TridentCore|1.2.23|
|KustoConnector|1.5.2|TridentTokenLibrary|1.9.10|
|LibraryManager|1.0.2|Vegas|3.5.09.07|
|LibraryMetadataCooker|1.0.0|**Wildfire**|**1.11.0.1 ⬆️ 1.11.3**|
|MlflowLibrary|2.11.3.1|
|MMLSpark|1.0.10|
|MySQLJavaConnector|1.0.3|
|NotebookUtils|1.1.60|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_libgcc_mutex|0.1|mccabe|0.7.0|
|_openmp_mutex|5.1|mdurl|0.1.0|
|_py-xgboost-mutex|2.0|menuinst|2.2.0|
|adal|1.2.7|mesa-libegl-cos6-x86_64|11.0.7|
|adlfs|2024.12.0|minizip|4.0.3|
|aiohappyeyeballs|2.4.4|mistune|3.1.2|
|aiohttp|3.11.10|mkl|2023.1.0|
|aiosignal|1.2.0|mkl-service|2.4.0|
|alabaster|0.7.16|mkl_fft|1.3.11|
|anyio|4.6.2|mkl_random|1.2.8|
|aom|3.6.0|mlflow-skinny|2.18.0|
|aplr|10.9.0|mltable|1.6.1|
|appdirs|1.4.4|mock|4.0.3|
|applicationinsights|0.11.10|more-itertools|10.3.0|
|archspec|0.2.3|mpc|1.3.1|
|argcomplete|3.6.2|mpfr|4.2.1|
|argon2-cffi|21.3.0|mpi|1.0|
|argon2-cffi-bindings|21.2.0|mpich|4.1.1|
|arrow|1.3.0|mpmath|1.3.0|
|arrow-cpp|19.0.0|msal|1.33.0|
|asgiref|3.8.1|msal|2025.03.01|
|asn1crypto|1.5.1|msal-extensions|2025.03.01|
|astropy|7.0.0|msgpack-python|1.0.3|
|astropy-iers-data|0.2025.1.13.0.34.51|msrest|2025.03.01|
|asttokens|2.0.5|msrestazure|0.6.4.post1|
|asttokens|3.0.0|multidict|6.1.0|
|async-lru|2.0.4|multipledispatch|0.6.0|
|async-timeout|5.0.1|multiprocess|0.70.15|
|async_generator|1.10|mypy|1.4.1|
|attrs|24.3.0|mypy-extensions|1.1.0|
|autopep8|2.0.4|mypy_extensions|1.0.0|
|aws-c-auth|0.6.19|mysql|8.4.0|
|aws-c-cal|0.5.20|narwhals|1.31.0|
|aws-c-common|0.8.5|nbclassic|1.1.0|
|aws-c-compression|0.2.16|nbclient|0.10.2|
|aws-c-event-stream|0.2.15|nbconvert|7.16.6|
|aws-c-http|0.6.25|nbconvert-core|7.16.6|
|aws-c-io|0.13.10|nbconvert-pandoc|7.16.6|
|aws-c-mqtt|0.7.13|nbformat|5.10.4|
|aws-c-s3|0.1.51|ncurses|6.4|
|aws-c-sdkutils|0.1.6|ncurses|6.5|
|aws-checksums|0.1.13|ndg-httpsclient|0.5.1|
|aws-crt-cpp|0.18.16|nest-asyncio|1.6.0|
|aws-sdk-cpp|1.11.212|networkx|3.4.2|
|azure-ai-ml|1.28.1|nlohmann_json|3.11.2|
|azure-common|1.1.28|nltk|3.9.1|
|azure-core|1.35.0|nose|1.3.7|
|azure-core-tracing-opentelemetry|1.0.0b12|notebook|7.3.2|
|azure-datalake-store|0.0.53|notebook-shim|0.2.4|
|azure-graphrbac|0.61.2|notebookutils|1.1.11.35|
|azure-identity|2025.03.01|nspr|4.35|
|azure-keyvault|2025.03.01|nss|3.89.1|
|azure-mgmt|2025.03.01|numba|0.61.0|
|azure-mgmt-authorization|4.0.0|numexpr|2.10.1|
|azure-mgmt-containerregistry|10.3.0|numpy|1.26.4|
|azure-mgmt-core|1.6.0|numpy|2.3.3|
|azure-mgmt-keyvault|10.3.1|numpy-base|1.26.4|
|azure-mgmt-network|29.0.0|numpydoc|1.7.0|
|azure-mgmt-resource|24.0.0|oauthlib|3.2.2|
|azure-mgmt-storage|23.0.0|ocl-icd|2.3.2|
|azure-monitor-opentelemetry|1.7.0|olefile|0.46|
|azure-monitor-opentelemetry-exporter|1.0.0b41|onnx|1.18.0|
|azure-storage|2025.03.01|openjpeg|2.5.2|
|azure-storage-blob|12.19.0|openldap|2.6.4|
|azure-storage-file-datalake|12.14.0|openpyxl|3.1.5|
|azure-storage-file-share|12.22.0|openssl|3.0.17|
|azureml-core|1.60.0|openssl|3.0.16|
|azureml-dataprep|5.1.6|opentelemetry-api|1.36.0|
|azureml-dataprep-native|41.0.0|opentelemetry-instrumentation|0.57b0|
|azureml-dataprep-rslex|2.22.5|opentelemetry-instrumentation-asgi|0.57b0|
|azureml-mlflow|1.60.0|opentelemetry-instrumentation-dbapi|0.57b0|
|azureml-synapse|0.0.1|opentelemetry-instrumentation-django|0.57b0|
|babel|2.16.0|opentelemetry-instrumentation-fastapi|0.57b0|
|backports|1.1|opentelemetry-instrumentation-flask|0.57b0|
|backports.functools_lru_cache|1.6.4|opentelemetry-instrumentation-psycopg2|0.57b0|
|backports.shutil_get_terminal_size|1.0.0|opentelemetry-instrumentation-requests|0.57b0|
|backports.tempfile|1.0|opentelemetry-instrumentation-urllib|0.57b0|
|backports.weakref|1.0.post1|opentelemetry-instrumentation-urllib3|0.57b0|
|bcrypt|3.2.0|opentelemetry-instrumentation-wsgi|0.57b0|
|beautifulsoup4|4.12.3|opentelemetry-resource-detector-azure|0.1.5|
|binaryornot|0.4.4|opentelemetry-sdk|1.36.0|
|bitarray|2.5.1|opentelemetry-semantic-conventions|0.57b0|
|bkcharts|0.2|opentelemetry-util-http|0.57b0|
|black|24.10.0|orc|2.0.1|
|blas|1.0|overrides|7.4.0|
|bleach|6.2.0|packaging|24.2|
|blinker|1.9.0|packaging|25.0|
|blosc|1.21.3|pandas|2.2.3|
|bokeh|3.6.2|pandas|2.3.2|
|boltons|24.1.0|pandasql|0.7.3|
|boost-cpp|1.82.0|pandoc|2.12|
|boto|2.49.0|pandocfilters|1.5.0|
|bottleneck|1.4.2|paramiko|3.5.0|
|brotli|1.0.9|parso|0.8.4|
|brotli-bin|1.0.9|parso|0.8.5|
|brotli-python|1.0.9|partd|1.4.2|
|brunsli|0.1|patch|2.7.6|
|bzip2|1.0.8|patchelf|0.17.2|
|c-ares|1.19.1|path|16.2.0|
|c-blosc2|2.12.0|path.py|12.5.0|
|ca-certificates|2025.2.25|pathlib2|2.3.6|
|**ca-certificates**|**2025.2.25 ⬆️ 2025.9.9**|pathspec|0.10.3|
|cached-property|1.5.2|patsy|1.0.1|
|cachetools|5.5.1|pcre2|10.42|
|certifi|2025.1.31|pep8|1.7.1|
|certifi|2025.8.3|pexpect|4.9.0|
|cffi|2.0.0|pexpect|4.8.0|
|cffi|1.17.1|pickleshare|0.7.5|
|cfitsio|3.470|pillow|11.3.0|
|chardet|4.0.0|pillow|11.1.0|
|charls|2.2.0|pip|23.3.1|
|charset-normalizer|3.3.2|pip|25.0|
|charset-normalizer|3.4.3|pkginfo|1.11.2|
|click|8.1.7|platformdirs|4.4.0|
|cloudpickle|2.2.1|platformdirs|3.10.0|
|clr_loader|0.2.7.post0|plotly|6.0.1|
|cmake|3.31.2|pluggy|1.5.0|
|colorama|0.4.6|ply|3.11|
|comm|0.2.3|portalocker|2.10.1|
|comm|0.2.1|powerbiclient|3.1.1|
|conda-package-handling|2.4.0|prettytable|3.5.0|
|conda-package-streaming|0.11.0|prometheus_client|0.21.0|
|conda-verify|3.4.2|prompt-toolkit|3.0.43|
|contextlib2|21.6.0|prompt-toolkit|3.0.52|
|contourpy|1.3.3|prompt_toolkit|3.0.43|
|contourpy|1.3.1|propcache|0.2.0|
|control-script|1.0.3|protobuf|4.25.3|
|cookiecutter|2.6.0|psutil|5.9.0|
|cpp-expected|1.1.0|**psutil**|**5.9.0 ⬆️ 7.1.0**|
|**cryptography**|**45.0.7 ⬆️ 46.0.1**|pthread-stubs|0.3|
|cryptography|44.0.1|ptyprocess|0.7.0|
|cuda-cudart|12.4.127|pure-eval|0.2.3|
|cuda-cudart_linux-64|12.4.127|pure_eval|0.2.2|
|cuda-cupti|12.4.127|py-cpuinfo|9.0.0|
|cuda-libraries|12.4.1|py-lief|0.12.3|
|cuda-nvrtc|12.4.127|py-xgboost|3.0.1|
|cuda-nvtx|12.4.127|py4j|0.10.9.7|
|cuda-opencl|12.4.127|pyarrow|19.0.0|
|cuda-runtime|12.4.1|pyasn1|0.6.1|
|cuda-version|12.4|pyasn1-modules|0.4.2|
|curl|8.12.1|pybind11-abi|4|
|cycler|0.12.1|pycodestyle|2.12.1|
|cycler|0.11.0|pycosat|0.6.6|
|cyrus-sasl|2.1.28|pycparser|2.21|
|cython|3.0.11|pycparser|2.23|
|cytoolz|1.0.1|pycurl|7.45.4|
|daal4py|2023.1.1|pydash|8.0.5|
|dal|2023.1.1|pydocstyle|6.3.0|
|dash|2.18.2|pyerfa|2.0.1.5|
|dash-core-components|2.0.0|pyflakes|3.2.0|
|dash-cytoscape|1.0.2|pygments|2.19.2|
|dash-html-components|2.0.0|pygments|2.15.1|
|dash-table|5.0.0|pyjwt|2.10.1|
|dask|2024.12.1|pynacl|1.5.0|
|dask-core|2024.12.1|pyodbc|5.2.0|
|dask-expr|1.1.21|pyopenssl|25.0.0|
|databricks-sdk|0.33.0|**pyparsing**|**3.2.3 ⬆️ 3.2.4**|
|dataclasses|0.8|pyparsing|3.2.0|
|datasets|3.3.2|pyperclip|1.9.0|
|dav1d|1.2.1|pyqt|6.7.1|
|dbus|1.13.18|pyqt6-sip|13.9.1|
|**debugpy**|**1.8.16 ⬆️ 1.8.17**|pyrsistent|0.20.0|
|debugpy|1.8.11|pysocks|1.7.1|
|decorator|5.2.1|pyspark|3.5.1.5.4.20240407|
|decorator|5.1.1|pyspark|20240404|
|defusedxml|0.7.1|pytables|3.10.2|
|deprecated|1.2.13|pytest|8.3.4|
|dill|0.3.8|python|3.11.13|
|distlib|0.3.8|python|3.11.11|
|distributed|2024.12.1|python-dateutil|2.9.0post0|
|distro|1.9.0|python-dateutil|2.9.0.post0|
|django|5.1.3|python-fastjsonschema|2.20.0|
|docker-py|7.1.0|python-json-logger|3.2.1|
|docutils|0.18.1|python-libarchive-c|5.1|
|entrypoints|0.4|python-lmdb|1.6.2|
|et_xmlfile|1.1.0|python-slugify|5.0.2|
|executing|2.2.1|python-tzdata|2023.3|
|executing|0.8.3|python-xxhash|3.5.0|
|expat|2.7.1|pythonnet|3.0.1|
|expat|2.6.4|pytorch|2.5.1|
|fastcache|1.1.0|pytorch-cuda|12.4|
|filelock|3.13.1|pytorch-mutex|1.0|
|fixedint|0.1.6|pytz|2024.1|
|flake8|7.1.1|pytz|2025.2|
|flask|3.0.3|pywavelets|1.8.0|
|flit|3.9.0|pyyaml|6.0.2|
|flit-core|3.9.0|pyzmq|26.2.0|
|fluent-logger|0.10.0|pyzmq|27.1.0|
|fmt|9.1.0|qdarkstyle|3.2.3|
|fontconfig|2.14.1|qstylizer|0.2.2|
|**fonttools**|**4.59.2 ⬆️ 4.60.0**|qt|6.7.2|
|fonttools|4.55.3|qt-main|6.7.2|
|freetype|2.12.1|qt5compat|6.7.2|
|frozendict|2.4.2|qtawesome|1.3.1|
|frozenlist|1.5.0|qtbase|6.7.2|
|fsspec|2024.12.0|qtconsole|5.6.1|
|fsspec_wrapper|0.1.14|qtdeclarative|6.7.2|
|future|1.0.0|qtimageformats|6.7.2|
|geographiclib|2.0|qtpy|2.4.1|
|geopy|2.4.1|qtshadertools|6.7.2|
|get_terminal_size|1.0.0|qtsvg|6.7.2|
|gevent|23.9.1|qttools|6.7.2|
|gflags|2.2.2|qttranslations|6.7.2|
|giflib|5.2.2|qtwebchannel|6.7.2|
|gitdb|4.0.12|qtwebengine|6.7.2|
|gitpython|3.1.43|qtwebsockets|6.7.2|
|glib|2.78.4|re2|2022.04.01|
|glib-tools|2.78.4|readline|8.2|
|glob2|0.7|readline|8.3|
|glog|0.5.0|referencing|0.30.2|
|gmp|6.3.0|regex|2024.11.6|
|gmpy2|2.2.1|reproc|14.2.4|
|google-auth|2.38.0|reproc-cpp|14.2.4|
|greenlet|3.1.1|requests|2.32.3|
|h11|0.14.0|requests|2.32.5|
|hdf5|1.14.5|requests-oauthlib|2.0.0|
|heapdict|1.0.1|retrying|1.4.2|
|html5lib|1.1|rfc3339-validator|0.1.4|
|httpcore|1.0.2|rfc3986-validator|0.1.1|
|httpx|0.27.0|rhash|1.4.3|
|huggingface_hub|0.29.2|rich|13.9.4|
|humanfriendly|10.0|ripgrep|14.1.0|
|icu|73.1|rpds-py|0.22.3|
|idna|3.7|rsa|4.7.2|
|idna|3.10|rtree|1.0.1|
|imagecodecs|2024.9.22|ruamel.yaml|0.18.6|
|imageio|2.37.0|ruamel.yaml.clib|0.2.8|
|imagesize|1.4.1|ruamel_yaml|0.17.21|
|importlib-metadata|8.5.0|s2n|1.3.27|
|importlib_metadata|8.5.0|safetensors|0.5.3|
|impulse-python-handler|1.0.30.1.0.0|salib|1.5.1|
|inflection|0.5.1|scikit-build|0.15.0|
|iniconfig|1.1.1|scikit-image|0.25.0|
|intel-openmp|2023.1.0|scikit-learn|1.6.1|
|interpret|0.7.2|scikit-learn-intelex|2023.1.1|
|interpret-core|0.7.2|scipy|1.15.1|
|intervaltree|3.1.0|seaborn|0.13.2|
|ipykernel|6.30.1|secretstorage|3.3.1|
|ipykernel|6.29.5|send2trash|1.8.2|
|ipython|9.5.0|setuptools|75.8.0|
|ipython|8.30.0|setuptools|78.1.1|
|ipython-pygments-lexers|1.1.1|shap|0.47.2|
|ipython_genutils|0.2.0|simdjson|3.10.1|
|ipywidgets|8.1.7|simplegeneric|0.8.1|
|ipywidgets|8.1.5|singledispatch|3.7.0|
|isodate|0.6.1|sip|6.10.0|
|itsdangerous|2.2.0|six|1.16.0|
|jaraco.classes|3.2.1|six|1.17.0|
|jedi|0.19.2|slicer|0.0.8|
|jeepney|0.7.1|smmap|5.0.2|
|jinja2|3.1.6|snappy|1.2.1|
|jmespath|1.0.1|sniffio|1.3.0|
|joblib|1.4.2|snowballstemmer|2.2.0|
|jpeg|9e|sortedcollections|2.1.0|
|json5|0.9.25|sortedcontainers|2.4.0|
|jsonpatch|1.33|soupsieve|2.5|
|jsonpickle|4.1.1|spark-mssql-connector-synapse35|1.0.0|
|jsonpointer|2.1|spdlog|1.11.0|
|jsonschema|4.23.0|sphinx|7.3.7|
|jsonschema-specifications|2023.7.1|sphinxcontrib|1.0|
|jupyter-client|8.6.3|sphinxcontrib-applehelp|1.0.2|
|jupyter-core|5.8.1|sphinxcontrib-devhelp|1.0.2|
|jupyter-lsp|2.2.0|sphinxcontrib-htmlhelp|2.0.0|
|jupyter-ui-poll|1.0.0|sphinxcontrib-jsmath|1.0.1|
|jupyter_client|8.6.3|sphinxcontrib-qthelp|1.0.3|
|jupyter_console|6.6.3|sphinxcontrib-serializinghtml|1.1.10|
|jupyter_core|5.7.2|sphinxcontrib-websupport|1.2.4|
|jupyter_events|0.12.0|sqlalchemy|2.0.37|
|jupyter_server|2.15.0|sqlanalyticsconnectorpy|1.0.1|
|jupyter_server_terminals|0.4.4|sqlite|3.45.3|
|jupyterlab|4.3.4|sqlite|3.50.2|
|jupyterlab-widgets|3.0.15|sqlparse|0.5.2|
|jupyterlab_pygments|0.3.0|stack-data|0.6.3|
|jupyterlab_server|2.27.3|stack_data|0.2.0|
|jupyterlab_widgets|3.0.13|statsmodels|0.14.4|
|jxrlib|1.1|strictyaml|1.7.3|
|keyring|24.3.1|sympy|1.13.3|
|kiwisolver|1.4.8|synapseml-cognitive|1.0.10.dev1|
|kiwisolver|1.4.9|synapseml-core|1.0.10.dev1|
|knack|0.12.0|synapseml-deep-learning|1.0.10.dev1|
|krb5|1.20.1|synapseml-internal|1.0.10.1.dev1|
|lazy-object-proxy|1.10.0|synapseml-lightgbm|1.0.10.dev1|
|lazy_loader|0.4|synapseml-opencv|1.0.10.dev1|
|lcms2|2.16|synapseml-vw|1.0.10.dev1|
|ld_impl_linux-64|2.40|tabulate|0.9.0|
|lerc|4.0.0|tbb|2021.8.0|
|liac-arff|2.5.0|tbb4py|2021.8.0|
|libabseil|20240116.2|tblib|1.7.0|
|libaec|1.1.3|terminado|0.17.1|
|libarchive|3.7.7|testpath|0.6.0|
|libavif|1.1.1|text-unidecode|1.3|
|libboost|1.82.0|textdistance|4.6.3|
|libbrotlicommon|1.0.9|threadpoolctl|3.5.0|
|libbrotlidec|1.0.9|tifffile|2024.12.12|
|libbrotlienc|1.0.9|tinycss2|1.4.0|
|libcublas|12.4.5.8|tk|8.6.15|
|libcufft|11.2.1.3|tk|8.6.14|
|libcufile|1.9.1.3|tokenizers|0.21.0|
|libcups|2.4.2|toml|0.10.2|
|libcurand|10.3.5.147|tomli|2.0.1|
|libcurl|8.12.1|tomli-w|1.2.0|
|libcusolver|11.6.1.9|toolz|1.0.0|
|libcusparse|12.3.1.170|torchdata|0.9.0|
|libdeflate|1.22|torchtriton|3.1.0|
|libedit|3.1.20230828|tornado|6.5.2|
|libev|4.33|tornado|6.4.2|
|libevent|2.1.12|tqdm|4.67.1|
|libffi|3.4.4|traitlets|5.14.3|
|libgcc-ng|11.2.0|transformers|4.49.0|
|libgfortran-ng|11.2.0|truststore|0.10.0|
|libgfortran5|11.2.0|typed-ast|1.5.5|
|libglib|2.78.4|typing-extensions|4.12.2|
|libgomp|11.2.0|typing-extensions|4.15.0|
|libgrpc|1.62.2|typing_extensions|4.12.2|
|libiconv|1.16|tzdata|2025a|
|liblief|0.12.3|tzdata|2025.2|
|libmamba|2.0.5|ujson|5.10.0|
|libmambapy|2.0.5|unicodecsv|0.14.1|
|libnghttp2|1.57.0|unicodedata2|15.1.0|
|libnpp|12.2.5.30|unidecode|1.3.8|
|libnvfatbin|12.4.127|unixodbc|2.3.11|
|libnvjitlink|12.4.127|urllib3|2.3.0|
|libnvjpeg|12.3.1.117|urllib3|2.5.0|
|libpng|1.6.39|utf8proc|2.6.1|
|libpq|17.4|virtualenv|20.28.0|
|libprotobuf|4.25.3|wcwidth|0.2.13|
|library-metadata-cooker|3.5.0.1|wcwidth|0.2.5|
|libsodium|1.0.18|webencodings|0.5.1|
|libsolv|0.7.30|websocket-client|1.8.0|
|libspatialindex|1.9.3|werkzeug|3.0.6|
|libssh2|1.11.1|wheel|0.45.1|
|libstdcxx-ng|11.2.0|whichcraft|0.6.1|
|libthrift|0.15.0|widgetsnbextension|4.0.13|
|libtiff|4.5.1|widgetsnbextension|4.0.14|
|libuuid|1.41.5|wrapt|1.17.0|
|libuv|1.48.0|xcb-util-cursor|0.1.4|
|libwebp-base|1.3.2|xgboost|3.0.1|
|libxcb|1.17.0|xlrd|2.0.1|
|libxcb|1.15|xlsxwriter|3.1.1|
|libxgboost|3.0.1|xlwt|1.3.0|
|libxkbcommon|1.0.1|xorg-libx11|1.8.12|
|libxml2|2.13.5|xorg-libxau|1.0.12|
|libxslt|1.1.41|xorg-libxdmcp|1.1.5|
|libzlib|1.3.1|xorg-xorgproto|2024.1|
|libzopfli|1.0.3|xxhash|0.8.0|
|lightgbm|4.6.0|xyzservices|2022.9.0|
|llvm-openmp|14.0.6|xz|5.6.4|
|llvmlite|0.44.0|yaml|0.2.5|
|locket|1.0.0|yaml-cpp|0.8.0|
|lxml|5.3.0|yapf|0.40.2|
|lz4|4.3.2|yarl|1.18.0|
|lz4-c|1.9.4|zeromq|4.3.5|
|lzo|2.10|zfp|1.0.0|
|make|4.2.1|zict|3.0.0|
|markdown|3.8|zipp|3.21.0|
|markdown-it-py|2.2.0|zlib|1.2.13|
|markupsafe|3.0.2|zlib|1.3.1|
|marshmallow|3.26.1|zlib-ng|2.0.7|
|matplotlib|3.10.6|zope|1.0|
|matplotlib|3.10.0|zope.event|5.0|
|matplotlib-base|3.10.0|zope.interface|7.1.1|
|matplotlib-inline|0.1.6|zstandard|0.23.0|
|matplotlib-inline|0.1.7|zstd|1.5.6|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|junit-platform-engine|1.5.2|
|JLargeArrays|1.5|juniversalchardet|2.4.0|
|JTransforms|3.1|kafka-clients|3.4.1|
|RoaringBitmap|0.9.45|kryo-shaded|4.0.2|
|ST4|4.0.4|kusto-spark|3.0_2.12-5.2.2-SNAPSHOT|
|SparkCustomEvents|3.5.0-1.0.11|lapack|3.0.3|
|TokenLibrary-assembly|4.3.8|leveldbjni-all|1.8|
|VegasConnector|3.5.09|libfb303|0.9.3|
|activation|1.1.1|libthrift|0.12.0|
|aircompressor|0.27|lightgbmlib|3.3.510|
|algebra|2.12-2.0.1|log4j|1.2-api-2.20.0|
|aliyun-java-sdk-core|4.5.10|log4j-api|2.20.0|
|aliyun-java-sdk-kms|2.11.0|log4j-core|2.20.0|
|aliyun-java-sdk-ram|3.1.0|log4j-slf4j2-impl|2.20.0|
|aliyun-sdk-oss|3.13.0|lz4-java|1.8.0|
|annotations|7.0.0|mdsdclientdynamic|2.0|
|antlr-runtime|3.5.2|metrics-core|4.2.19|
|antlr4-runtime|4.9.3|metrics-graphite|4.2.19|
|aopalliance-repackaged|2.6.1|metrics-healthchecks|4.2.9|
|apiguardian-api|1.1.0|metrics-jmx|4.2.19|
|arpack|3.0.3|metrics-json|4.2.19|
|arpack_combined_all|0.1|metrics-jvm|4.2.19|
|arrow-format|2.0.1|metrics-servlet|4.2.10|
|arrow-memory-core|2.0.1|metrics-servlets|4.2.10|
|arrow-memory-netty|2.0.1|metrics4-scala|2.12-4.2.9|
|arrow-vector|2.0.1|microsoft-catalog-metastore-client|1.1.21|
|audience-annotations|0.5.0|microsoft-log4j-etwappender|1.0|
|**avro**|**1.11.3 ⬆️ 1.11.4**|minlog|1.3.0|
|**avro-ipc**|**1.11.3 ⬆️ 1.11.4**|mlflow-spark|2.12-2.11.3|
|**avro-mapred**|**1.11.3 ⬆️ 1.11.4**|mysql-connector-java|8.0.18|
|aws-java-sdk-bundle|1.12.262|netty-all|4.1.96.Final|
|azure-core|1.47.0|netty-buffer|4.1.96.Final|
|azure-core-http-netty|1.14.1|netty-codec|4.1.96.Final|
|azure-cosmos-analytics-spark|5_2-12_synapse-2.2.5|netty-codec-dns|4.1.101.Final|
|azure-data-lake-store-sdk|2.3.9|netty-codec-http|4.1.96.Final|
|azure-eventhubs|3.3.0|netty-codec-http2|4.1.96.Final|
|azure-eventhubs-spark|2.12-2.3.22|netty-codec-socks|4.1.96.Final|
|azure-json|1.1.0|netty-common|4.1.96.Final|
|azure-keyvault-core|1.0.0|netty-handler|4.1.96.Final|
|azure-storage|7.0.1|netty-handler-proxy|4.1.96.Final|
|azure-storage-blob|2.25.3|netty-resolver|4.1.96.Final|
|azure-storage-common|2.24.3|netty-resolver-dns|4.1.101.Final|
|azure-storage-internal-avro|2.10.3|netty-resolver-dns-classes-macos|4.1.101.Final|
|azure-synapse-ml-pandas|2.12-0.1.1|netty-resolver-dns-native-macos|4.1.101.Final-osx-x86_64|
|blas|3.0.3|netty-tcnative-boringssl-static|2.0.62.Final-linux-x86_64|
|bonecp|0.8.0.RELEASE|netty-tcnative-boringssl-static|2.0.62.Final-windows-x86_64|
|breeze|2.12-2.1.0|netty-tcnative-boringssl-static|2.0.62.Final-osx-x86_64|
|breeze-macros|2.12-2.1.0|netty-tcnative-boringssl-static|2.0.62.Final-osx-aarch_64|
|cats-kernel|2.12-2.1.1|netty-tcnative-boringssl-static|2.0.62.Final-linux-aarch_64|
|chill|2.12-0.10.0|netty-tcnative-boringssl-static|2.0.62.Final|
|chill-java|0.10.0|netty-tcnative-classes|2.0.62.Final|
|client-sdk|1.24.1|netty-transport|4.1.96.Final|
|commons-cli|1.5.0|netty-transport-classes-epoll|4.1.96.Final|
|**commons-codec**|**1.16.0 ⬆️ 1.16.1**|netty-transport-classes-kqueue|4.1.96.Final|
|commons-collections|3.2.2|netty-transport-native-epoll|4.1.96.Final-linux-aarch_64|
|commons-collections4|4.4|netty-transport-native-epoll|4.1.96.Final-linux-x86_64|
|commons-compiler|3.1.9|netty-transport-native-kqueue|4.1.96.Final-osx-aarch_64|
|commons-compress|1.23.0|netty-transport-native-kqueue|4.1.96.Final-osx-x86_64|
|commons-crypto|1.1.0|netty-transport-native-unix-common|4.1.96.Final|
|commons-dbcp|1.4|notebook-utils|1.1.11-spark35|
|commons-io|2.11.0|objenesis|3.3|
|commons-io|2.18.0|onnx-protobuf|2.12-0.9.3|
|commons-lang|2.6|onnxruntime_gpu|1.8.1|
|commons-lang3|3.12.0|opencsv|2.3|
|commons-logging|1.1.3|opencv|3.2.0-1|
|commons-math3|3.6.1|openlineage-spark|2.12-1.26.0-xml-04242025|
|commons-pool|1.5.4|opentest4j|1.2.0|
|commons-pool2|2.11.1|opentracing-api|0.33.0|
|commons-text|1.10.0|opentracing-noop|0.33.0|
|compress-lzf|1.1.2|opentracing-util|0.33.0|
|curator-client|2.13.0|**orc-core**|**1.9.2-shaded-protobuf ⬆️ 1.9.5-shaded-protobuf**|
|curator-framework|2.13.0|**orc-mapreduce**|**1.9.2-shaded-protobuf ⬆️ 1.9.5-shaded-protobuf**|
|curator-recipes|2.13.0|**orc-shims**|**1.9.2 ⬆️ 1.9.5**|
|datanucleus-api-jdo|4.2.4|oro|2.0.8|
|datanucleus-core|4.1.17|osgi-resource-locator|1.0.3|
|datanucleus-rdbms|4.1.19|paranamer|2.8|
|datasketches-java|3.3.0|parquet-column|1.13.1|
|datasketches-memory|2.1.0|parquet-common|1.13.1|
|**delta-kernel-api**|**3.2.0.21 ⬆️ 3.2.0.20250917.1**|parquet-encoding|1.13.1|
|**delta-kernel-defaults**|**3.2.0.21 ⬆️ 3.2.0.20250917.1**|parquet-format-structures|1.13.1|
|**delta-spark**|**2.12-3.2.0.21 ⬆️ 2.12-3.2.0.20250917.1**|**parquet-hadoop-ms**|**3.5.1.5.4.20250512.2 ⬆️ 3.5.5.5.4.20250914.2**|
|**delta-storage**|**3.2.0.21 ⬆️ 3.2.0.20250917.1**|parquet-jackson|1.13.1|
|derby|0.14.2.0|pickle|1.3|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|postgresql|2.2.9|
|flatbuffers-java|1.12.0|profiler|1.1.1|
|fluent-logger|0.3.4-jar-with-dependencies-provided|proton-j|0.33.8|
|gcs-connector-hadoop3|2.2.14-shaded|py4j|0.10.9.7|
|genesis-client|2.12-0.33.1-jar-with-dependencies|qpid-proton-j-extensions|1.2.4|
|gluten-velox-bundle-spark|3.5_2.12-mariner_2.0_x86_64-1.3.0-20250423.2|reactive-streams|1.0.3|
|gson|2.8.9|reactor-core|3.4.34|
|guava|4.0.1|reactor-netty-core|1.0.40|
|**hadoop-aliyun**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|reactor-netty-http|1.0.40|
|**hadoop-annotations**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|rocksdbjni|8.3.2|
|**hadoop-aws**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scala-collection-compat|2.12-2.7.0|
|**hadoop-azure**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scala-compiler|2.12.18|
|**hadoop-azure-datalake**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scala-java8-compat|2.12-0.9.0|
|hadoop-azureml|1.0-fs|scala-library|2.12.18|
|**hadoop-client-api**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scala-parser-combinators|2.12-2.3.0|
|**hadoop-client-runtime**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scala-reflect|2.12.18|
|**hadoop-cloud-storage**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scala-xml|2.12-2.1.0|
|**hadoop-openstack**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scalactic|2.12-3.2.14|
|hadoop-shaded-guava|1.1.1|scalatra|2.12-3.0.0-M1|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.4.20250512.2 ⬆️ 3.3.4.5.4.20250914.2**|scalatra-common|2.12-3.0.0-M1|
|hdinsight-spark-metrics|3.5.0-1.0.11|scalatra-metrics|2.12-3.0.0-M1|
|hive-common|2.3.9|shims|0.9.45|
|hive-exec|2.3.9-core|slf4j-api|2.0.7|
|hive-llap-common|2.3.9|snappy-java|1.1.10.5|
|hive-metastore|2.3.9|spark|3.5-rpc-history-server-core_2.12-1.0.0|
|hive-serde|2.3.9|spark|3.5-advisor-core_2.12-1.0.18|
|hive-shims|2.3.9|spark|3.5-rpc-history-server-app-listener_2.12-1.0.0|
|hive-shims|0.23-2.3.9|spark-avro|2.12-3.5.0|
|hive-shims-common|2.3.9|**spark-avro**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|hive-shims-scheduler|2.3.9|**spark-catalyst**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|hive-storage-api|2.8.1|**spark-common-utils**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|hk2-api|2.6.1|**spark-core**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|hk2-locator|2.6.1|**spark-enhancement**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|hk2-utils|2.6.1|spark-enhancementui|2.12-3.3.0|
|httpclient|4.5.14|**spark-graphx**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|httpclient5|5.1.3|**spark-hadoop-cloud**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|httpcore|4.4.16|**spark-hive**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|httpmime|4.5.13|spark-jobinsight|2.12-1.0.0-spark3.5|
|httpmime|4.5.14|spark-kusto-synapse-connector|3.5_2.12-1.5.2|
|impulse-core_spark|3.5_2.12-1.0.30|**spark-kvstore**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|impulse-telemetry-mds_spark|3.5_2.12-1.0.30|**spark-launcher**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|ini4j|0.5.4|spark-lighter-contract|2.12-2.1.0_spark-3.5.1_20240717.4|
|isolation-forest|3.5.0_2.12-3.0.5|spark-lighter-core|2.12-2.0.11_spark-3.5.1_20240717.4|
|istack-commons-runtime|3.0.8|**spark-microsoft-tools**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|ivy|2.5.1|**spark-mllib**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-annotations|2.15.2|**spark-mllib-local**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-core|2.15.2|spark-mssql-connector-synapse35|1.6.9|
|jackson-core-asl|1.9.13|**spark-network-common**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-databind|2.15.2|**spark-network-shuffle**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-dataformat-cbor|2.15.2|**spark-onesecurity-client**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-dataformat-xml|2.12.7|**spark-onesecurity-common**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-datatype-jsr310|2.15.2|**spark-onesecurity-server**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-mapper-asl|1.9.13|**spark-repl**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-module-jaxb-annotations|2.15.2|**spark-sketch**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jackson-module-scala|2.12-2.15.2|**spark-sql**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jakarta.activation-api|1.2.2|**spark-sql-api**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jakarta.annotation-api|1.3.5|**spark-sql-kafka**|**0_2.12-3.5.1.5.4.20250512.2 ⬆️ 0_2.12-3.5.5.5.4.20250914.2**|
|jakarta.inject|2.6.1|**spark-streaming**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jakarta.servlet-api|4.0.3|**spark-streaming-kafka**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 0_2.12-3.5.5.5.4.20250914.2**|
|jakarta.validation-api|2.0.2|**spark-streaming-kafka**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jakarta.ws.rs-api|2.1.6|**spark-tags**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|jakarta.xml.bind-api|2.3.2|**spark-token-provider-kafka**|**0_2.12-3.5.1.5.4.20250512.2 ⬆️ 0_2.12-3.5.5.5.4.20250914.2**|
|janino|3.1.9|**spark-unsafe**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|javassist|3.29.2-GA|spark-xml|2.12-0.17.0|
|javatuples|1.2|**spark-yarn**|**2.12-3.5.1.5.4.20250512.2 ⬆️ 2.12-3.5.5.5.4.20250914.2**|
|javax.jdo|3.2.0-m3|**spark_diagnostic_cli**|**2.1.7_spark-3.5.1_20250531.2-shaded ⬆️ 2.1.8_spark-3.5.1_20250901.4-shaded**|
|javolution|5.5.1|sparklyr-connector|3.5.1-1.0.0267535|
|jaxb-api|2.2.11|sparknativeparquetwriter|2.12-0.40.0|
|jaxb-runtime|2.3.2|spire|2.12-0.17.0|
|jcl-over-slf4j|2.0.7|spire-macros|2.12-0.17.0|
|jdo-api|3.0.1|spire-platform|2.12-0.17.0|
|jdom2|2.0.6|spire-util|2.12-0.17.0|
|jersey-client|2.40|spray-json|2.12-1.3.5|
|jersey-common|2.40|stax-api|1.0.1|
|jersey-container-servlet|2.40|stax2-api|4.2.1|
|jersey-container-servlet-core|2.40|stream|2.9.6|
|jersey-hk2|2.40|structuredstream|2.12-2.4.1|
|jersey-server|2.40|structuredstreamforspark|2.12-2.4.1|
|jettison|1.1|synapseml-cognitive|2.12-1.0.10-spark3.5|
|**jetty-util**|**9.4.53.v20231009 ⬆️ 9.4.57.v20241219**|synapseml-core|2.12-1.0.10-spark3.5|
|**jetty-util-ajax**|**9.4.53.v20231009 ⬆️ 9.4.57.v20241219**|synapseml-deep-learning|2.12-1.0.10-spark3.5|
|jline|2.14.6|synapseml-internal|2.12-1.0.10.1-spark3.5|
|joda-time|2.12.5|synapseml-lightgbm|2.12-1.0.10-spark3.5|
|jodd-core|3.5.2|synapseml-opencv|2.12-1.0.10-spark3.5|
|jsch|0.1.54|synapseml-vw|2.12-1.0.10-spark3.5|
|json|3|synfs|1.1.11-spark35|
|json|1.8|threeten-extra|1.7.1|
|json-simple|1.1.1|tink|1.9.0|
|json-simple|1.1|transaction-api|1.1|
|json4s-ast|2.12-3.7.0-M11|transform-token-provider-utils|0.0.0|
|json4s-core|2.12-3.7.0-M11|trident-core|1.2.23|
|json4s-jackson|2.12-3.7.0-M11|tridenttokenlibrary-assembly|1.9.10|
|json4s-scalap|2.12-3.7.0-M11|univocity-parsers|2.9.1|
|jsr305|3.0.0|vw-jni|9.3.0|
|jta|1.1|wildfly-openssl|2.1.4.Final|
|jul-to-slf4j|2.0.7|woodstox-core|6.2.4|
|junit-jupiter|5.5.2|xbean-asm9-shaded|4.23|
|junit-jupiter-api|5.5.2|xz|1.9|
|junit-jupiter-engine|5.5.2|**zookeeper**|**3.6.3.5.4.20250512.2 ⬆️ 3.6.3.5.4.20250914.2**|
|junit-jupiter-params|5.5.2|**zookeeper-jute**|**3.6.3.5.4.20250512.2 ⬆️ 3.6.3.5.4.20250914.2**|
|junit-platform-commons|1.5.2|zstd-jni|1.5.5-4|

# R Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|DBI|1.2.3|listenv|0.9.1|
|DiceDesign|1.10|lobstr|1.1.2|
|GPfit|1.0-8|lubridate|1.9.4|
|KernSmooth|2.23-26|magrittr|2.0.3|
|MASS|7.3-64|maps|3.4.2.1|
|Matrix|1.7-3|markdown|1.13|
|ModelMetrics|1.2.2.2|memoise|2.0.1|
|R.methodsS3|1.8.2|methods|4.4.1|
|R.oo|1.27.1|mgcv|1.9-3|
|R.utils|2.13.0|mime|0.13|
|R6|2.6.1|miniUI|0.1.1.1|
|R6P|0.4.0|modeldata|1.4.0|
|RColorBrewer|1.1-3|modelenv|0.2.0|
|RODBC|1.3-25|modelr|0.1.11|
|Rcpp|1.0.14|munsell|0.5.1|
|SQUAREM|2021.1|nlme|3.1-168|
|TTR|0.24.4|nnet|7.3-20|
|V8|6.0.3|notebookutils|1.1.11.35|
|XML|3.99-0.17|numDeriv|2016.8-1.1|
|arrow|18.1.0|openssl|2.3.2|
|askpass|1.2.1|pROC|1.18.5|
|assertthat|0.2.1|parallel|4.4.1|
|backports|1.5.0|parallelly|1.43.0|
|base|4.4.1|parsnip|1.3.1|
|base64enc|0.1-3|patchwork|1.3.0|
|bigD|0.3.1|pillar|1.10.2|
|bit|4.6.0|pkgbuild|1.4.7|
|bit64|4.6.0-1|pkgconfig|2.0.3|
|bitops|1.0-9|pkgdown|2.1.1|
|blob|1.2.4|pkgload|1.4.0|
|brew|1.0-10|plotly|4.10.4|
|brio|1.1.5|plyr|1.8.9|
|broom|1.0.8|praise|1.0.0|
|bslib|0.9.0|prettyunits|1.2.0|
|cachem|1.1.0|processx|3.8.6|
|callr|3.7.6|prodlim|2024.06.25|
|cards|0.5.1|profvis|0.4.0|
|caret|6.0-94|progress|1.2.3|
|cellranger|1.1.0|progressr|0.15.1|
|class|7.3-23|promises|1.3.2|
|classInt|0.4-11|proxy|0.4-27|
|cli|3.6.4|pryr|0.1.6|
|clipr|0.8.0|ps|1.8.1|
|clock|0.7.3|purrr|1.0.4|
|codetools|0.2-20|quantmod|0.4.26|
|collections|0.3.7|ragg|1.3.3|
|colorspace|2.1-1|rappdirs|0.3.3|
|commonmark|1.9.5|rbokeh|0.5.2|
|compiler|4.4.1|rcmdcheck|1.4.0|
|config|0.3.2|reactR|0.6.1|
|conflicted|1.2.0|reactable|0.4.4|
|coro|1.1.0|readr|2.1.5|
|cpp11|0.5.2|readxl|1.4.5|
|crayon|1.5.3|recipes|1.2.1|
|credentials|2.0.2|rematch|2.0.0|
|crosstalk|1.2.1|rematch2|2.1.2|
|crul|1.5.0|remotes|2.5.0|
|curl|6.2.2|reprex|2.1.1|
|data.table|1.17.0|reshape2|1.4.4|
|datasets|4.4.1|rjson|0.2.23|
|dbplyr|2.5.0|rlang|1.1.5|
|desc|1.4.3|rlist|0.4.6.2|
|devtools|2.4.5|rmarkdown|2.29|
|diagram|1.6.5|roxygen2|7.3.2|
|dials|1.4.0|rpart|4.1.24|
|diffobj|0.3.5|rprojroot|2.0.4|
|digest|0.6.37|rsample|1.3.0|
|doFuture|1.0.2|rstudioapi|0.17.1|
|downlit|0.4.4|rversions|2.1.2|
|dplyr|1.1.4|rvest|1.0.4|
|dtplyr|1.3.1|s2|1.1.7|
|e1071|1.7-16|safetensors|0.1.2|
|ellipsis|0.3.2|sass|0.4.9|
|evaluate|1.0.3|scales|1.3.0|
|fansi|1.0.6|selectr|0.4-2|
|farver|2.1.2|sessioninfo|1.2.3|
|fastmap|1.2.0|sf|1.0-16|
|fontawesome|0.5.3|sfd|0.1.0|
|forcats|1.0.0|shape|1.4.6.1|
|foreach|1.5.2|shiny|1.10.0|
|fs|1.6.5|slider|0.3.2|
|furrr|0.3.1|sourcetools|0.1.7-1|
|future|1.34.0|sparklyr|1.8.6|
|future.apply|1.11.3|sparsevctrs|0.3.2|
|gargle|1.5.2|splines|4.4.1|
|generics|0.1.3|stats|4.4.1|
|gert|2.1.4|stats4|4.4.1|
|ggplot2|3.5.1|stringi|1.8.4|
|gh|1.4.1|stringr|1.5.1|
|gistr|0.9.0|survival|3.8-3|
|gitcreds|0.1.2|sys|3.4.3|
|globals|0.16.3|systemfonts|1.2.1|
|glue|1.8.0|tcltk|4.4.1|
|googledrive|2.1.1|testthat|3.2.3|
|googlesheets4|1.1.1|textshaping|0.4.0|
|gower|1.0.1|tibble|3.2.1|
|grDevices|4.4.1|tidymodels|1.3.0|
|graphics|4.4.1|tidyr|1.3.1|
|grid|4.4.1|tidyselect|1.2.1|
|gsl|2.1-8|tidyverse|2.0.0|
|gt|0.11.1|timeDate|4041.110|
|gtable|0.3.6|timechange|0.3.0|
|gtsummary|2.1.0|tinytex|0.56|
|hardhat|1.4.1|tools|4.4.1|
|haven|2.5.4|torch|0.14.2|
|hexbin|1.28.5|triebeard|0.4.1|
|highcharter|0.9.4|tune|1.3.0|
|highr|0.11|tzdb|0.5.0|
|hms|1.1.3|units|0.8-5|
|htmltools|0.5.8.1|urlchecker|1.0.1|
|htmlwidgets|1.6.4|urltools|1.7.3|
|httpcode|0.3.0|usethis|3.1.0|
|httpuv|1.6.15|utf8|1.2.4|
|httr|1.4.7|utils|4.4.1|
|httr2|1.1.2|uuid|1.2-1|
|ids|1.0.1|vctrs|0.6.5|
|igraph|2.0.3|viridisLite|0.4.2|
|infer|1.0.7|vroom|1.6.5|
|ini|0.3.1|waldo|0.6.1|
|ipred|0.9-15|warp|0.2.1|
|isoband|0.2.7|whisker|0.4.1|
|iterators|1.0.14|withr|3.0.2|
|jose|1.2.1|wk|0.9.4|
|jquerylib|0.1.4|workflows|1.2.0|
|jsonlite|2.0.0|workflowsets|1.1.0|
|juicyjuice|0.1.0|xfun|0.52|
|knitr|1.50|xgboost|2.1.4.1|
|labeling|0.4.3|xml2|1.3.6|
|later|1.4.1|xopen|1.0.1|
|lattice|0.22-7|xtable|1.8-4|
|lava|1.8.1|xts|0.14.1|
|lazyeval|0.2.2|yaml|2.3.10|
|lhs|1.2.0|yardstick|1.3.2|
|lifecycle|1.0.4|zip|2.3.2|
|lightgbm|4.6.0|zoo|1.8-13|

