# System Environment
*   **Product**: Fabric Runtime 1.2 (Spark 3.4)
*   **Vhd Release**: Spark3.4-Rel-2025-02-12.0-rc.1
*   **Operating System**: CBL-Mariner 2.0.20250207
*   **Apache Spark**: 3.4.3
*   **Java**: 11.0.26
*   **Scala**: 2.12.17
*   **Python**: 3.10/2.0.0
*   **Delta Lake**: 2.4.0.22

# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1565260|Wildfire/spark34:1.9.25|New Spark 3.4 Release which includes changes in wildfire-spark, wildfire-livy|
|1559834|Conda:8.0.30|Upgrade semantic-link-sempy to 0.9.0|
|1567940|DSCopilotInstaller:1.0.1|Updated the DS Copilot Installer to use V1 for Spark 3.4, ensuring compatibility with the current version without introducing new changes for users.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1564829|HiveMetaStoreClient:1.1.21.1|Reverts changes in the metastore component that introduced an additional dependency on codahale libraries, which caused outages for some customers running Spark 3.4 jobs.|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|AutoscaleProbe|3.9.4|**OneLakeClientStarter**|**1.0.24 ⬆️ 1.0.24.1**|
|Autotune|1.11.1.1|OnelakeSparkCatalog|0.1.21|
|AzureMLExtensions|1.0.4|Peregrine|0.10.4|
|CSparkMetricUpdate|1.0.9|PostgreSQLJDBCDriver|1.0.3|
|**Conda**|**8.0.29 ⬆️ 8.0.30**|Python|3.10/2.0.0|
|CosmosDBConnector|2.2.0|R|1.0.7|
|**DSCopilotInstaller**|**1.0.0 ⬆️ 1.0.1**|SQLServerODBCDriver|18.1.0|
|DWConnector|1.0.3|SStreamOnSparkJar|2.3.5.1|
|Delta|2.4.0.22|SparkAdvisor|1.0.4|
|EventHubConnector|2.3.26|SparkDiagnosticsLibrary|1.0.29|
|ExternalHiveMetastoreLibraries|0.0.7|SparkLighter|2.1.0|
|FabricDWConnector|1.0.10|SparkNativeParquetWriter|0.15.4.1|
|FsspecWrapper|1.0.16|SparkRPCHistoryServer|1.5.0|
|Genesis|0.33.1|SparklyrConnector|1.0.1|
|GlutenUI|1.0.1|TokenLibrary|4.3.6|
|HiveMetaStoreClient|1.1.21.1|TridentCore|1.2.16|
|Impulse|1.2.5|TridentTokenLibrary|1.9.7|
|KustoConnector|1.5.1|VPaaSClient|3.4.01|
|LibraryManager|1.0.24|Vegas|3.4.09.02|
|LibraryMetadataCooker|2.0.3|**Wildfire**|**1.9.24 ⬆️ 1.9.25**|
|MMLSpark|1.4.20|
|MachineLearningPredict|1.0.2|
|MlflowLibrary|2.6.0.1|
|MySQLJavaConnector|1.0.3|
|NotebookUtils|1.1.59|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_openmp_mutex|4.5|lxml|4.9.3|
|_py-xgboost-mutex|2.0|lz4-c|1.9.4|
|absl-py|2.0.0|mako|1.2.4|
|adal|1.2.7|markdown|3.4.4|
|adlfs|2023.4.0|markdown-it-py|3.0.0|
|aiohttp|3.8.6|markupsafe|2.1.3|
|aiosignal|1.3.1|matplotlib|3.7.2|
|alembic|1.12.0|matplotlib-base|3.7.2|
|alsa-lib|1.2.10|matplotlib-inline|0.1.6|
|ansi2html|1.8.0|mdurl|0.1.0|
|anyio|3.7.1|mistune|3.0.1|
|appdirs|1.4.4|mkl|2021.4.0|
|argon2-cffi|23.1.0|mkl-service|2.4.0|
|argon2-cffi-bindings|21.2.0|mkl_fft|1.3.1|
|arrow|1.3.0|mkl_random|1.2.2|
|astor|0.8.1|ml_dtypes|0.3.1|
|asttokens|2.4.0|mlflow-skinny|2.6.0|
|astunparse|1.6.3|monotonic|1.5|
|async-timeout|4.0.3|more-itertools|10.1.0|
|atk-1.0|2.38.0|mpc|1.3.1|
|attr|2.5.1|mpfr|4.2.1|
|attrs|23.1.0|mpg123|1.32.3|
|autopage|0.5.2|mpmath|1.3.0|
|aws-c-auth|0.7.3|msal|1.24.1|
|aws-c-cal|0.6.1|msal_extensions|1.0.0|
|aws-c-common|0.9.0|msgpack|1.0.7|
|aws-c-compression|0.2.17|multidict|6.0.4|
|aws-c-event-stream|0.3.1|multiprocess|0.70.15|
|aws-c-http|0.7.11|munkres|1.1.4|
|aws-c-io|0.13.32|mypy|1.4.1|
|aws-c-mqtt|0.9.3|mypy-extensions|1.0.0|
|aws-c-s3|0.3.14|mysql-common|8.0.33|
|aws-c-sdkutils|0.1.12|mysql-libs|8.0.33|
|aws-checksums|0.1.17|nbclient|0.8.0|
|aws-crt-cpp|0.21.0|nbconvert-core|7.9.2|
|aws-sdk-cpp|1.10.57|nbformat|5.9.2|
|azure-core|1.29.4|ncurses|6.4|
|azure-datalake-store|0.0.51|nest-asyncio|1.5.8|
|azure-identity|1.14.1|networkx|3.2|
|azure-storage-blob|12.18.3|nltk|3.8.1|
|azure-storage-file-datalake|12.12.0|nni|2.10.1|
|azure-synapse-ml-predict|1.0.0|notebookutils|1.1.8.34.20241224.2|
|azureml-synapse|0.0.1|nspr|4.35|
|backcall|0.2.0|nss|3.94|
|backoff|1.11.1|numba|0.57.1|
|backports|1.0|numpy|1.24.3|
|backports.functools_lru_cache|1.6.5|numpy-base|1.24.3|
|bcrypt|4.0.1|oauthlib|3.2.2|
|beautifulsoup4|4.12.2|onnxruntime|1.16.1|
|blas|1.0|openai|0.27.8|
|bleach|6.1.0|openjpeg|2.5.0|
|blinker|1.6.3|openpyxl|3.1.2|
|brotli|1.0.9|openssl|3.1.4|
|brotli-bin|1.0.9|opt-einsum|3.3.0|
|brotli-python|1.0.9|opt_einsum|3.3.0|
|bzip2|1.0.8|optuna|2.8.0|
|c-ares|1.20.1|orc|1.9.0|
|ca-certificates|2023.7.22|overrides|7.4.0|
|cached-property|1.5.2|packaging|23.2|
|cached_property|1.5.2|pandas|2.0.3|
|cachetools|5.3.2|pandas-stubs|2.1.1.230928|
|cairo|1.18.0|pandasql|0.7.3|
|catboost|1.1.1|pandocfilters|1.5.0|
|certifi|2023.7.22|pango|1.50.14|
|cffi|1.16.0|paramiko|3.3.1|
|charset-normalizer|3.3.1|parso|0.8.3|
|chroma-hnswlib|0.7.3|pathos|0.3.1|
|chromadb|0.4.13|pathtools|0.1.2|
|click|8.1.7|patsy|0.5.3|
|cliff|4.2.0|pbr|5.11.1|
|cloudpickle|2.2.1|pcre2|10.40|
|clr_loader|0.2.6|pexpect|4.8.0|
|cmaes|0.10.0|pickleshare|0.7.5|
|cmd2|2.4.3|pillow|10.0.1|
|colorama|0.4.6|pip|23.1.2|
|coloredlogs|15.0.1|pixman|0.42.2|
|colorlog|6.7.0|pkgutil-resolve-name|1.3.10|
|comm|0.1.4|platformdirs|3.5.1|
|conda-package-handling|2.2.0|plotly|5.16.1|
|conda-package-streaming|0.9.0|ply|3.11|
|configparser|5.3.0|pooch|1.8.0|
|contextlib2|21.6.0|portalocker|2.8.2|
|contourpy|1.1.1|posthog|3.0.2|
|cryptography|41.0.5|powerbiclient|3.1.1|
|cycler|0.12.1|pox|0.3.3|
|cython|3.0.4|ppft|1.7.6.7|
|dash|2.14.0|prettytable|3.8.0|
|dash-core-components|2.0.0|prometheus_client|0.17.1|
|dash-html-components|2.0.0|prompt-toolkit|3.0.39|
|dash-table|5.0.0|prompt_toolkit|3.0.39|
|dash_cytoscape|0.2.0|protobuf|4.21.12|
|databricks-cli|0.18.0|psutil|5.9.5|
|dataclasses|0.8|pthread-stubs|0.4|
|datasets|2.14.6|ptyprocess|0.7.0|
|dbus|1.13.6|pulsar-client|3.3.0|
|debugpy|1.8.0|pulseaudio-client|16.1|
|decorator|5.1.1|pure_eval|0.2.2|
|defusedxml|0.7.1|py-xgboost|1.7.6|
|dill|0.3.7|py4j|0.10.9.7|
|diskcache|5.6.3|pyarrow|12.0.1|
|distlib|0.3.7|pyasn1|0.5.0|
|docker-py|6.1.3|pyasn1-modules|0.3.0|
|docker-pycreds|0.4.0|pycosat|0.6.6|
|**dscopilot-installer**|**0.0.7 ⬆️ 0.0.9**|pycparser|2.21|
|entrypoints|0.4|pydantic|1.10.9|
|et_xmlfile|1.1.0|pygments|2.16.1|
|exceptiongroup|1.1.3|pyjwt|2.8.0|
|executing|1.2.0|pynacl|1.5.0|
|expat|2.5.0|pyodbc|4.0.39|
|fastapi|0.103.2|pyopenssl|23.2.0|
|filelock|3.11.0|pyparsing|3.0.9|
|flaml|2.3.3.post3|pyperclip|1.8.2|
|flask|3.0.0|pypika|0.48.9|
|flatbuffers|23.5.26|pyqt|5.15.9|
|fluent-logger|0.10.0|pyqt5-sip|12.12.2|
|font-ttf-dejavu-sans-mono|2.37|pysocks|1.7.1|
|font-ttf-inconsolata|3.000|pyspark|3.4.1.5.3.20230713|
|font-ttf-source-code-pro|2.038|python|3.10.12|
|font-ttf-ubuntu|0.83|python-dateutil|2.8.2|
|fontconfig|2.14.2|python-fastjsonschema|2.18.1|
|fonts-conda-ecosystem|1|python-flatbuffers|23.5.26|
|fonts-conda-forge|1|python-graphviz|0.20.1|
|fonttools|4.43.1|python-json-logger|2.0.7|
|fqdn|1.5.1|python-tzdata|2023.3|
|freetype|2.12.1|python-xxhash|3.4.1|
|fribidi|1.0.10|python_abi|3.10|
|frozenlist|1.4.0|pythonnet|3.0.1|
|fsspec|2023.10.0|pythonwebhdfs|0.2.3|
|fsspec_wrapper|0.1.12|pytorch|2.0.1|
|gast|0.4.0|pytorch-mutex|1.0|
|gdk-pixbuf|2.42.10|pytz|2023.3.post1|
|geographiclib|1.52|pyu2f|0.1.5|
|geopy|2.3.0|pywin32-on-windows|0.1.0|
|gettext|0.21.1|pyyaml|6.0.1|
|gevent|23.9.0.post1|pyzmq|25.1.1|
|gflags|2.2.2|qt-main|5.15.8|
|giflib|5.2.1|rdma-core|28.9|
|gitdb|4.0.11|re2|2023.03.02|
|gitpython|3.1.40|readline|8.2|
|glib|2.78.0|referencing|0.30.2|
|glib-tools|2.78.0|regex|2023.8.8|
|glog|0.6.0|requests|2.31.0|
|gmp|6.2.1|requests-oauthlib|1.3.1|
|gmpy2|2.1.2|responses|0.23.3|
|google-auth|2.23.3|retrying|1.3.3|
|google-auth-oauthlib|1.0.0|rfc3339-validator|0.1.4|
|google-pasta|0.2.0|rfc3986-validator|0.1.1|
|graphite2|1.3.13|rich|13.6.0|
|graphviz|8.1.0|rouge-score|0.1.2|
|greenlet|3.0.1|rpds-py|0.10.6|
|grpcio|1.54.3|rsa|4.9|
|gson|0.0.3|ruamel.yaml|0.17.32|
|gst-plugins-base|1.22.6|ruamel.yaml.clib|0.2.7|
|gstreamer|1.22.6|ruamel_yaml|0.15.80|
|gtk2|2.24.33|s2n|1.3.49|
|gts|0.7.6|sacremoses|0.0.53|
|h11|0.14.0|salib|1.4.7|
|h5py|3.10.0|schema|0.7.5|
|harfbuzz|8.2.1|scikit-learn|1.3.0|
|hdf5|1.14.2|scipy|1.10.1|
|holidays|0.35|seaborn|0.12.2|
|html5lib|1.1|seaborn-base|0.12.2|
|huggingface_hub|0.18.0|**semantic-link-sempy**|**0.8.4 ⬆️ 0.9.0**|
|humanfriendly|10.0|send2trash|1.8.2|
|icu|73.2|sentence-transformers|2.0.0|
|idna|3.4|sentry-sdk|1.32.0|
|imageio|2.31.1|seqeval|1.2.2|
|importlib-metadata|6.8.0|setproctitle|1.3.3|
|importlib-resources|6.1.0|setuptools|68.2.2|
|importlib_metadata|6.8.0|shap|0.42.1|
|importlib_resources|6.1.0|shellingham|1.5.4|
|impulse-python-handler|1.0.22.1.0.0|simplejson|3.19.2|
|intel-openmp|2021.4.0|sip|6.7.12|
|interpret|0.4.3|six|1.16.0|
|interpret-core|0.4.3|slicer|0.0.7|
|ipykernel|6.26.0|smmap|5.0.0|
|ipython|8.14.0|snappy|1.1.10|
|ipywidgets|8.0.7|sniffio|1.3.0|
|isodate|0.6.1|soupsieve|2.5|
|isoduration|20.11.0|sqlalchemy|2.0.22|
|itsdangerous|2.1.2|sqlanalyticsconnectorpy|1.0.1|
|jaraco-context|4.3.0|sqlanalyticsfabricconnectorpy|1.0.0|
|jax|0.4.17|sqlparse|0.4.4|
|jaxlib|0.4.14|stack_data|0.6.2|
|jedi|0.19.1|starlette|0.27.0|
|jinja2|3.1.2|statsmodels|0.14.0|
|joblib|1.3.2|stevedore|5.1.0|
|joblibspark|0.5.2|sympy|1.12|
|json-tricks|3.17.3|synapseml-cognitive|1.0.9|
|jsonpointer|2.4|synapseml-core|1.0.9|
|jsonschema|4.19.1|synapseml-deep-learning|1.0.9|
|jsonschema-specifications|2023.7.1|synapseml-internal|1.0.9.0.dev1|
|jsonschema-with-format-nongpl|4.19.1|synapseml-lightgbm|1.0.9|
|jupyter-ui-poll|0.2.2|synapseml-mlflow|1.0.30.post1|
|jupyter_client|8.5.0|synapseml-opencv|1.0.9|
|jupyter_core|5.4.0|synapseml-utils|1.0.26|
|jupyter_events|0.8.0|synapseml-vw|1.0.9|
|jupyter_server|2.7.3|tabulate|0.9.0|
|jupyter_server_terminals|0.4.4|tbb|2021.10.0|
|jupyterlab_pygments|0.2.2|tenacity|8.2.3|
|jupyterlab_widgets|3.0.9|tensorboard|2.12.3|
|keras|2.12.0|tensorboard-data-server|0.7.0|
|keras-preprocessing|1.1.2|tensorflow|2.12.1|
|keyutils|1.6.1|tensorflow-base|2.12.1|
|kiwisolver|1.4.5|tensorflow-estimator|2.12.1|
|krb5|1.21.2|termcolor|2.3.0|
|lame|3.100|terminado|0.17.1|
|lcms2|2.15|threadpoolctl|3.2.0|
|ld_impl_linux-64|2.40|tiktoken|0.5.1|
|lerc|4.0.0|tinycss2|1.2.1|
|liac-arff|2.5.0|tk|8.6.13|
|libabseil|20230125.3|tokenizers|0.13.3|
|libaec|1.1.2|toml|0.10.2|
|libarrow|12.0.1|tomli|2.0.1|
|libbrotlicommon|1.0.9|toolz|0.12.0|
|libbrotlidec|1.0.9|tornado|6.3.3|
|libbrotlienc|1.0.9|tqdm|4.66.1|
|libcap|2.69|traitlets|5.12.0|
|libclang|15.0.7|transformers|4.26.0|
|libclang13|15.0.7|treeinterpreter|0.2.2|
|libcrc32c|1.1.2|typed-ast|1.5.5|
|libcups|2.3.3|typeguard|2.13.3|
|libcurl|8.4.0|typer|0.9.0|
|libdeflate|1.19|types-python-dateutil|2.8.19.14|
|libebm|0.4.3|types-pytz|2023.3.1.1|
|libedit|3.1.20191231|types-pyyaml|6.0.12.12|
|libev|4.33|typing-extensions|4.8.0|
|libevent|2.1.12|typing_extensions|4.5.0|
|libexpat|2.5.0|typing_utils|0.1.0|
|libffi|3.4.2|tzdata|2023c|
|libflac|1.4.3|ucx|1.14.1|
|libgcc-ng|13.2.0|unicodedata2|15.1.0|
|libgcrypt|1.10.1|unixodbc|2.3.12|
|libgd|2.3.3|uri-template|1.3.0|
|libgfortran-ng|13.2.0|urllib3|1.26.17|
|libgfortran5|13.2.0|uvicorn|0.23.2|
|libglib|2.78.0|virtualenv|20.23.1|
|libgoogle-cloud|2.12.0|wandb|0.15.12|
|libgpg-error|1.47|wcwidth|0.2.8|
|libgrpc|1.54.3|webcolors|1.13|
|libhwloc|2.9.3|webencodings|0.5.1|
|libiconv|1.17|websocket-client|1.6.4|
|libjpeg-turbo|2.1.5.1|websockets|12.0|
|libllvm14|14.0.6|werkzeug|3.0.1|
|libllvm15|15.0.7|wheel|0.41.2|
|libnghttp2|1.52.0|widgetsnbextension|4.0.9|
|libnsl|2.0.1|wolframalpha|5.0.0|
|libnuma|2.0.16|wrapt|1.15.0|
|libogg|1.3.4|xcb-util|0.4.0|
|libopus|1.3.1|xcb-util-image|0.4.0|
|libpng|1.6.39|xcb-util-keysyms|0.4.0|
|libpq|15.4|xcb-util-renderutil|0.3.9|
|libprotobuf|3.21.12|xcb-util-wm|0.4.1|
|libpulsar|3.2.0|xgboost|1.7.6|
|library-metadata-cooker|3.4.1.2|xkeyboard-config|2.40|
|librsvg|2.56.3|xmltodict|0.13.0|
|libsndfile|1.2.2|xorg-kbproto|1.0.7|
|libsodium|1.0.18|xorg-libice|1.1.1|
|libsqlite|3.43.2|xorg-libsm|1.2.4|
|libssh2|1.11.0|xorg-libx11|1.8.7|
|libstdcxx-ng|13.2.0|xorg-libxau|1.0.11|
|libsystemd0|254|xorg-libxdmcp|1.1.3|
|libthrift|0.18.1|xorg-libxext|1.3.4|
|libtiff|4.6.0|xorg-libxrender|0.9.11|
|libtool|2.4.7|xorg-renderproto|0.11.1|
|libutf8proc|2.8.0|xorg-xextproto|7.3.0|
|libuuid|2.38.1|xorg-xf86vidmodeproto|2.3.1|
|libuv|1.46.0|xorg-xproto|7.0.31|
|libvorbis|1.3.7|xxhash|0.8.2|
|libwebp|1.3.2|xz|5.2.6|
|libwebp-base|1.3.2|yaml|0.2.5|
|libxcb|1.15|yarl|1.9.2|
|libxgboost|1.7.6|zeromq|4.3.5|
|libxkbcommon|1.6.0|zipp|3.17.0|
|libxml2|2.11.5|zlib|1.2.13|
|libxslt|1.1.37|zope.event|5.0|
|libzlib|1.2.13|zope.interface|6.1|
|lightgbm|4.0.0|zstandard|0.21.0|
|lime|0.2.0.1|zstd|1.5.5|
|llvm-openmp|17.0.3|_libgcc_mutex|0.1|
|llvmlite|0.40.1|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|json-simple|1.1|
|JLargeArrays|1.5|json4s-ast|2.12-3.7.0-M11|
|JTransforms|3.1|json4s-core|2.12-3.7.0-M11|
|RoaringBitmap|0.9.38|json4s-jackson|2.12-3.7.0-M11|
|ST4|4.0.4|json4s-scalap|2.12-3.7.0-M11|
|SparkCustomEvents|3.4.0-1.0.8|jsr305|3.0.0|
|TokenLibrary-assembly|4.3.6|jta|1.1|
|VPaaSConnector|3.4.01|jul-to-slf4j|2.0.6|
|VegasConnector|3.4.09|junit-jupiter|5.5.2|
|activation|1.1.1|junit-jupiter-api|5.5.2|
|aircompressor|0.21|junit-jupiter-engine|5.5.2|
|algebra|2.12-2.0.1|junit-jupiter-params|5.5.2|
|aliyun-java-sdk-core|4.5.10|junit-platform-commons|1.5.2|
|aliyun-java-sdk-kms|2.11.0|junit-platform-engine|1.5.2|
|aliyun-java-sdk-ram|3.1.0|kafka-clients|3.3.2|
|aliyun-sdk-oss|3.13.0|kryo-shaded|4.0.2|
|annotations|7.0.0|kusto-spark|3.0_2.12-5.2.2-SNAPSHOT|
|antlr-runtime|3.5.2|lapack|3.0.3|
|antlr4-runtime|4.9.3|leveldbjni-all|1.8|
|aopalliance-repackaged|2.6.1|libfb303|0.9.3|
|apiguardian-api|1.1.0|libthrift|0.12.0|
|arpack|3.0.3|lightgbmlib|3.3.510|
|arpack_combined_all|0.1|log4j|1.2-api-2.19.0|
|arrow-format|1.0.0|log4j-api|2.19.0|
|arrow-memory-core|1.0.0|log4j-core|2.19.0|
|arrow-memory-netty|1.0.0|log4j-slf4j2-impl|2.19.0|
|arrow-vector|1.0.0|lz4-java|1.8.0|
|audience-annotations|0.5.0|mdsdclientdynamic|2.0|
|autotune-client|2.12-1.11.1-3.4-125200601|metrics-core|4.2.15|
|autotune-common|2.12-1.11.1-3.4-125200601|metrics-graphite|4.2.15|
|avro|1.11.3|metrics-jmx|4.2.15|
|avro-ipc|1.11.3|metrics-json|4.2.15|
|avro-mapred|1.11.3|metrics-jvm|4.2.15|
|aws-java-sdk-bundle|1.12.262|microsoft-catalog-metastore-client|1.1.21|
|azure-cosmos-analytics-spark|4_2-12_synapse-2.2.0|microsoft-log4j-etwappender|1.0|
|azure-data-lake-store-sdk|2.3.9|minlog|1.3.0|
|azure-eventhubs|3.3.0|mlflow-spark|2.6.0|
|azure-eventhubs-spark|2.12-2.3.22|mysql-connector-java|8.0.18|
|azure-keyvault-core|1.0.0|netty-all|4.1.87.Final|
|azure-storage|7.0.1|netty-buffer|4.1.87.Final|
|azure-synapse-ml-pandas|2.12-0.1.1|netty-codec|4.1.87.Final|
|azure-synapse-ml-predict|2.12-1.0|netty-codec-http|4.1.87.Final|
|blas|3.0.3|netty-codec-http2|4.1.87.Final|
|bonecp|0.8.0.RELEASE|netty-codec-socks|4.1.87.Final|
|breeze|2.12-2.1.0|netty-common|4.1.87.Final|
|breeze-macros|2.12-2.1.0|netty-handler|4.1.87.Final|
|cats-kernel|2.12-2.1.1|netty-handler-proxy|4.1.87.Final|
|chill|2.12-0.10.0|netty-resolver|4.1.87.Final|
|chill-java|0.10.0|netty-transport|4.1.87.Final|
|client-sdk|1.24.1|netty-transport-classes-epoll|4.1.87.Final|
|commons-cli|1.5.0|netty-transport-classes-kqueue|4.1.87.Final|
|commons-codec|1.15|netty-transport-native-epoll|4.1.87.Final-linux-x86_64|
|commons-collections|3.2.2|netty-transport-native-epoll|4.1.87.Final-linux-aarch_64|
|commons-collections4|4.4|netty-transport-native-kqueue|4.1.87.Final-osx-aarch_64|
|commons-compiler|3.1.9|netty-transport-native-kqueue|4.1.87.Final-osx-x86_64|
|commons-compress|1.22|netty-transport-native-unix-common|4.1.87.Final|
|commons-crypto|1.1.0|notebook-utils|1.1.8-spark34-20241224.2|
|commons-dbcp|1.4|objenesis|3.2|
|commons-io|2.11.0|onnx-protobuf|2.12-0.9.3|
|commons-lang|2.6|onnxruntime_gpu|1.8.1|
|commons-lang3|3.12.0|opencsv|2.3|
|commons-logging|1.1.3|opencv|3.2.0-1|
|commons-math3|3.6.1|opentest4j|1.2.0|
|commons-pool|1.5.4|opentracing-api|0.33.0|
|commons-pool2|2.11.1|opentracing-noop|0.33.0|
|commons-text|1.10.0|opentracing-util|0.33.0|
|compress-lzf|1.1.2|orc-core|1.8.7-shaded-protobuf|
|curator-client|2.13.0|orc-mapreduce|1.8.7-shaded-protobuf|
|curator-framework|2.13.0|orc-shims|1.8.7|
|curator-recipes|2.13.0|oro|2.0.8|
|datanucleus-api-jdo|4.2.4|osgi-resource-locator|1.0.3|
|datanucleus-core|4.1.17|paranamer|2.8|
|datanucleus-rdbms|4.1.19|parquet-column|1.12.3|
|delta-core|2.12-2.4.0.22|parquet-common|1.12.3|
|delta-iceberg|2.12-2.4.0.22|parquet-encoding|1.12.3|
|delta-storage|2.4.0.22|parquet-format-structures|1.12.3|
|derby|0.14.2.0|**parquet-hadoop-ms**|**3.4.3.5.3.20241209.1 ⬆️ 3.4.3.5.3.20250203.5**|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|parquet-jackson|1.12.3|
|flatbuffers-java|1.12.0|peregrine-spark|3.4.0-0.10.4|
|fluent-logger|0.3.4-jar-with-dependencies-provided|pickle|1.3|
|gcs-connector-hadoop3|2.2.11-shaded|postgresql|2.2.9|
|genesis-client|2.12-0.33.1-jar-with-dependencies|protobuf-java|2.5.0|
|**gluten-delta**|**1.2.0-20241114.4-3.4**|proton-j|0.33.8|
|**gluten-velox-bundle-spark**|**3.4_2.12-mariner_2.0_x86_64-1.2.0-20241114.4**|py4j|0.10.9.7|
|gson|2.8.9|qpid-proton-j-extensions|1.2.4|
|guava|4.0.1|rocksdbjni|7.9.2|
|**hadoop-aliyun**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scala-collection-compat|2.12-2.7.0|
|**hadoop-annotations**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scala-compiler|2.12.17|
|**hadoop-aws**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scala-java8-compat|2.12-0.9.0|
|**hadoop-azure**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scala-library|2.12.17|
|**hadoop-azure-datalake**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scala-parser-combinators|2.12-2.1.1|
|hadoop-azureml|1.0-fs|scala-reflect|2.12.17|
|**hadoop-client-api**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scala-xml|2.12-2.1.0|
|**hadoop-client-runtime**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|scalactic|2.12-3.2.14|
|**hadoop-cloud-storage**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|shims|0.9.38|
|**hadoop-openstack**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|slf4j-api|2.0.6|
|hadoop-shaded-guava|1.1.1|snappy-java|1.1.10.5|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.3.20241209.1 ⬆️ 3.3.4.5.3.20250203.5**|spark|3.4-rpc-history-server-app-listener_2.12-1.0.0|
|hdinsight-spark-metrics|3.4.0-1.0.8|spark|3.4-rpc-history-server-core_2.12-1.0.0|
|hive-common|2.3.9|spark|3.4-advisor-core_2.12-1.0.18|
|hive-exec|2.3.9-core|spark-avro|2.12-3.4.1|
|hive-llap-common|2.3.9|**spark-avro**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hive-metastore|2.3.9|**spark-catalyst**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hive-serde|2.3.9|**spark-core**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hive-shims|2.3.9|**spark-enhancement**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hive-shims|0.23-2.3.9|spark-enhancementui|2.12-3.3.0|
|hive-shims-common|2.3.9|**spark-graphx**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hive-shims-scheduler|2.3.9|**spark-hadoop-cloud**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hive-storage-api|2.8.1|**spark-hive**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hk2-api|2.6.1|spark-kusto-synapse-connector|3.4_2.12-1.5.1|
|hk2-locator|2.6.1|**spark-kvstore**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|hk2-utils|2.6.1|**spark-launcher**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|httpclient|4.5.14|spark-lighter-contract|2.12-2.0.9_spark-3.4.0_20240703.5|
|httpclient5|5.1.3|spark-lighter-core|2.12-2.0.11_spark-3.4.0_20241101.1|
|httpcore|4.4.16|**spark-microsoft-tools**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|httpmime|4.5.14|**spark-mllib**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|httpmime|4.5.13|**spark-mllib-local**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|impulse-core_spark|3.4_2.12-1.0.22|**spark-network-common**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|impulse-telemetry-mds_spark|3.4_2.12-1.0.22|**spark-network-shuffle**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|ini4j|0.5.4|**spark-repl**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|isolation-forest|3.4.2_2.12-3.0.4|**spark-sketch**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|istack-commons-runtime|3.0.8|**spark-sql**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|ivy|2.5.1|**spark-sql-kafka**|**0_2.12-3.4.3.5.3.20241209.1 ⬆️ 0_2.12-3.4.3.5.3.20250203.5**|
|jackson-annotations|2.14.2|**spark-streaming**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|jackson-core|2.14.2|**spark-streaming-kafka**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 0_2.12-3.4.3.5.3.20250203.5**|
|jackson-core-asl|1.9.13|**spark-streaming-kafka**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|jackson-databind|2.14.2|**spark-tags**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|jackson-dataformat-cbor|2.14.2|**spark-token-provider-kafka**|**0_2.12-3.4.3.5.3.20241209.1 ⬆️ 0_2.12-3.4.3.5.3.20250203.5**|
|jackson-datatype-jsr310|2.14.2|**spark-unsafe**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|jackson-mapper-asl|1.9.13|**spark-yarn**|**2.12-3.4.3.5.3.20241209.1 ⬆️ 2.12-3.4.3.5.3.20250203.5**|
|jackson-module-scala|2.12-2.14.2|spark_diagnostic_cli|2.1.7_spark-3.4.1_20250107.2-shaded|
|jakarta.annotation-api|1.3.5|sparklyr-connector|3.4.1-1.0.0273341|
|jakarta.inject|2.6.1|sparknativeparquetwriter|2.12-0.15.4|
|jakarta.servlet-api|4.0.3|spire|2.12-0.17.0|
|jakarta.validation-api|2.0.2|spire-macros|2.12-0.17.0|
|jakarta.ws.rs-api|2.1.6|spire-platform|2.12-0.17.0|
|jakarta.xml.bind-api|2.3.2|spire-util|2.12-0.17.0|
|janino|3.1.9|spray-json|2.12-1.3.5|
|javassist|3.25.0-GA|stax-api|1.0.1|
|javatuples|1.2|stream|2.9.6|
|javax.jdo|3.2.0-m3|structuredstreamforspark|2.12-3.4.1-2.3.5|
|javolution|5.5.1|synapseml-cognitive|2.12-1.0.9|
|jaxb-api|2.2.11|synapseml-core|2.12-1.0.9|
|jaxb-runtime|2.3.2|synapseml-deep-learning|2.12-1.0.9|
|jcl-over-slf4j|2.0.6|synapseml-internal|2.12-1.0.9.0-spark3.4|
|jdo-api|3.0.1|synapseml-lightgbm|2.12-1.0.9|
|jdom2|2.0.6|synapseml-opencv|2.12-1.0.9|
|jersey-client|2.36|synapseml-vw|2.12-1.0.9|
|jersey-common|2.36|synfs|1.1.8-spark34-20241224.2|
|jersey-container-servlet|2.36|threeten-extra|1.7.1|
|jersey-container-servlet-core|2.36|tink|1.7.0|
|jersey-hk2|2.36|transaction-api|1.1|
|jersey-server|2.36|trident-core|1.2.16|
|jettison|1.1|tridenttokenlibrary-assembly|1.9.7|
|jetty-util|9.4.54.v20240208|univocity-parsers|2.9.1|
|jetty-util-ajax|9.4.54.v20240208|vw-jni|9.3.0|
|jline|2.14.6|wildfly-openssl|1.0.7.Final|
|joda-time|2.12.2|xbean-asm9-shaded|4.22|
|jodd-core|3.5.2|xz|1.9|
|jsch|0.1.54|**zookeeper**|**3.6.3.5.3.20241209.1 ⬆️ 3.6.3.5.3.20250203.5**|
|json|3|**zookeeper-jute**|**3.6.3.5.3.20241209.1 ⬆️ 3.6.3.5.3.20250203.5**|
|json|1.8|zstd-jni|1.5.2-5|
|json-simple|1.1.1|

# R Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|DBI|1.2.3|listenv|0.9.1|
|DiceDesign|1.10|lobstr|1.1.2|
|FabricTelemetry|1.0.2|lubridate|1.9.3|
|GPfit|1.0-8|magrittr|2.0.3|
|KernSmooth|2.23-24|maps|3.4.2|
|MASS|7.3-60.0.1|markdown|1.13|
|Matrix|1.6-5|memoise|2.0.1|
|ModelMetrics|1.2.2.2|methods|4.4.1|
|R.methodsS3|1.8.2|mgcv|1.9-1|
|R.oo|1.27.0|mime|0.12|
|R.utils|2.12.3|miniUI|0.1.1.1|
|R6|2.5.1|modeldata|1.4.0|
|R6P|0.3.0|modelenv|0.1.1|
|RColorBrewer|1.1-3|modelr|0.1.11|
|RODBC|1.3-23|munsell|0.5.1|
|Rcpp|1.0.13|nlme|3.1-165|
|SQUAREM|2021.1|nnet|7.3-19|
|TTR|0.24.4|notebookutils|1.1.8.34.20241224.2|
|V8|5.0.0|numDeriv|2016.8-1.1|
|XML|3.99-0.17|openssl|2.2.1|
|arrow|17.0.0|pROC|1.18.5|
|askpass|1.2.0|parallel|4.4.1|
|assertthat|0.2.1|parallelly|1.38.0|
|backports|1.5.0|parsnip|1.2.1|
|base|4.4.1|patchwork|1.2.0|
|base64enc|0.1-3|pillar|1.9.0|
|bigD|0.2.0|pkgbuild|1.4.4|
|bit|4.0.5|pkgconfig|2.0.3|
|bit64|4.0.5|pkgdown|2.1.0|
|bitops|1.0-8|pkgload|1.4.0|
|blob|1.2.4|plotly|4.10.4|
|brew|1.0-10|plyr|1.8.9|
|brio|1.1.5|praise|1.0.0|
|broom|1.0.6|prettyunits|1.2.0|
|bslib|0.8.0|processx|3.8.4|
|cachem|1.1.0|prodlim|2024.06.25|
|callr|3.7.6|profvis|0.3.8|
|cards|0.2.0|progress|1.2.3|
|caret|6.0-94|progressr|0.14.0|
|cellranger|1.1.0|promises|1.3.0|
|class|7.3-22|proxy|0.4-27|
|classInt|0.4-10|pryr|0.1.6|
|cli|3.6.3|ps|1.7.7|
|clipr|0.8.0|purrr|1.0.2|
|clock|0.7.1|quantmod|0.4.26|
|codetools|0.2-20|ragg|1.3.2|
|collections|0.3.7|rappdirs|0.3.3|
|colorspace|2.1-1|rbokeh|0.5.2|
|commonmark|1.9.1|rcmdcheck|1.4.0|
|compiler|4.4.1|reactR|0.6.0|
|config|0.3.2|reactable|0.4.4|
|conflicted|1.2.0|readr|2.1.5|
|coro|1.0.4|readxl|1.4.3|
|cpp11|0.4.7|recipes|1.1.0|
|crayon|1.5.3|rematch|2.0.0|
|credentials|2.0.1|rematch2|2.1.2|
|crosstalk|1.2.1|remotes|2.5.0|
|crul|1.5.0|reprex|2.1.1|
|curl|5.2.1|reshape2|1.4.4|
|data.table|1.15.4|rjson|0.2.21|
|datasets|4.4.1|rlang|1.1.4|
|dbplyr|2.5.0|rlist|0.4.6.2|
|desc|1.4.3|rmarkdown|2.27|
|devtools|2.4.5|roxygen2|7.3.2|
|diagram|1.6.5|rpart|4.1.23|
|dials|1.3.0|rprojroot|2.0.4|
|diffobj|0.3.5|rsample|1.2.1|
|digest|0.6.36|rstudioapi|0.16.0|
|doFuture|1.0.1|rversions|2.1.2|
|downlit|0.4.4|rvest|1.0.4|
|dplyr|1.1.4|s2|1.1.7|
|dtplyr|1.3.1|safetensors|0.1.2|
|e1071|1.7-14|sass|0.4.9|
|ellipsis|0.3.2|scales|1.3.0|
|evaluate|0.24.0|selectr|0.4-2|
|fansi|1.0.6|sessioninfo|1.2.2|
|farver|2.1.2|sf|1.0-16|
|fastmap|1.2.0|sfd|0.1.0|
|fontawesome|0.5.2|shape|1.4.6.1|
|forcats|1.0.0|shiny|1.9.1|
|foreach|1.5.2|slider|0.3.1|
|fs|1.6.4|sourcetools|0.1.7-1|
|furrr|0.3.1|sparklyr|1.8.6|
|future|1.34.0|splines|4.4.1|
|future.apply|1.11.2|stats|4.4.1|
|gargle|1.5.2|stats4|4.4.1|
|generics|0.1.3|stringi|1.8.4|
|gert|2.1.1|stringr|1.5.1|
|ggplot2|3.5.1|survival|3.7-0|
|gh|1.4.1|sys|3.4.2|
|gistr|0.9.0|systemfonts|1.1.0|
|gitcreds|0.1.2|tcltk|4.4.1|
|globals|0.16.3|testthat|3.2.1.1|
|glue|1.7.0|textshaping|0.4.0|
|googledrive|2.1.1|tibble|3.2.1|
|googlesheets4|1.1.1|tidymodels|1.2.0|
|gower|1.0.1|tidyr|1.3.1|
|grDevices|4.4.1|tidyselect|1.2.1|
|graphics|4.4.1|tidyverse|2.0.0|
|grid|4.4.1|timeDate|4032.109|
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
|jsonlite|1.8.8|xfun|0.46|
|juicyjuice|0.1.0|xgboost|1.7.8.1|
|knitr|1.48|xml2|1.3.6|
|labeling|0.4.3|xopen|1.0.1|
|later|1.3.2|xtable|1.8-4|
|lattice|0.22-6|xts|0.14.0|
|lava|1.7.3|yaml|2.3.10|
|lazyeval|0.2.2|yardstick|1.3.1|
|lhs|1.2.0|zip|2.3.1|
|lifecycle|1.0.4|zoo|1.8-12|
|lightgbm|4.5.0|

