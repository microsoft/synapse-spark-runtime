# System Environment
*   **Product**: Fabric Runtime 1.1 (Spark 3.3)
*   **Vhd Release**: Spark3.3-Rel-2024-10-02.1-rc.1
*   **Operating System**: Ubuntu 18.04.6 LTS
*   **Apache Spark**: 3.3.4
*   **Java**: 1.8.0_422
*   **Scala**: 2.12.15
*   **Python**: 3.10/1.0.6
*   **Delta Lake**: 2.2.0.17

*The end of support date for Runtime 1.1 has been announced as July 12, 2024. Runtime 1.1, based on Apache Spark 3.3, will be deprecated and disabled as of March 31, 2025. [**Upgrade your workspace**](https://learn.microsoft.com/en-us/fabric/data-engineering/runtime#multiple-runtimes-support) and environments to Runtime 1.2 or Runtime 1.3. For the complete lifecycle and support policies of Apache Spark runtimes in Fabric, refer to [**Lifecycle of Apache Spark runtimes in Fabric**](https://learn.microsoft.com/en-us/fabric/data-engineering/lifecycle).*
# New Features
|Id|Component|Description|
|-----|-----|-----|
|1444776|TokenLibrary:3.6.7|Enabling Reading and Writing Internal Log Files to SystemStorage account with shorter lived tokens  and SP Auth With Certs|
|1451954|ServiceConfigurationTemplates/spark/3.3.0:various|Set the Spark property to allow special characters in table names for Spark in Fabric.|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1467934|AutoscaleProbe:3.9.3|New Autoscale Version contains autoscale reliability fixes to reduce TJS and token library errors.|
|1450275|NotebookUtils:1.1.45|Support system hobo storage refresh sas token for mount v1|
|1466644|Wildfire/spark33:1.7.61|New Spark 3.3 component release, including improvements and fixes in Hadoop and Livy.|
|1464217|ComponentName:ComponentVersion|Enhance security for library snapshot sas token by encrypting it before passing it library management scripts|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1466644|Wildfire/spark33:1.7.61|New Spark 3.3 component release, including improvements and fixes in Hadoop and Livy.|
|1455145|LibraryManager:1.0.32|Library manager bug fix for library metadata cooker timeout issue|
|1455901|Wildfire/spark33:1.7.60|New Spark component release, including fixes in Hadoop, Spark and Livy including security fix|
|1448531|OneLakeClientStarter:spark3/1.0.23|Some paths containing special characters in friendly names were reported as File not found error. This issue is fixed in new OLC release.|
|1439924|DWConnector:2.1.5|Upgrade Synapse DW Connector to 2.1.5. Fixes temp files clean up after read and filter pushdown by removing unsupported Escape keyword from the SQL clauses constructed by the connector.|
|1445535|LibraryManager:1.0.30|Library Management bug fixes for Synapse DEP customers using custom conda channel setup on Azure Storage account|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|**AutoscaleProbe**|**3.9.2 ⬆️ 3.9.3**|MySQLJavaConnector|1.0.3|
|Autotune|1.11.1.2|**NotebookUtils**|**1.1.44 ⬆️ 1.1.45**|
|AzureMLExtensions|1.0.4|**OneLakeClientStarter**|**1.0.20 ⬆️ 1.0.23**|
|CDM|1.19.8|OnelakeSparkCatalog|0.1.10|
|CSparkMetricUpdate|1.0.5|Peregrine|0.10.4|
|ClusterGateway|spark/2.4.4|PostgreSQLJDBCDriver|1.0.3|
|Conda|1.0.21|Python|3.10/1.0.6|
|CosmosDBConnector|2.1.1|R|1.0.7|
|DSCopilotInstaller|1.0.0|SQLServerODBCDriver|18.1.0|
|**DWConnector**|**2.1.4.2 ⬆️ 2.1.5**|SStreamOnSparkJar|2.3.0.1|
|Delta|2.2.0.17|SparkAdvisor|1.0.0|
|Dotnet|6.0.0|SparkDiagnosticsLibrary|1.0.21|
|EventHubConnector|2.3.26|SparkInitialize|1.0.0|
|ExternalHiveMetastoreLibraries|0.0.7|SparkLighter|2.0.8|
|FabricDWConnector|1.0.10|SparkNativeParquetWriter|0.8.1.1|
|FsspecWrapper|1.0.13|SparkRPCHistoryServer|1.0.29|
|**Genesis**|**0.29.0 ⬆️ 0.32.1**|SparklyrConnector|1.0.1|
|HiveMetaStoreClient|1.1.21|**TokenLibrary**|**3.6.5 ⬆️ 3.6.7**|
|Impulse|1.2.4|TridentCore|1.2.9|
|KustoConnector|1.5.1|TridentTokenLibrary|1.9.4|
|**LibraryManager**|**1.0.28 ⬆️ 1.0.33**|VSANodeScanAgent|1.0.1|
|LibraryMetadataCooker|2.0.1|Vegas|3.3.09.01|
|MMLSpark|1.4.17|VertiParquet|0.8.6.1|
|MachineLearningPredict|1.0.2|**Wildfire**|**1.7.59 ⬆️ 1.7.61**|
|MlflowLibrary|2.1.1.1|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_openmp_mutex|4.5|libsqlite|3.40.0|
|_py-xgboost-mutex|2.0|libssh2|1.10.0|
|absl-py|1.4.0|libstdcxx-ng|12.2.0|
|adal|1.2.7|libsystemd0|253|
|adlfs|2023.1.0|libthrift|0.18.0|
|aiohttp|3.8.4|libtiff|4.5.0|
|aiosignal|1.3.1|libtool|2.4.7|
|alsa-lib|1.2.8|libudev1|253|
|anyio|3.6.2|libutf8proc|2.8.0|
|argcomplete|2.1.2|libuuid|2.38.1|
|argon2-cffi|21.3.0|libuv|1.44.2|
|argon2-cffi-bindings|21.2.0|libvorbis|1.3.7|
|arrow-cpp|11.0.0|libwebp|1.2.4|
|asttokens|2.2.1|libwebp-base|1.2.4|
|astunparse|1.6.3|libxcb|1.13|
|async-timeout|4.0.2|libxgboost|1.7.1|
|atk-1.0|2.38.0|libxkbcommon|1.5.0|
|attr|2.5.1|libxml2|2.10.3|
|attrs|22.2.0|libxslt|1.1.37|
|aws-c-auth|0.6.24|libzlib|1.2.13|
|aws-c-cal|0.5.20|lightgbm|3.3.3|
|aws-c-common|0.8.11|lime|0.2.0.1|
|aws-c-compression|0.2.16|llvm-openmp|16.0.1|
|aws-c-event-stream|0.2.18|llvmlite|0.39.1|
|aws-c-http|0.7.4|lxml|4.9.2|
|aws-c-io|0.13.17|lz4-c|1.9.4|
|aws-c-mqtt|0.8.6|markdown|3.4.1|
|aws-c-s3|0.2.4|markupsafe|2.1.2|
|aws-c-sdkutils|0.1.7|matplotlib|3.6.3|
|aws-checksums|0.1.14|matplotlib-base|3.6.3|
|aws-crt-cpp|0.19.7|matplotlib-inline|0.1.6|
|aws-sdk-cpp|1.10.57|mistune|2.0.5|
|azure-common|1.1.28|mkl|2022.2.1|
|azure-core|1.26.4|mlflow-skinny|2.1.1|
|azure-datalake-store|0.0.51|mpg123|1.31.3|
|azure-graphrbac|0.61.1|msal|1.21.0|
|azure-identity|1.12.0|msal_extensions|1.0.0|
|azure-mgmt-authorization|3.0.0|msgpack|1.0.5|
|azure-mgmt-containerregistry|10.1.0|msrest|0.7.1|
|azure-mgmt-core|1.4.0|msrestazure|0.6.4|
|azure-mgmt-keyvault|10.2.1|multidict|6.0.4|
|azure-mgmt-resource|21.2.1|multiprocess|0.70.14|
|azure-mgmt-storage|20.1.0|munkres|1.1.4|
|azure-storage-blob|12.15.0|mypy|0.780|
|azure-storage-file-datalake|12.9.1|mypy-extensions|0.4.4|
|azure-synapse-ml-predict|1.0.0|mysql-common|8.0.32|
|azureml-core|1.49.0|mysql-libs|8.0.32|
|azureml-synapse|0.0.1|nbclient|0.7.3|
|backcall|0.2.0|nbconvert-core|7.3.0|
|backports|1.0|nbformat|5.8.0|
|backports-tempfile|1.0|ncurses|6.3|
|backports-weakref|1.0.post1|ndg-httpsclient|0.5.1|
|backports.functools_lru_cache|1.6.4|nest-asyncio|1.5.6|
|bcrypt|3.2.2|**notebookutils**|**1.0.34.33.20240612.3 ⬆️ 1.0.34.33.20240905.1**|
|beautifulsoup4|4.11.2|nspr|4.35|
|bleach|6.0.0|nss|3.89|
|blinker|1.6.1|numba|0.56.4|
|brotli|1.0.9|numpy|1.23.5|
|brotli-bin|1.0.9|oauthlib|3.2.2|
|brotli-python|1.0.9|openjpeg|2.5.0|
|brotlipy|0.7.0|openpyxl|3.1.0|
|bzip2|1.0.8|openssl|3.1.0|
|c-ares|1.18.1|opt_einsum|3.3.0|
|ca-certificates|2022.12.7|orc|1.8.2|
|cached-property|1.5.2|packaging|21.3|
|cached_property|1.5.2|pandas|1.5.3|
|cachetools|5.3.0|pandasql|0.7.3|
|cairo|1.16.0|pandocfilters|1.5.0|
|certifi|2022.12.7|pango|1.50.14|
|cffi|1.15.1|paramiko|2.12.0|
|charset-normalizer|2.1.1|parquet-cpp|1.5.1|
|click|8.1.3|parso|0.8.3|
|cloudpickle|2.2.1|pathos|0.3.0|
|colorama|0.4.6|pathspec|0.11.1|
|comm|0.1.3|patsy|0.5.3|
|conda-package-handling|2.0.2|pcre2|10.40|
|conda-package-streaming|0.7.0|pexpect|4.8.0|
|configparser|5.3.0|pickleshare|0.7.5|
|contextlib2|21.6.0|pillow|9.4.0|
|contourpy|1.0.7|pip|23.0.1|
|cryptography|40.0.1|pixman|0.40.0|
|cycler|0.11.0|pkginfo|1.9.6|
|dash|2.9.2|pkgutil-resolve-name|1.3.10|
|dash-core-components|2.0.0|platformdirs|3.2.0|
|dash-html-components|2.0.0|plotly|5.13.0|
|dash-table|5.0.0|ply|3.11|
|dash_cytoscape|0.2.0|pooch|1.7.0|
|databricks-cli|0.17.6|portalocker|2.7.0|
|dbus|1.13.6|pox|0.3.2|
|debugpy|1.6.7|ppft|1.7.6.6|
|decorator|5.1.1|prettytable|3.6.0|
|defusedxml|0.7.1|prometheus_client|0.16.0|
|dill|0.3.6|prompt-toolkit|3.0.38|
|distlib|0.3.6|protobuf|4.21.12|
|docker-py|6.0.0|psutil|5.9.4|
|dscopilot-installer|0.0.7|pthread-stubs|0.4|
|entrypoints|0.4|ptyprocess|0.7.0|
|et_xmlfile|1.1.0|pulseaudio|16.1|
|executing|1.2.0|pulseaudio-client|16.1|
|expat|2.5.0|pulseaudio-daemon|16.1|
|fftw|3.3.10|pure_eval|0.2.2|
|filelock|3.11.0|py-xgboost|1.7.1|
|flask|2.2.3|py4j|0.10.9.5|
|flask-compress|1.13|pyarrow|11.0.0|
|flatbuffers|22.12.06|pyasn1|0.4.8|
|flit-core|3.8.0|pyasn1-modules|0.2.7|
|fluent-logger|0.10.0|pycosat|0.6.4|
|font-ttf-dejavu-sans-mono|2.37|pycparser|2.21|
|font-ttf-inconsolata|3.000|pygments|2.14.0|
|font-ttf-source-code-pro|2.038|pyjwt|2.6.0|
|font-ttf-ubuntu|0.83|pynacl|1.5.0|
|fontconfig|2.14.2|pyodbc|4.0.35|
|fonts-conda-ecosystem|1|pyopenssl|23.1.1|
|fonts-conda-forge|1|pyparsing|3.0.9|
|fonttools|4.39.3|pyperclip|1.8.2|
|freetype|2.12.1|pyqt|5.15.7|
|fribidi|1.0.10|pyqt5-sip|12.11.0|
|frozenlist|1.3.3|pyrsistent|0.19.3|
|fsspec|2023.4.0|pysocks|1.7.1|
|fsspec_wrapper|0.1.9|pyspark|3.3.1|
|gast|0.4.0|python|3.10.10|
|gdk-pixbuf|2.42.10|python-dateutil|2.8.2|
|geographiclib|1.52|python-fastjsonschema|2.16.3|
|geopy|2.3.0|python-flatbuffers|23.1.21|
|gettext|0.21.1|python-graphviz|0.20.1|
|gevent|22.10.2|python-json-logger|2.0.7|
|gflags|2.2.2|python_abi|3.10|
|giflib|5.2.1|pytorch|1.13.1|
|gitdb|4.0.10|pytz|2022.7.1|
|gitpython|3.1.31|pyu2f|0.1.5|
|glib|2.74.1|pywin32-on-windows|0.1.0|
|glib-tools|2.74.1|pyyaml|6.0|
|glog|0.6.0|pyzmq|25.0.2|
|google-auth|2.17.2|qt-main|5.15.8|
|google-auth-oauthlib|0.4.6|re2|2023.02.01|
|google-pasta|0.2.0|readline|8.2|
|graphite2|1.3.13|regex|2022.10.31|
|graphviz|2.50.0|requests|2.28.2|
|greenlet|2.0.2|requests-oauthlib|1.3.1|
|grpcio|1.51.1|rfc3339-validator|0.1.4|
|gson|0.0.3|rfc3986-validator|0.1.1|
|gst-plugins-base|1.22.0|rsa|4.9|
|gstreamer|1.22.0|ruamel.yaml|0.17.21|
|gstreamer-orc|0.4.33|ruamel.yaml.clib|0.2.7|
|gtk2|2.24.33|ruamel_yaml|0.15.80|
|gts|0.7.6|s2n|1.3.37|
|h5py|3.8.0|salib|1.4.7|
|harfbuzz|6.0.0|scikit-learn|1.2.0|
|hdf5|1.14.0|scipy|1.10.1|
|html5lib|1.1|seaborn|0.12.2|
|humanfriendly|10.0|seaborn-base|0.12.2|
|icu|70.1|secretstorage|3.3.3|
|idna|3.4|send2trash|1.8.0|
|imageio|2.25.0|setuptools|67.6.1|
|importlib-metadata|5.2.0|shap|0.41.0|
|importlib_metadata|5.2.0|sip|6.7.7|
|importlib_resources|5.12.0|six|1.16.0|
|impulse-python-handler|1.0.22.1.0.0|sleef|3.5.1|
|interpret|0.3.1|slicer|0.0.7|
|interpret-core|0.3.1|smmap|3.0.5|
|ipykernel|6.22.0|snappy|1.1.10|
|ipython|8.9.0|sniffio|1.3.0|
|ipywidgets|8.0.4|soupsieve|2.3.2.post1|
|isodate|0.6.1|sqlalchemy|2.0.9|
|itsdangerous|2.1.2|sqlanalyticsconnectorpy|1.0.1|
|jack|1.9.22|sqlparse|0.4.3|
|jedi|0.18.2|stack_data|0.6.2|
|jeepney|0.8.0|statsmodels|0.13.5|
|jinja2|3.1.2|synapseml-cognitive|1.0.4.dev1|
|jmespath|1.0.1|synapseml-core|1.0.4.dev1|
|joblib|1.2.0|synapseml-deep-learning|1.0.4.dev1|
|jpeg|9e|synapseml-internal|1.0.4.0.dev1|
|jsonpickle|2.2.0|synapseml-lightgbm|1.0.4.dev1|
|jsonschema|4.17.3|synapseml-mlflow|1.0.23|
|jupyter_client|8.1.0|synapseml-opencv|1.0.4.dev1|
|jupyter_core|5.3.0|synapseml-utils|1.0.19.post1|
|jupyter_events|0.6.3|synapseml-vw|1.0.4.dev1|
|jupyter_server|2.2.1|tabulate|0.9.0|
|jupyter_server_terminals|0.4.4|tbb|2021.8.0|
|jupyterlab_pygments|0.2.2|tenacity|8.2.2|
|jupyterlab_widgets|3.0.7|tensorboard|2.11.2|
|keras|2.11.0|tensorboard-data-server|0.6.1|
|keras-preprocessing|1.1.2|tensorboard-plugin-wit|1.8.1|
|keyutils|1.6.1|tensorflow|2.11.0|
|kiwisolver|1.4.4|tensorflow-base|2.11.0|
|knack|0.10.1|tensorflow-estimator|2.11.0|
|krb5|1.20.1|termcolor|2.2.0|
|lame|3.100|terminado|0.17.1|
|lcms2|2.15|threadpoolctl|3.1.0|
|ld_impl_linux-64|2.40|tinycss2|1.2.1|
|lerc|4.0.0|tk|8.6.12|
|liac-arff|2.5.0|toml|0.10.2|
|libabseil|20220623.0|toolz|0.12.0|
|libaec|1.0.6|tornado|6.2|
|libarrow|11.0.0|tqdm|4.65.0|
|libblas|3.9.0|traitlets|5.9.0|
|libbrotlicommon|1.0.9|treeinterpreter|0.2.2|
|libbrotlidec|1.0.9|typed-ast|1.4.3|
|libbrotlienc|1.0.9|typing-extensions|4.5.0|
|libcap|2.67|typing_extensions|4.5.0|
|libcblas|3.9.0|tzdata|2023c|
|libclang|15.0.7|unicodedata2|15.0.0|
|libclang13|15.0.7|unixodbc|2.3.10|
|libcrc32c|1.1.2|urllib3|1.26.14|
|libcups|2.3.3|virtualenv|20.19.0|
|libcurl|7.88.1|wcwidth|0.2.6|
|libdb|6.2.32|webencodings|0.5.1|
|libdeflate|1.17|websocket-client|1.5.1|
|libebm|0.3.1|werkzeug|2.2.3|
|libedit|3.1.20191231|wheel|0.40.0|
|libev|4.33|widgetsnbextension|4.0.7|
|libevent|2.1.10|wrapt|1.15.0|
|libexpat|2.5.0|xcb-util|0.4.0|
|libffi|3.4.2|xcb-util-image|0.4.0|
|libflac|1.4.2|xcb-util-keysyms|0.4.0|
|libgcc-ng|12.2.0|xcb-util-renderutil|0.3.9|
|libgcrypt|1.10.1|xcb-util-wm|0.4.1|
|libgd|2.3.3|xgboost|1.7.1|
|libgfortran-ng|12.2.0|xkeyboard-config|2.38|
|libgfortran5|12.2.0|xorg-kbproto|1.0.7|
|libglib|2.74.1|xorg-libice|1.0.10|
|libgoogle-cloud|2.7.0|xorg-libsm|1.2.3|
|libgpg-error|1.46|xorg-libx11|1.8.4|
|libgrpc|1.51.1|xorg-libxau|1.0.9|
|libhwloc|2.9.0|xorg-libxdmcp|1.1.3|
|libiconv|1.17|xorg-libxext|1.3.4|
|liblapack|3.9.0|xorg-libxrender|0.9.10|
|libllvm11|11.1.0|xorg-renderproto|0.11.1|
|libllvm15|15.0.7|xorg-xextproto|7.3.0|
|libnghttp2|1.52.0|xorg-xproto|7.0.31|
|libnsl|2.0.0|xz|5.2.6|
|libogg|1.3.4|yaml|0.2.5|
|libopenblas|0.3.21|yarl|1.8.2|
|libopus|1.3.1|zeromq|4.3.4|
|libpng|1.6.39|zipp|3.15.0|
|libpq|15.2|zlib|1.2.13|
|libprotobuf|3.21.12|zope.event|4.6|
|library-metadata-cooker|3.3.1.3|zope.interface|6.0|
|librsvg|2.54.4|zstandard|0.19.0|
|libsndfile|1.2.0|zstd|1.5.2|
|libsodium|1.0.18|_libgcc_mutex|0.1|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|json-simple|1.1.1|
|JLargeArrays|1.5|json-simple|1.1|
|JTransforms|3.1|json4s-ast|2.12-3.7.0-M11|
|RoaringBitmap|0.9.25|json4s-core|2.12-3.7.0-M11|
|ST4|4.0.4|json4s-jackson|2.12-3.7.0-M11|
|SparkCustomEvents|3.3.0-1.0.4|json4s-scalap|2.12-3.7.0-M11|
|**TokenLibrary-assembly**|**3.6.5 ⬆️ 3.6.7**|jsr305|3.0.0|
|VegasConnector|3.3.09|jta|1.1|
|activation|1.1.1|jul-to-slf4j|1.7.32|
|aircompressor|0.21|junit-jupiter|5.5.2|
|algebra|2.12-2.0.1|junit-jupiter-api|5.5.2|
|aliyun-java-sdk-core|4.5.10|junit-jupiter-engine|5.5.2|
|aliyun-java-sdk-kms|2.11.0|junit-jupiter-params|5.5.2|
|aliyun-java-sdk-ram|3.1.0|junit-platform-commons|1.5.2|
|aliyun-sdk-oss|3.13.0|junit-platform-engine|1.5.2|
|annotations|7.0.0|kafka-clients|2.8.1|
|antlr-runtime|3.5.2|kryo-shaded|4.0.2|
|antlr4-runtime|4.8|kusto-spark|3.0_2.12-5.2.2-SNAPSHOT|
|aopalliance-repackaged|2.6.1|lapack|2.2.1|
|apiguardian-api|1.1.0|leveldbjni-all|1.8|
|arpack|2.2.1|libfb303|0.9.3|
|arpack_combined_all|0.1|libthrift|0.12.0|
|arrow-format|7.0.0|lightgbmlib|3.3.510|
|arrow-memory-core|7.0.0|log4j|1.2-api-2.17.2|
|arrow-memory-netty|7.0.0|log4j-api|2.17.2|
|arrow-vector|7.0.0|log4j-core|2.17.2|
|audience-annotations|0.5.0|log4j-slf4j-impl|2.17.2|
|autotune-client|2.12-1.11.1-3.3-125200601|lz4-java|1.8.0|
|autotune-common|2.12-1.11.1-3.3-125200601|mdsdclientdynamic|2.0|
|avro|1.11.0|metrics-core|4.2.7|
|avro-ipc|1.11.0|metrics-graphite|4.2.7|
|avro-mapred|1.11.0|metrics-jmx|4.2.7|
|aws-java-sdk-bundle|1.12.262|metrics-json|4.2.7|
|azure-cosmos-analytics-spark|3_2-12_synapse-2.1.1|metrics-jvm|4.2.7|
|azure-data-lake-store-sdk|2.3.9|microsoft-catalog-metastore-client|1.1.21|
|azure-eventhubs|3.3.0|microsoft-log4j-etwappender|1.0|
|azure-eventhubs-spark|2.12-2.3.22|minlog|1.3.0|
|azure-keyvault-core|1.0.0|mlflow-spark|2.1.1|
|azure-storage|7.0.1|mysql-connector-java|8.0.18|
|azure-synapse-ml-pandas|2.12-0.1.1|netty-all|4.1.74.Final|
|azure-synapse-ml-predict|2.12-1.0|netty-buffer|4.1.74.Final|
|blas|2.2.1|netty-codec|4.1.74.Final|
|bonecp|0.8.0.RELEASE|netty-common|4.1.74.Final|
|breeze|2.12-1.2|netty-handler|4.1.74.Final|
|breeze-macros|2.12-1.2|netty-resolver|4.1.74.Final|
|cats-kernel|2.12-2.1.1|netty-tcnative-classes|2.0.48.Final|
|chill|2.12-0.10.0|netty-transport|4.1.74.Final|
|chill-java|0.10.0|netty-transport-classes-epoll|4.1.74.Final|
|client-sdk|1.24.1|netty-transport-classes-kqueue|4.1.74.Final|
|commons-cli|1.5.0|netty-transport-native-epoll|4.1.74.Final-linux-x86_64|
|commons-codec|1.15|netty-transport-native-epoll|4.1.74.Final-linux-aarch_64|
|commons-collections|3.2.2|netty-transport-native-kqueue|4.1.74.Final-osx-x86_64|
|commons-collections4|4.4|netty-transport-native-kqueue|4.1.74.Final-osx-aarch_64|
|commons-compiler|3.0.16|netty-transport-native-unix-common|4.1.74.Final|
|commons-compress|1.21|**notebook-utils**|**1.0.34-spark33-20240612.3 ⬆️ 1.0.34-spark33-20240905.1**|
|commons-crypto|1.1.0|objenesis|3.2|
|commons-dbcp|1.4|onnx-protobuf|2.12-0.9.3|
|commons-io|2.11.0|onnxruntime_gpu|1.8.1|
|commons-lang|2.6|opencsv|2.3|
|commons-lang3|3.12.0|opencv|3.2.0-1|
|commons-logging|1.1.3|opentest4j|1.2.0|
|commons-math3|3.6.1|opentracing-api|0.33.0|
|commons-pool|1.5.4|opentracing-noop|0.33.0|
|commons-pool2|2.11.1|opentracing-util|0.33.0|
|commons-text|1.10.0|orc-core|1.7.10|
|compress-lzf|1.1|orc-mapreduce|1.7.10|
|core|1.1.2|orc-shims|1.7.10|
|curator-client|2.13.0|oro|2.0.8|
|curator-framework|2.13.0|osgi-resource-locator|1.0.3|
|curator-recipes|2.13.0|paranamer|2.8|
|datanucleus-api-jdo|4.2.4|parquet-column|1.12.3|
|datanucleus-core|4.1.17|parquet-common|1.12.3|
|datanucleus-rdbms|4.1.19|parquet-encoding|1.12.3|
|delta-core|2.12-2.2.0.17|parquet-format-structures|1.12.3|
|delta-iceberg|2.12-2.2.0.17|parquet-hadoop|1.12.3|
|delta-storage|2.2.0.17|parquet-jackson|1.12.3|
|derby|0.14.2.0|peregrine-spark|3.3.0-0.10.3|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|pickle|1.2|
|flatbuffers-java|1.12.0|postgresql|2.2.9|
|fluent-logger-jar-with-dependencies-jdk8|8|protobuf-java|2.5.0|
|**genesis-client**|**2.12-0.28.0-jar-with-dependencies ⬆️ 2.12-0.32.1-jar-with-dependencies**|proton-j|0.33.8|
|gluten-velox-bundle-spark|3.3_2.12-ubuntu_18.04-0.5.0-SNAPSHOT|py4j|0.10.9.5|
|gson|2.8.9|qpid-proton-j-extensions|1.2.4|
|guava|4.0.1|rocksdbjni|6.20.3|
|**hadoop-aliyun**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scala-collection-compat|2.12-2.1.1|
|**hadoop-annotations**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scala-compiler|2.12.15|
|**hadoop-aws**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scala-java8-compat|2.12-0.9.0|
|**hadoop-azure**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scala-library|2.12.15|
|**hadoop-azure-datalake**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scala-parser-combinators|2.12-1.1.2|
|hadoop-azureml|1.0-fs|scala-reflect|2.12.15|
|**hadoop-client-api**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scala-xml|2.12-1.2.0|
|**hadoop-client-runtime**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|scalactic|2.12-3.2.14|
|**hadoop-cloud-storage**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|shapeless|2.12-2.3.7|
|**hadoop-openstack**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|shims|0.9.25|
|hadoop-shaded-guava|1.1.1|slf4j-api|1.7.32|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.2.20240814.5 ⬆️ 3.3.4.5.2.20240924.1**|snappy-java|1.1.10.5|
|hdinsight-spark-metrics|3.3.0-1.0.4|spark|3.3-rpc-history-server-app-listener_2.12-1.0.0|
|hive-beeline|2.3.9|spark|3.3-rpc-history-server-core_2.12-1.0.0|
|hive-cli|2.3.9|spark|3.3-advisor-core_2.12-1.0.18|
|hive-common|2.3.9|**spark-avro**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-exec|2.3.9-core|**spark-catalyst**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-jdbc|2.3.9|spark-cdm-connector-assembly-spark|3.3-1.19.7|
|hive-llap-common|2.3.9|**spark-core**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-metastore|2.3.9|**spark-enhancement**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-serde|2.3.9|spark-enhancementui|2.12-3.0.0|
|hive-service-rpc|3.1.2|**spark-graphx**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-shims|0.23-2.3.9|**spark-hadoop-cloud**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-shims|2.3.9|**spark-hive**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-shims-common|2.3.9|**spark-hive-thriftserver**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-shims-scheduler|2.3.9|spark-kusto-synapse-connector|3.0_2.12-1.5.1|
|hive-storage-api|2.7.2|**spark-kvstore**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hive-vector-code-gen|2.3.9|**spark-launcher**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|hk2-api|2.6.1|spark-lighter-contract|2.12-2.0.8_spark-3.3.0_20240704.2|
|hk2-locator|2.6.1|spark-lighter-core|2.12-2.0.11_spark-3.3.0_20240704.2|
|hk2-utils|2.6.1|**spark-microsoft-tools**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|httpclient|4.5.13|**spark-mllib**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|httpclient5|5.1.3|**spark-mllib-local**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|httpcore|4.4.14|**spark-network-common**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|httpmime|4.5.13|**spark-network-shuffle**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|impulse-core_spark|3.3_2.12-1.0.22|**spark-repl**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|impulse-telemetry-mds_spark|3.3_2.12-1.0.22|**spark-sketch**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|ini4j|0.5.4|**spark-sql**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|isolation-forest|3.3.3_2.12-3.0.4|**spark-sql-kafka**|**0_2.12-3.3.4.5.2.20240814.5 ⬆️ 0_2.12-3.3.4.5.2.20240924.1**|
|istack-commons-runtime|3.0.8|**spark-streaming**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|ivy|2.5.1|**spark-streaming-kafka**|**0_2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|jackson-annotations|2.13.4|**spark-streaming-kafka**|**0_2.12-3.3.4.5.2.20240814.5 ⬆️ 0_2.12-3.3.4.5.2.20240924.1**|
|jackson-core|2.13.4|**spark-tags**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|jackson-core-asl|1.9.13|**spark-token-provider-kafka**|**0_2.12-3.3.4.5.2.20240814.5 ⬆️ 0_2.12-3.3.4.5.2.20240924.1**|
|jackson-databind|2.13.4.2|**spark-unsafe**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|jackson-dataformat-cbor|2.13.4|**spark-yarn**|**2.12-3.3.4.5.2.20240814.5 ⬆️ 2.12-3.3.4.5.2.20240924.1**|
|jackson-mapper-asl|1.9.13|spark_diagnostic_cli|2.1.0_spark-3.3.0_20240705.2|
|jackson-module-scala|2.12-2.13.4|sparklyr-connector|3.3.1-1.0.0274143|
|jakarta.annotation-api|1.3.5|sparknativeparquetwriter|2.12-0.8.1-spark-3.3|
|jakarta.inject|2.6.1|spire|2.12-0.17.0|
|jakarta.servlet-api|4.0.3|spire-macros|2.12-0.17.0|
|jakarta.validation-api|2.0.2|spire-platform|2.12-0.17.0|
|jakarta.ws.rs-api|2.1.6|spire-util|2.12-0.17.0|
|jakarta.xml.bind-api|2.3.2|spray-json|2.12-1.3.5|
|janino|3.0.16|stax-api|1.0.1|
|javassist|3.25.0-GA|stream|2.9.6|
|javatuples|1.2|structuredstreamforspark|2.12-3.2.0-2.3.0|
|javax.jdo|3.2.0-m3|super-csv|2.2.0|
|javolution|5.5.1|synapseml-cognitive|2.12-1.0.4-spark3.3|
|jaxb-api|2.2.11|synapseml-core|2.12-1.0.4-spark3.3|
|jaxb-runtime|2.3.2|synapseml-deep-learning|2.12-1.0.4-spark3.3|
|jcl-over-slf4j|1.7.32|synapseml-internal|2.12-1.0.4.0-spark3.3|
|jdo-api|3.0.1|synapseml-lightgbm|2.12-1.0.4-spark3.3|
|jdom2|2.0.6|synapseml-opencv|2.12-1.0.4-spark3.3|
|jersey-client|2.36|synapseml-vw|2.12-1.0.4-spark3.3|
|jersey-common|2.36|**synfs**|**1.0.34-spark33-20240612.3 ⬆️ 1.0.34-spark33-20240905.1**|
|jersey-container-servlet|2.36|threeten-extra|1.5.0|
|jersey-container-servlet-core|2.36|tink|1.6.1|
|jersey-hk2|2.36|transaction-api|1.1|
|jersey-server|2.36|trident-core|1.2.9|
|jettison|1.1|tridenttokenlibrary-assembly|1.9.4|
|jetty-util|9.4.53.v20231009|univocity-parsers|2.9.1|
|jetty-util-ajax|9.4.53.v20231009|velocity|1.5|
|jline|2.14.6|vw-jni|9.3.0|
|joda-time|2.10.13|wildfly-openssl|1.0.7.Final|
|jodd-core|3.5.2|xbean-asm9-shaded|4.20|
|jpam|1.1|xz|1.9|
|jsch|0.1.54|**zookeeper**|**3.6.3.5.2.20240814.5 ⬆️ 3.6.3.5.2.20240924.1**|
|json|1|**zookeeper-jute**|**3.6.3.5.2.20240814.5 ⬆️ 3.6.3.5.2.20240924.1**|
|json|3|zstd-jni|1.5.2-1|
|json|1.8|

# R Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|DBI|1.2.1|lightgbm|3.3.4|
|DiceDesign|1.10|listenv|0.9.1|
|FabricTelemetry|1.0.2|lobstr|1.1.2|
|GPfit|1.0-8|lubridate|1.9.3|
|KernSmooth|2.23-22|magrittr|2.0.3|
|MASS|7.3-60.0.1|maps|3.4.2|
|Matrix|1.6-5|markdown|1.12|
|ModelMetrics|1.2.2.2|memoise|2.0.1|
|R.methodsS3|1.8.2|methods|4.2.3|
|R.oo|1.26.0|mgcv|1.9-1|
|R.utils|2.12.3|mime|0.12|
|R6|2.5.1|miniUI|0.1.1.1|
|R6P|0.3.0|modeldata|1.3.0|
|RColorBrewer|1.1-3|modelenv|0.1.1|
|RODBC|1.3-20|modelr|0.1.11|
|Rcpp|1.0.12|munsell|0.5.0|
|SQUAREM|2021.1|nlme|3.1-164|
|TTR|0.24.4|nnet|7.3-19|
|V8|4.4.1|**notebookutils**|**1.0.34.33.20240612.3 ⬆️ 1.0.34.33.20240905.1**|
|XML|3.99-0.16.1|numDeriv|2016.8-1.1|
|arrow|10.0.1|openssl|2.1.1|
|askpass|1.2.0|pROC|1.18.5|
|assertthat|0.2.1|parallel|4.2.3|
|backports|1.4.1|parallelly|1.36.0|
|base|4.2.3|parsnip|1.1.1|
|base64enc|0.1-3|patchwork|1.2.0|
|bigD|0.2.0|pillar|1.9.0|
|bit|4.0.5|pkgbuild|1.4.2|
|bit64|4.0.5|pkgconfig|2.0.3|
|bitops|1.0-7|pkgdown|2.0.7|
|blob|1.2.4|pkgload|1.3.4|
|brew|1.0-10|plotly|4.10.1|
|brio|1.1.4|plyr|1.8.9|
|broom|1.0.5|praise|1.0.0|
|bslib|0.6.1|prettyunits|1.2.0|
|cachem|1.0.8|processx|3.8.3|
|callr|3.7.3|prodlim|2023.08.28|
|caret|6.0-93|profvis|0.3.8|
|cellranger|1.1.0|progress|1.2.3|
|class|7.3-22|progressr|0.14.0|
|cli|3.6.2|promises|1.2.1|
|clipr|0.8.0|proxy|0.4-27|
|clock|0.7.0|pryr|0.1.6|
|codetools|0.2-19|ps|1.7.6|
|collections|0.3.7|purrr|1.0.2|
|colorspace|2.1-0|quantmod|0.4.25|
|commonmark|1.9.1|r2d3|0.2.6|
|compiler|4.2.3|ragg|1.2.7|
|config|0.3.2|rappdirs|0.3.3|
|conflicted|1.2.0|rbokeh|0.5.2|
|coro|1.0.3|rcmdcheck|1.4.0|
|cpp11|0.4.7|reactR|0.5.0|
|crayon|1.5.2|reactable|0.4.4|
|credentials|2.0.1|readr|2.1.5|
|crosstalk|1.2.1|readxl|1.4.3|
|crul|1.4.0|recipes|1.0.9|
|curl|5.1.0|rematch|2.0.0|
|data.table|1.14.10|rematch2|2.1.2|
|datasets|4.2.3|remotes|2.4.2.1|
|dbplyr|2.3.4|reprex|2.1.0|
|desc|1.4.3|reshape2|1.4.4|
|devtools|2.4.5|rjson|0.2.21|
|diagram|1.6.5|rlang|1.1.3|
|dials|1.2.0|rlist|0.4.6.2|
|diffobj|0.3.5|rmarkdown|2.19|
|digest|0.6.34|roxygen2|7.3.1|
|downlit|0.4.3|rpart|4.1.23|
|dplyr|1.1.4|rprojroot|2.0.4|
|dtplyr|1.3.1|rsample|1.2.0|
|e1071|1.7-14|rstudioapi|0.15.0|
|ellipsis|0.3.2|rversions|2.1.2|
|evaluate|0.23|rvest|1.0.3|
|fansi|1.0.6|sass|0.4.8|
|farver|2.1.1|scales|1.3.0|
|fastmap|1.1.1|selectr|0.4-2|
|fontawesome|0.5.2|sessioninfo|1.2.2|
|forcats|1.0.0|shape|1.4.6|
|foreach|1.5.2|shiny|1.8.0|
|forge|0.2.0|slider|0.3.1|
|fs|1.6.3|sourcetools|0.1.7-1|
|furrr|0.3.1|sparklyr|1.8.2|
|future|1.33.1|splines|4.2.3|
|future.apply|1.11.1|stats|4.2.3|
|gargle|1.5.2|stats4|4.2.3|
|generics|0.1.3|stringi|1.8.3|
|gert|2.0.1|stringr|1.5.1|
|ggplot2|3.4.0|survival|3.5-7|
|gh|1.4.0|sys|3.4.2|
|gistr|0.9.0|systemfonts|1.0.5|
|gitcreds|0.1.2|tcltk|4.2.3|
|globals|0.16.2|testthat|3.2.1|
|glue|1.7.0|textshaping|0.3.7|
|googledrive|2.1.1|tibble|3.2.1|
|googlesheets4|1.1.1|tidymodels|1.0.0|
|gower|1.0.1|tidyr|1.3.1|
|grDevices|4.2.3|tidyselect|1.2.0|
|graphics|4.2.3|tidyverse|1.3.2|
|grid|4.2.3|timeDate|4032.109|
|gt|0.9.0|timechange|0.3.0|
|gtable|0.3.4|tinytex|0.49|
|hardhat|1.3.0|tools|4.2.3|
|haven|2.5.4|torch|0.9.0|
|hexbin|1.28.3|triebeard|0.4.1|
|highcharter|0.9.4|tune|1.1.2|
|highr|0.10|tzdb|0.4.0|
|hms|1.1.3|urlchecker|1.0.1|
|htmltools|0.5.7|urltools|1.7.3|
|htmlwidgets|1.6.4|usethis|2.2.2|
|httpcode|0.3.0|utf8|1.2.4|
|httpuv|1.6.14|utils|4.2.3|
|httr|1.4.7|uuid|1.2-0|
|httr2|1.0.0|vctrs|0.6.5|
|ids|1.0.1|viridisLite|0.4.2|
|igraph|1.5.1|vroom|1.6.5|
|infer|1.0.6|waldo|0.5.2|
|ini|0.3.1|warp|0.2.1|
|ipred|0.9-14|whisker|0.4.1|
|isoband|0.2.7|withr|3.0.0|
|iterators|1.0.14|workflows|1.1.3|
|jose|1.2.0|workflowsets|1.0.1|
|jquerylib|0.1.4|xfun|0.41|
|jsonlite|1.8.8|xgboost|1.7.1.1|
|juicyjuice|0.1.0|xml2|1.3.6|
|knitr|1.45|xopen|1.0.0|
|labeling|0.4.3|xtable|1.8-4|
|later|1.3.2|xts|0.13.2|
|lattice|0.22-5|yaml|2.3.8|
|lava|1.7.3|yardstick|1.3.0|
|lazyeval|0.2.2|zip|2.3.1|
|lhs|1.1.6|zoo|1.8-12|
|lifecycle|1.0.4|

