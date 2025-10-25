# System Environment
*   **Product**: Fabric Runtime 1.2 (Spark 3.4)
*   **VHD Name**: 1d3941431dbdc5.vhd
*   **Vhd Release**: Spark3.4-Rel-2025-08-13.1-rc.1
*   **Operating System**: CBL-Mariner 2.0.20250729
*   **Apache Spark**: 3.4.3
*   **Java**: 11.0.27
*   **Scala**: 2.12.17
*   **Python**: 3.10/2.0.0
*   **Delta Lake**: 2.4.0.25

# New Features
|Id|Component|Description|
|-----|-----|-----|
|1720595|Wildfire/spark34:1.9.35.1, OnelakeSparkCatalog:0.2.13|New Spark 3.4 Release with changes in Spark and Onelake Spark Catalog to support legacy query patterns like `<lakehouse>.<table>` and `<workspace>.<artifact>.<table>` on schemaless artifacts|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1761228|LibraryManager/spark34:1.0.31|Adds support for handling case changes in internal Python library names during upgrades in Spark 3.x.|
|1765376|ServiceConfigurationTemplates:spark/3.4.0|Increase spark.yarn.am.waitTime to 200s so that spark context gets enough time for initialization.|
|1736846|ServiceConfigurationTemplates:spark/3.4.0|Enables the ABFS client transaction ID by default to prevent rename failures and improve idempotency in Spark 3.x clusters.|
|1765765|Genesis:0.34.0|Increase timeout for library deployment stage from 10 mins to 30 mins. This is a short-term mitigation for the session acquisition failures due to slow untar performance in LDS|
|1769937|Conda:8.0.42|Reverts changes to flaml and semantic-link-sempy due to broken symlinks. Includes bug fixes and improvements for error handling, performance, and feature support in Spark clusters and semantic modeling functionalities.|
|1720595|Wildfire/spark34:1.9.35.1, OnelakeSparkCatalog:0.2.13|New Spark 3.4 Release with changes in Spark and Onelake Spark Catalog to support legacy query patterns like `<lakehouse>.<table>` and `<workspace>.<artifact>.<table>` on schemaless artifacts|
|1747640|FabricDWConnector:1.0.11|Downgrade Fabric DW Connector to 1.0.19|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1778557|DSCopilot:1.2.1|Enables GPT-4.1 in DS Copilot as the new default model in regions where it is deployed.|
|1711356|AutoscaleProbe:3.9.7|Introduces Autoscale probe version 3.9.7 with a bug fix for scaledown nodes having shuffle data, increasing the graceful decommission timeout to 20 hours to address `ShuffleFetchFailureException`.|
|1756975|LibraryManager:1.0.30|Updates LibraryManager with reliability improvements for Fabric Environment Publish and security fixes to redact sensitive tokens from user-facing logs.|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|**AutoscaleProbe**|**3.9.6 ⬆️ 3.9.7**|OneLakeClientStarter|1.0.26.2|
|Autotune|1.11.1.1|**OnelakeSparkCatalog**|**0.2.7 ⬆️ 0.2.13**|
|AzureMLExtensions|1.0.4|Peregrine|0.10.4|
|Conda|8.0.42|PostgreSQLJDBCDriver|1.0.3|
|CosmosDBConnector|2.2.5|Python|3.10/2.0.0|
|**CSparkMetricUpdate**|**1.0.11 ⬆️ 1.0.12**|R|1.0.7|
|**Delta**|**2.4.0.24 ⬆️ 2.4.0.25**|SparkAdvisor|1.0.5|
|**DSCopilot**|**1.1.0 ⬆️ 1.2.1**|SparkDiagnosticsLibrary|1.0.31|
|DSCopilotInstaller|1.0.1|SparkLighter|2.1.0|
|DWConnector|1.0.4|SparklyrConnector|1.0.1|
|EventHubConnector|2.3.26|SparkNativeParquetWriter|1.2.0-20250515.2|
|ExternalHiveMetastoreLibraries|0.0.7|SparkRPCHistoryServer|1.6.0|
|FabricDWConnector|1.0.11|SQLServerODBCDriver|18.1.0|
|FsspecWrapper|1.0.18|SStreamOnSparkJar|2.3.5.1|
|**Genesis**|**0.33.1 ⬆️ 0.34.0**|TokenLibrary|4.3.8|
|HiveMetaStoreClient|1.1.21.2|**TridentCore**|**1.2.23 ⬆️ 1.2.25**|
|Impulse|1.2.5|**TridentTokenLibrary**|**1.9.10 ⬆️ 1.9.14**|
|**KustoConnector**|**1.5.1 ⬆️ 1.5.3**|Vegas|3.4.09.03|
|**LibraryManager**|**1.0.29 ⬆️ 1.0.31**|VPaaSClient|3.4.01|
|LibraryMetadataCooker|2.0.3|**Wildfire**|**1.9.32.1 ⬆️ 1.9.35.1**|
|MachineLearningPredict|1.0.2|
|MlflowLibrary|2.6.0.1|
|MMLSpark|1.4.20|
|MySQLJavaConnector|1.0.3|
|NotebookUtils|1.1.62.2|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_openmp_mutex|4.5|llvm-openmp|17.0.3|
|_py-xgboost-mutex|2.0|llvmlite|0.40.1|
|absl-py|2.0.0|lxml|4.9.3|
|adal|1.2.7|lz4-c|1.9.4|
|adlfs|2023.4.0|mako|1.2.4|
|aiohttp|3.8.6|markdown|3.4.4|
|aiosignal|1.3.1|markdown-it-py|3.0.0|
|alembic|1.12.0|markupsafe|2.1.3|
|alsa-lib|1.2.10|matplotlib|3.7.2|
|ansi2html|1.8.0|matplotlib-base|3.7.2|
|anyio|3.7.1|matplotlib-inline|0.1.6|
|appdirs|1.4.4|mdurl|0.1.0|
|argon2-cffi|23.1.0|mistune|3.0.1|
|argon2-cffi-bindings|21.2.0|mkl|2021.4.0|
|arrow|1.3.0|mkl-service|2.4.0|
|astor|0.8.1|mkl_fft|1.3.1|
|asttokens|2.4.0|mkl_random|1.2.2|
|astunparse|1.6.3|ml_dtypes|0.3.1|
|async-timeout|4.0.3|mlflow-skinny|2.6.0|
|atk-1.0|2.38.0|monotonic|1.5|
|attr|2.5.1|more-itertools|10.1.0|
|attrs|23.1.0|mpc|1.3.1|
|autopage|0.5.2|mpfr|4.2.1|
|aws-c-auth|0.7.3|mpg123|1.32.3|
|aws-c-cal|0.6.1|mpmath|1.3.0|
|aws-c-common|0.9.0|msal|1.24.1|
|aws-c-compression|0.2.17|msal_extensions|1.0.0|
|aws-c-event-stream|0.3.1|msgpack|1.0.7|
|aws-c-http|0.7.11|multidict|6.0.4|
|aws-c-io|0.13.32|multiprocess|0.70.15|
|aws-c-mqtt|0.9.3|munkres|1.1.4|
|aws-c-s3|0.3.14|mypy|1.4.1|
|aws-c-sdkutils|0.1.12|mypy-extensions|1.0.0|
|aws-checksums|0.1.17|mysql-common|8.0.33|
|aws-crt-cpp|0.21.0|mysql-libs|8.0.33|
|aws-sdk-cpp|1.10.57|nbclient|0.8.0|
|azure-core|1.29.4|nbconvert-core|7.9.2|
|azure-datalake-store|0.0.51|nbformat|5.9.2|
|azure-identity|1.14.1|ncurses|6.4|
|azure-storage-blob|12.18.3|nest-asyncio|1.5.8|
|azure-storage-file-datalake|12.12.0|networkx|3.2|
|azure-synapse-ml-predict|1.0.0|nltk|3.8.1|
|azureml-synapse|0.0.1|nni|2.10.1|
|backcall|0.2.0|notebookutils|1.1.11.34.20250605.2|
|backoff|1.11.1|nspr|4.35|
|backports|1.0|nss|3.94|
|backports.functools_lru_cache|1.6.5|numba|0.57.1|
|bcrypt|4.0.1|numpy|1.24.3|
|beautifulsoup4|4.12.2|numpy-base|1.24.3|
|blas|1.0|oauthlib|3.2.2|
|bleach|6.1.0|onnxruntime|1.16.1|
|blinker|1.6.3|openai|0.27.8|
|brotli|1.0.9|openjpeg|2.5.0|
|brotli-bin|1.0.9|openpyxl|3.1.2|
|brotli-python|1.0.9|openssl|3.1.4|
|bzip2|1.0.8|opt-einsum|3.3.0|
|c-ares|1.20.1|opt_einsum|3.3.0|
|ca-certificates|2023.7.22|optuna|2.8.0|
|cached-property|1.5.2|orc|1.9.0|
|cached_property|1.5.2|overrides|7.4.0|
|cachetools|5.3.2|packaging|23.2|
|cairo|1.18.0|pandas|2.0.3|
|catboost|1.1.1|pandas-stubs|2.1.1.230928|
|certifi|2023.7.22|pandasql|0.7.3|
|cffi|1.16.0|pandocfilters|1.5.0|
|charset-normalizer|3.3.1|pango|1.50.14|
|**chat-magics**|**0.1.25.2.25 ⬆️ 0.1.25.2.28**|paramiko|3.3.1|
|**chat-magics-fabric**|**0.2.0.25.2.26 ⬆️ 0.2.0.25.8.21**|parso|0.8.3|
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
|**ds-copilot**|**0.1.25.2.25 ⬆️ 0.1.25.2.28**|pycparser|2.21|
|dscopilot-installer|0.0.9|pydantic|1.10.9|
|entrypoints|0.4|pygments|2.16.1|
|et_xmlfile|1.1.0|pyjwt|2.8.0|
|exceptiongroup|1.1.3|pynacl|1.5.0|
|executing|1.2.0|pyodbc|4.0.39|
|expat|2.5.0|pyopenssl|23.2.0|
|fabric-connection|0.2.0|pyparsing|3.0.9|
|fastapi|0.103.2|pyperclip|1.8.2|
|filelock|3.11.0|pypika|0.48.9|
|flaml|2.3.4.post2|pyqt|5.15.9|
|flask|3.0.0|pyqt5-sip|12.12.2|
|flatbuffers|23.5.26|pysocks|1.7.1|
|fluent-logger|0.10.0|pyspark|3.4.1.5.3.20230713|
|font-ttf-dejavu-sans-mono|2.37|python|3.10.12|
|font-ttf-inconsolata|3.000|python-dateutil|2.8.2|
|font-ttf-source-code-pro|2.038|python-fastjsonschema|2.18.1|
|font-ttf-ubuntu|0.83|python-flatbuffers|23.5.26|
|fontconfig|2.14.2|python-graphviz|0.20.1|
|fonts-conda-ecosystem|1|python-json-logger|2.0.7|
|fonts-conda-forge|1|python-tzdata|2023.3|
|fonttools|4.43.1|python-xxhash|3.4.1|
|fqdn|1.5.1|python_abi|3.10|
|freetype|2.12.1|pythonnet|3.0.1|
|fribidi|1.0.10|pythonwebhdfs|0.2.3|
|frozenlist|1.4.0|pytorch|2.0.1|
|fsspec|2023.10.0|pytorch-mutex|1.0|
|fsspec_wrapper|0.1.15|pytz|2023.3.post1|
|gast|0.4.0|pyu2f|0.1.5|
|gdk-pixbuf|2.42.10|pywin32-on-windows|0.1.0|
|geographiclib|1.52|pyyaml|6.0.1|
|geopy|2.3.0|pyzmq|25.1.1|
|gettext|0.21.1|qt-main|5.15.8|
|gevent|23.9.0.post1|rdma-core|28.9|
|gflags|2.2.2|re2|2023.03.02|
|giflib|5.2.1|readline|8.2|
|gitdb|4.0.11|referencing|0.30.2|
|gitpython|3.1.40|regex|2023.8.8|
|glib|2.78.0|requests|2.31.0|
|glib-tools|2.78.0|requests-oauthlib|1.3.1|
|glog|0.6.0|responses|0.23.3|
|gmp|6.2.1|retrying|1.3.3|
|gmpy2|2.1.2|rfc3339-validator|0.1.4|
|google-auth|2.23.3|rfc3986-validator|0.1.1|
|google-auth-oauthlib|1.0.0|rich|13.6.0|
|google-pasta|0.2.0|rouge-score|0.1.2|
|graphite2|1.3.13|rpds-py|0.10.6|
|graphviz|8.1.0|rsa|4.9|
|greenlet|3.0.1|ruamel.yaml|0.17.32|
|grpcio|1.54.3|ruamel.yaml.clib|0.2.7|
|gson|0.0.3|ruamel_yaml|0.15.80|
|gst-plugins-base|1.22.6|s2n|1.3.49|
|gstreamer|1.22.6|sacremoses|0.0.53|
|gtk2|2.24.33|salib|1.4.7|
|gts|0.7.6|schema|0.7.5|
|h11|0.14.0|scikit-learn|1.3.0|
|h5py|3.10.0|scipy|1.10.1|
|harfbuzz|8.2.1|seaborn|0.12.2|
|hdf5|1.14.2|seaborn-base|0.12.2|
|holidays|0.35|semantic-link-sempy|0.10.2|
|html5lib|1.1|send2trash|1.8.2|
|huggingface_hub|0.18.0|sentence-transformers|2.0.0|
|humanfriendly|10.0|sentry-sdk|1.32.0|
|icu|73.2|seqeval|1.2.2|
|idna|3.4|setproctitle|1.3.3|
|imageio|2.31.1|setuptools|68.2.2|
|importlib-metadata|6.8.0|shap|0.42.1|
|importlib-resources|6.1.0|shellingham|1.5.4|
|importlib_metadata|6.8.0|simplejson|3.19.2|
|importlib_resources|6.1.0|sip|6.7.12|
|impulse-python-handler|1.0.22.1.0.0|six|1.16.0|
|intel-openmp|2021.4.0|slicer|0.0.7|
|interpret|0.4.3|smmap|5.0.0|
|interpret-core|0.4.3|snappy|1.1.10|
|ipykernel|6.26.0|sniffio|1.3.0|
|ipython|8.14.0|soupsieve|2.5|
|ipywidgets|8.0.7|sqlalchemy|2.0.22|
|isodate|0.6.1|sqlanalyticsconnectorpy|1.0.1|
|isoduration|20.11.0|sqlanalyticsfabricconnectorpy|1.0.0|
|itsdangerous|2.1.2|sqlparse|0.4.4|
|jaraco-context|4.3.0|stack_data|0.6.2|
|jax|0.4.17|starlette|0.27.0|
|jaxlib|0.4.14|statsmodels|0.14.0|
|jedi|0.19.1|stevedore|5.1.0|
|jinja2|3.1.2|sympy|1.12|
|joblib|1.3.2|synapseml-cognitive|1.0.9|
|joblibspark|0.5.2|synapseml-core|1.0.9|
|json-tricks|3.17.3|synapseml-deep-learning|1.0.9|
|jsonpointer|2.4|synapseml-internal|1.0.9.0.dev1|
|jsonschema|4.19.1|synapseml-lightgbm|1.0.9|
|jsonschema-specifications|2023.7.1|synapseml-mlflow|1.0.31|
|jsonschema-with-format-nongpl|4.19.1|synapseml-opencv|1.0.9|
|jupyter-ui-poll|0.2.2|synapseml-utils|1.1.6.post2|
|jupyter_client|8.5.0|synapseml-vw|1.0.9|
|jupyter_core|5.4.0|tabulate|0.9.0|
|jupyter_events|0.8.0|tbb|2021.10.0|
|jupyter_server|2.7.3|tenacity|8.2.3|
|jupyter_server_terminals|0.4.4|tensorboard|2.12.3|
|jupyterlab_pygments|0.2.2|tensorboard-data-server|0.7.0|
|jupyterlab_widgets|3.0.9|tensorflow|2.12.1|
|keras|2.12.0|tensorflow-base|2.12.1|
|keras-preprocessing|1.1.2|tensorflow-estimator|2.12.1|
|keyutils|1.6.1|termcolor|2.3.0|
|kiwisolver|1.4.5|terminado|0.17.1|
|krb5|1.21.2|threadpoolctl|3.2.0|
|lame|3.100|tiktoken|0.5.1|
|lcms2|2.15|tinycss2|1.2.1|
|ld_impl_linux-64|2.40|tk|8.6.13|
|lerc|4.0.0|tokenizers|0.13.3|
|liac-arff|2.5.0|toml|0.10.2|
|libabseil|20230125.3|tomli|2.0.1|
|libaec|1.1.2|toolz|0.12.0|
|libarrow|12.0.1|tornado|6.3.3|
|libbrotlicommon|1.0.9|tqdm|4.66.1|
|libbrotlidec|1.0.9|traitlets|5.12.0|
|libbrotlienc|1.0.9|transformers|4.26.0|
|libcap|2.69|treeinterpreter|0.2.2|
|libclang|15.0.7|typed-ast|1.5.5|
|libclang13|15.0.7|typeguard|2.13.3|
|libcrc32c|1.1.2|typer|0.9.0|
|libcups|2.3.3|types-python-dateutil|2.8.19.14|
|libcurl|8.4.0|types-pytz|2023.3.1.1|
|libdeflate|1.19|types-pyyaml|6.0.12.12|
|libebm|0.4.3|typing-extensions|4.8.0|
|libedit|3.1.20191231|typing_extensions|4.5.0|
|libev|4.33|typing_utils|0.1.0|
|libevent|2.1.12|tzdata|2023c|
|libexpat|2.5.0|ucx|1.14.1|
|libffi|3.4.2|unicodedata2|15.1.0|
|libflac|1.4.3|unixodbc|2.3.12|
|libgcc-ng|13.2.0|uri-template|1.3.0|
|libgcrypt|1.10.1|urllib3|1.26.17|
|libgd|2.3.3|uvicorn|0.23.2|
|libgfortran-ng|13.2.0|virtualenv|20.23.1|
|libgfortran5|13.2.0|wandb|0.15.12|
|libglib|2.78.0|wcwidth|0.2.8|
|libgoogle-cloud|2.12.0|webcolors|1.13|
|libgpg-error|1.47|webencodings|0.5.1|
|libgrpc|1.54.3|websocket-client|1.6.4|
|libhwloc|2.9.3|websockets|12.0|
|libiconv|1.17|werkzeug|3.0.1|
|libjpeg-turbo|2.1.5.1|wheel|0.41.2|
|libllvm14|14.0.6|widgetsnbextension|4.0.9|
|libllvm15|15.0.7|wolframalpha|5.0.0|
|libnghttp2|1.52.0|wrapt|1.15.0|
|libnsl|2.0.1|xcb-util|0.4.0|
|libnuma|2.0.16|xcb-util-image|0.4.0|
|libogg|1.3.4|xcb-util-keysyms|0.4.0|
|libopus|1.3.1|xcb-util-renderutil|0.3.9|
|libpng|1.6.39|xcb-util-wm|0.4.1|
|libpq|15.4|xgboost|1.7.6|
|libprotobuf|3.21.12|xkeyboard-config|2.40|
|libpulsar|3.2.0|xmltodict|0.13.0|
|library-metadata-cooker|3.4.1.2|xorg-kbproto|1.0.7|
|librsvg|2.56.3|xorg-libice|1.1.1|
|libsndfile|1.2.2|xorg-libsm|1.2.4|
|libsodium|1.0.18|xorg-libx11|1.8.7|
|libsqlite|3.43.2|xorg-libxau|1.0.11|
|libssh2|1.11.0|xorg-libxdmcp|1.1.3|
|libstdcxx-ng|13.2.0|xorg-libxext|1.3.4|
|libsystemd0|254|xorg-libxrender|0.9.11|
|libthrift|0.18.1|xorg-renderproto|0.11.1|
|libtiff|4.6.0|xorg-xextproto|7.3.0|
|libtool|2.4.7|xorg-xf86vidmodeproto|2.3.1|
|libutf8proc|2.8.0|xorg-xproto|7.0.31|
|libuuid|2.38.1|xxhash|0.8.2|
|libuv|1.46.0|xz|5.2.6|
|libvorbis|1.3.7|yaml|0.2.5|
|libwebp|1.3.2|yarl|1.9.2|
|libwebp-base|1.3.2|zeromq|4.3.5|
|libxcb|1.15|zipp|3.17.0|
|libxgboost|1.7.6|zlib|1.2.13|
|libxkbcommon|1.6.0|zope.event|5.0|
|libxml2|2.11.5|zope.interface|6.1|
|libxslt|1.1.37|zstandard|0.21.0|
|libzlib|1.2.13|zstd|1.5.5|
|lightgbm|4.0.0|_libgcc_mutex|0.1|
|lime|0.2.0.1|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|json4s-ast|2.12-3.7.0-M11|
|JLargeArrays|1.5|json4s-core|2.12-3.7.0-M11|
|JTransforms|3.1|json4s-jackson|2.12-3.7.0-M11|
|RoaringBitmap|0.9.38|json4s-scalap|2.12-3.7.0-M11|
|ST4|4.0.4|jsr305|3.0.0|
|**SparkCustomEvents**|**3.4.0-1.0.10 ⬆️ 3.4.0-1.0.11**|jta|1.1|
|TokenLibrary-assembly|4.3.8|jul-to-slf4j|2.0.6|
|VPaaSConnector|3.4.01|junit-jupiter|5.5.2|
|VegasConnector|3.4.09|junit-jupiter-api|5.5.2|
|activation|1.1.1|junit-jupiter-engine|5.5.2|
|aircompressor|0.21|junit-jupiter-params|5.5.2|
|algebra|2.12-2.0.1|junit-platform-commons|1.5.2|
|aliyun-java-sdk-core|4.5.10|junit-platform-engine|1.5.2|
|aliyun-java-sdk-kms|2.11.0|kafka-clients|3.3.2|
|aliyun-java-sdk-ram|3.1.0|kryo-shaded|4.0.2|
|aliyun-sdk-oss|3.13.0|**kusto-spark**|**3.0_2.12-5.2.2-SNAPSHOT ⬆️ 3.0_2.12-5.3.1**|
|annotations|7.0.0|lapack|3.0.3|
|antlr-runtime|3.5.2|leveldbjni-all|1.8|
|antlr4-runtime|4.9.3|libfb303|0.9.3|
|aopalliance-repackaged|2.6.1|libthrift|0.12.0|
|apiguardian-api|1.1.0|lightgbmlib|3.3.510|
|arpack|3.0.3|log4j|1.2-api-2.19.0|
|arpack_combined_all|0.1|log4j-api|2.19.0|
|arrow-format|1.0.0|log4j-core|2.19.0|
|arrow-memory-core|1.0.0|log4j-slf4j2-impl|2.19.0|
|arrow-memory-netty|1.0.0|lz4-java|1.8.0|
|arrow-vector|1.0.0|mdsdclientdynamic|2.0|
|audience-annotations|0.5.0|metrics-core|4.2.15|
|autotune-client|2.12-1.11.1-3.4-125200601|metrics-graphite|4.2.15|
|autotune-common|2.12-1.11.1-3.4-125200601|metrics-jmx|4.2.15|
|avro|1.11.3|metrics-json|4.2.15|
|avro-ipc|1.11.3|metrics-jvm|4.2.15|
|avro-mapred|1.11.3|microsoft-catalog-metastore-client|1.1.21|
|aws-java-sdk-bundle|1.12.262|microsoft-log4j-etwappender|1.0|
|azure-cosmos-analytics-spark|4_2-12_synapse-2.2.5|minlog|1.3.0|
|azure-data-lake-store-sdk|2.3.9|mlflow-spark|2.6.0|
|azure-eventhubs|3.3.0|mysql-connector-java|8.0.18|
|azure-eventhubs-spark|2.12-2.3.22|netty-all|4.1.87.Final|
|azure-keyvault-core|1.0.0|netty-buffer|4.1.87.Final|
|azure-storage|7.0.1|netty-codec|4.1.87.Final|
|azure-synapse-ml-pandas|2.12-0.1.1|netty-codec-http|4.1.87.Final|
|azure-synapse-ml-predict|2.12-1.0|netty-codec-http2|4.1.87.Final|
|blas|3.0.3|netty-codec-socks|4.1.87.Final|
|bonecp|0.8.0.RELEASE|netty-common|4.1.87.Final|
|breeze|2.12-2.1.0|netty-handler|4.1.87.Final|
|breeze-macros|2.12-2.1.0|netty-handler-proxy|4.1.87.Final|
|cats-kernel|2.12-2.1.1|netty-resolver|4.1.87.Final|
|chill|2.12-0.10.0|netty-transport|4.1.87.Final|
|chill-java|0.10.0|netty-transport-classes-epoll|4.1.87.Final|
|client-sdk|1.24.1|netty-transport-classes-kqueue|4.1.87.Final|
|commons-cli|1.5.0|netty-transport-native-epoll|4.1.87.Final-linux-x86_64|
|commons-codec|1.15|netty-transport-native-epoll|4.1.87.Final-linux-aarch_64|
|commons-collections|3.2.2|netty-transport-native-kqueue|4.1.87.Final-osx-aarch_64|
|commons-collections4|4.4|netty-transport-native-kqueue|4.1.87.Final-osx-x86_64|
|commons-compiler|3.1.9|netty-transport-native-unix-common|4.1.87.Final|
|commons-compress|1.22|notebook-utils|1.1.11-spark34-20250605.2|
|commons-crypto|1.1.0|objenesis|3.2|
|commons-dbcp|1.4|onnx-protobuf|2.12-0.9.3|
|commons-io|2.11.0|onnxruntime_gpu|1.8.1|
|commons-lang|2.6|opencsv|2.3|
|commons-lang3|3.12.0|opencv|3.2.0-1|
|commons-logging|1.1.3|opentest4j|1.2.0|
|commons-math3|3.6.1|opentracing-api|0.33.0|
|commons-pool|1.5.4|opentracing-noop|0.33.0|
|commons-pool2|2.11.1|opentracing-util|0.33.0|
|commons-text|1.10.0|orc-core|1.8.7-shaded-protobuf|
|compress-lzf|1.1.2|orc-mapreduce|1.8.7-shaded-protobuf|
|curator-client|2.13.0|orc-shims|1.8.7|
|curator-framework|2.13.0|oro|2.0.8|
|curator-recipes|2.13.0|osgi-resource-locator|1.0.3|
|datanucleus-api-jdo|4.2.4|paranamer|2.8|
|datanucleus-core|4.1.17|parquet-column|1.12.3|
|datanucleus-rdbms|4.1.19|parquet-common|1.12.3|
|**delta-core**|**2.12-2.4.0.24 ⬆️ 2.12-2.4.0.25**|parquet-encoding|1.12.3|
|**delta-iceberg**|**2.12-2.4.0.24 ⬆️ 2.12-2.4.0.25**|parquet-format-structures|1.12.3|
|**delta-storage**|**2.4.0.24 ⬆️ 2.4.0.25**|**parquet-hadoop-ms**|**3.4.3.5.3.20250511.1 ⬆️ 3.4.3.5.3.20250628.1**|
|derby|0.14.2.0|parquet-jackson|1.12.3|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|peregrine-spark|3.4.0-0.10.4|
|flatbuffers-java|1.12.0|pickle|1.3|
|fluent-logger|0.3.4-jar-with-dependencies-provided|postgresql|2.2.9|
|gcs-connector-hadoop3|2.2.11-shaded|protobuf-java|2.5.0|
|**genesis-client**|**2.12-0.33.1-jar-with-dependencies ⬆️ 2.12-0.34.0-jar-with-dependencies**|proton-j|0.33.8|
|gson|2.8.9|py4j|0.10.9.7|
|guava|4.0.1|qpid-proton-j-extensions|1.2.4|
|**hadoop-aliyun**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|rocksdbjni|7.9.2|
|**hadoop-annotations**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scala-collection-compat|2.12-2.7.0|
|**hadoop-aws**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scala-compiler|2.12.17|
|**hadoop-azure**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scala-java8-compat|2.12-0.9.0|
|**hadoop-azure-datalake**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scala-library|2.12.17|
|hadoop-azureml|1.0-fs|scala-parser-combinators|2.12-2.1.1|
|**hadoop-client-api**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scala-reflect|2.12.17|
|**hadoop-client-runtime**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scala-xml|2.12-2.1.0|
|**hadoop-cloud-storage**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|scalactic|2.12-3.2.14|
|**hadoop-openstack**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|shims|0.9.38|
|hadoop-shaded-guava|1.1.1|slf4j-api|2.0.6|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250628.1**|snappy-java|1.1.10.5|
|**hdinsight-spark-metrics**|**3.4.0-1.0.10 ⬆️ 3.4.0-1.0.11**|spark|3.4-rpc-history-server-app-listener_2.12-1.0.0|
|hive-common|2.3.9|spark|3.4-rpc-history-server-core_2.12-1.0.0|
|hive-exec|2.3.9-core|spark|3.4-advisor-core_2.12-1.0.18|
|hive-llap-common|2.3.9|spark-avro|2.12-3.4.1|
|hive-metastore|2.3.9|**spark-avro**|**2.12-3.4.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hive-serde|2.3.9|**spark-catalyst**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hive-shims|2.3.9|**spark-core**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hive-shims|0.23-2.3.9|**spark-enhancement**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hive-shims-common|2.3.9|spark-enhancementui|2.12-3.3.0|
|hive-shims-scheduler|2.3.9|**spark-graphx**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hive-storage-api|2.8.1|**spark-hadoop-cloud**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hk2-api|2.6.1|**spark-hive**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|hk2-locator|2.6.1|**spark-kusto-synapse-connector**|**3.4_2.12-1.5.1 ⬆️ 3.4_2.12-1.5.3**|
|hk2-utils|2.6.1|**spark-kvstore**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|httpclient|4.5.14|**spark-launcher**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|httpclient5|5.1.3|spark-lighter-contract|2.12-2.0.9_spark-3.4.0_20240703.5|
|httpcore|4.4.16|spark-lighter-core|2.12-2.0.11_spark-3.4.0_20241101.1|
|httpmime|4.5.14|**spark-microsoft-tools**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|httpmime|4.5.13|**spark-mllib**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|impulse-core_spark|3.4_2.12-1.0.22|**spark-mllib-local**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|impulse-telemetry-mds_spark|3.4_2.12-1.0.22|**spark-network-common**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|ini4j|0.5.4|**spark-network-shuffle**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|isolation-forest|3.4.2_2.12-3.0.4|**spark-repl**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|istack-commons-runtime|3.0.8|**spark-sketch**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|ivy|2.5.1|**spark-sql**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|jackson-annotations|2.14.2|**spark-sql-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 0_2.12-3.4.3.5.3.20250628.1**|
|jackson-core|2.14.2|**spark-streaming**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|jackson-core-asl|1.9.13|**spark-streaming-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 0_2.12-3.4.3.5.3.20250628.1**|
|jackson-databind|2.14.2|**spark-streaming-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|jackson-dataformat-cbor|2.14.2|**spark-tags**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|jackson-datatype-jsr310|2.14.2|**spark-token-provider-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 0_2.12-3.4.3.5.3.20250628.1**|
|jackson-mapper-asl|1.9.13|**spark-unsafe**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|jackson-module-scala|2.12-2.14.2|**spark-yarn**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250628.1**|
|jakarta.annotation-api|1.3.5|spark_diagnostic_cli|2.1.9_spark-3.4.1_20250530.5-shaded|
|jakarta.inject|2.6.1|sparklyr-connector|3.4.1-1.0.0273341|
|jakarta.servlet-api|4.0.3|sparknativeparquetwriter|2.12-1.2.0-20250515.2|
|jakarta.validation-api|2.0.2|spire|2.12-0.17.0|
|jakarta.ws.rs-api|2.1.6|spire-macros|2.12-0.17.0|
|jakarta.xml.bind-api|2.3.2|spire-platform|2.12-0.17.0|
|janino|3.1.9|spire-util|2.12-0.17.0|
|javassist|3.25.0-GA|spray-json|2.12-1.3.5|
|javatuples|1.2|stax-api|1.0.1|
|javax.jdo|3.2.0-m3|stream|2.9.6|
|javolution|5.5.1|structuredstreamforspark|2.12-3.4.1-2.3.5|
|jaxb-api|2.2.11|synapseml-cognitive|2.12-1.0.9|
|jaxb-runtime|2.3.2|synapseml-core|2.12-1.0.9|
|jcl-over-slf4j|2.0.6|synapseml-deep-learning|2.12-1.0.9|
|jdo-api|3.0.1|synapseml-internal|2.12-1.0.9.0-spark3.4|
|jdom2|2.0.6|synapseml-lightgbm|2.12-1.0.9|
|jersey-client|2.36|synapseml-opencv|2.12-1.0.9|
|jersey-common|2.36|synapseml-vw|2.12-1.0.9|
|jersey-container-servlet|2.36|synfs|1.1.11-spark34-20250605.2|
|jersey-container-servlet-core|2.36|threeten-extra|1.7.1|
|jersey-hk2|2.36|tink|1.7.0|
|jersey-server|2.36|transaction-api|1.1|
|jettison|1.1|**trident-core**|**1.2.23 ⬆️ 1.2.25**|
|jetty-util|9.4.54.v20240208|**tridenttokenlibrary-assembly**|**1.9.10 ⬆️ 1.9.14**|
|jetty-util-ajax|9.4.54.v20240208|univocity-parsers|2.9.1|
|jline|2.14.6|vw-jni|9.3.0|
|joda-time|2.12.2|wildfly-openssl|1.0.7.Final|
|jodd-core|3.5.2|xbean-asm9-shaded|4.22|
|jsch|0.1.54|xz|1.9|
|json|3|**zookeeper**|**3.6.3.5.3.20250511.1 ⬆️ 3.6.3.5.3.20250628.1**|
|json|1.8|**zookeeper-jute**|**3.6.3.5.3.20250511.1 ⬆️ 3.6.3.5.3.20250628.1**|
|json-simple|1.1.1|zstd-jni|1.5.2-5|
|json-simple|1.1|

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
|R.oo|1.27.1|mime|0.12|
|R.utils|2.13.0|miniUI|0.1.1.1|
|R6|2.5.1|modeldata|1.4.0|
|R6P|0.3.0|modelenv|0.1.1|
|RColorBrewer|1.1-3|modelr|0.1.11|
|RODBC|1.3-23|munsell|0.5.1|
|Rcpp|1.0.13|nlme|3.1-165|
|SQUAREM|2021.1|nnet|7.3-19|
|TTR|0.24.4|notebookutils|1.1.11.34.20250605.2|
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

