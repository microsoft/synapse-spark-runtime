# System Environment
*   **Product**: Fabric Runtime 2.0 (Spark 4.1)
*   **VHD Name**: c31497428ef5c0.vhd
*   **Vhd Release**: Spark4.1-default-2026-07-20.0-rc.1
*   **Operating System**: Azure Linux 3.0
*   **Apache Spark**: 4.1.1
*   **Java**: 21.0.11
*   **Scala**: 2.13.17
*   **Python**: 3.13/1.0.0
*   **Delta Lake**: 4.2.0.20260714.2

# Improvements
|Id|Component|Description|
|-----|-----|-----|
|2193654|Impulse:1.5.226604159|Updates the Impulse diagnostics/telemetry library for the Spark 4.1 VHD to version `1.5.226604159` (latest official Impulse build, tag `v1.5.226604159`, published 2026-07-13).|
|2190667|FLTSparkExtensions:1.7.1|Release new version 1.7.1 of FLTSparkExtensions with File Ingestion (DFI), column-level Data Quality, reliability and shield-test improvements|
|2193144|delta:4.2.0.20260713.2|Updates Delta to the latest official release.|
|2197640|delta:4.2.0.20260714.2|Updates Delta to the latest official release.|
|2167386|ComponentName:ComponentVersion|Syncing spark 3.5 changes in spark4.1 for eventStream Adapter. Adding spark 4.1 dependencies, Cross workspace feature, Private Link support.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|2202597|Genesis:2.0.4, LibraryManager:1.0.18|Fixes library personalization failing during autoscale scale-up on Spark 4.1, and ensures the library-cleanup behavior chosen at deployment is honored when the cluster scales up.|
|2193678|LakeMetastore:0.4.16, TridentCore:1.4.4|Forces the use of FQDN based endpoints for Onelake and Platform APIs with changes put behind a Feature flag `spark.sql.fabric.catalog.enable-private-vnet-endpoints`|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|AutoscaleProbe|3.9.10|R|1.0.3|
|**Conda**|**10.0.0 ⬆️ 11.0.0**|SparkAdvisor|1.0.5|
|**CSparkMetricUpdate**|**1.0.2.210061716 ⬆️ 1.0.3.226407580**|SparkDiagnosticsLibrary|1.2.1|
|**Delta**|**4.2.0.20260630.5 ⬆️ 4.2.0.20260714.2**|SparkJobInsight|2.0.0|
|Esri|2.0.0|SparkLineage|1.0.0|
|EventStreamsFabricExtension|4.1.1|SparklyrConnector|1.0.0|
|FabricDWConnector|1.0.25|SparkNativeParquetWriter|4.1.0-20260429.1|
|FLTDeequ|2.0.18.1-msft|SparkRPCHistoryServer|41.2.0|
|**FLTSparkExtensions**|**1.6.1 ⬆️ 1.7.1**|SparkSqlConnector|1.1.0.217307560|
|FLTSparkUtils|0.4.0|SQLServerODBCDriver|18.1.0|
|FsspecWrapper|2.0.0|SStreamOnSparkJar|3.1.2|
|**Genesis**|**2.0.3 ⬆️ 2.0.4**|TokenLibrary|5.0.0|
|**GlutenUI**|**1.6.0-20260630.3 ⬆️ 1.6.0-20260718.1**|**TridentCore**|**1.3.4 ⬆️ 1.4.4**|
|HiveMetaStoreClient|1.1.21.2|TridentTokenLibrary|2.5.1|
|Iceberg|1.11.0|UpgradeToFabric|1.2.15|
|**Impulse**|**1.5.223168344 ⬆️ 1.5.226604159**|Vegas|4.1.0.01|
|KustoConnector|2.1.0|**Wildfire**|**1.10.55 ⬆️ 1.10.59**|
|**LibraryManager**|**1.0.17 ⬆️ 1.0.18**|
|LibraryMetadataCooker|1.0.0|
|MlflowLibrary|2.18.0.1|
|MMLSpark|1.4.28|
|NotebookUtils|1.1.15.20260524.4|
|OneLakeClientStarter|1.0.28.0|
|**OnelakeSparkCatalog**|**0.4.14 ⬆️ 0.4.16**|
|Python|3.13/1.0.0|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_openmp_mutex|4.5|openpyxl|3.1.5|
|_py-xgboost-mutex|2.0|openssl|3.6.3|
|_python_abi3_support|1.0|opentelemetry-api|1.16.0|
|adwaita-icon-theme|49.0|opentelemetry-sdk|1.16.0|
|**aiohappyeyeballs**|**2.6.2 ⬆️ 2.7.1**|opentelemetry-semantic-conventions|0.37b0|
|aiohttp|3.14.1|packaging|24.2|
|aiosignal|1.4.0|pandas|2.3.3|
|alsa-lib|1.2.16.1|pandasql|0.7.3|
|amqp|5.3.1|pango|1.56.4|
|annotated-doc|0.0.4|parso|0.8.7|
|annotated-types|0.7.0|pathspec|1.1.1|
|**anyio**|**4.14.1 ⬆️ 4.14.2**|patsy|1.0.2|
|asttokens|3.0.1|pcre2|10.47|
|at-spi2-atk|2.38.0|pexpect|4.9.0|
|at-spi2-core|2.40.3|**pillow**|**12.2.0 ⬆️ 12.3.0**|
|atk-1.0|2.38.0|pip|26.1.2|
|attrs|26.1.0|pixman|0.46.4|
|azure-core|1.39.0|platformdirs|4.10.0|
|azure-storage-blob|12.30.0|plotly|6.7.0|
|azure-storage-file-datalake|12.25.0|portalocker|3.2.0|
|backports.zstd|1.6.0|prompt-toolkit|3.0.52|
|billiard|4.2.4|prompt_toolkit|3.0.52|
|**boto3**|**1.43.36 ⬆️ 1.43.45**|propcache|0.5.2|
|**botocore**|**1.43.36 ⬆️ 1.43.45**|protobuf|5.29.6|
|brotli|1.2.0|psutil|7.2.2|
|brotli-bin|1.2.0|pthread-stubs|0.4|
|brotli-python|1.2.0|ptyprocess|0.7.0|
|bzip2|1.0.8|pure_eval|0.2.3|
|ca-certificates|2026.6.17|py-xgboost|2.1.4|
|cachetools|5.5.2|**pyasn1**|**0.6.3 ⬆️ 0.6.4**|
|cairo|1.18.4|pyasn1-modules|0.4.2|
|celery|5.5.3|pycparser|3.0|
|certifi|2026.6.17|pydantic|2.13.4|
|**cffi**|**2.0.0 ⬆️ 2.1.0**|pydantic-core|2.46.4|
|**charset-normalizer**|**3.4.7 ⬆️ 3.4.9**|pydantic-extra-types|2.11.1|
|**click**|**8.4.1 ⬆️ 8.4.2**|pydantic-settings|2.14.2|
|click-didyoumean|0.3.1|pygments|2.20.0|
|click-plugins|1.1.1.2|pyodbc|5.3.0|
|click-repl|0.3.0|pyparsing|3.3.2|
|cloudpickle|3.1.2|pyside6|6.11.1|
|colorama|0.4.6|pysocks|1.7.1|
|comm|0.2.3|python|3.13.11|
|contourpy|1.3.3|python-dateutil|2.9.0.post0|
|cpython|3.13.14|**python-discovery**|**1.4.2 ⬆️ 1.4.4**|
|cryptography|49.0.0|python-dotenv|1.2.2|
|cycler|0.12.1|python-gil|3.13.14|
|cyrus-sasl|2.1.28|python-graphviz|0.20.3|
|**databricks-sdk**|**0.119.0 ⬆️ 0.120.0**|**python-librt**|**0.11.0 ⬆️ 0.13.0**|
|dbus|1.16.2|python-multipart|0.0.32|
|debugpy|1.8.21|**python-tzdata**|**2026.2 ⬆️ 2026.3**|
|decorator|5.3.1|python_abi|3.13|
|defusedxml|0.7.1|pytz|2026.2|
|deprecated|1.3.1|pyu2f|0.1.5|
|distlib|0.4.3|pyyaml|6.0.3|
|dnspython|2.8.0|pyzmq|27.1.0|
|double-conversion|3.4.0|qhull|2020.2|
|email-validator|2.3.0|qt6-main|6.11.1|
|email_validator|2.3.0|readline|8.3|
|epoxy|1.5.10|regex|2026.5.9|
|et_xmlfile|2.0.0|requests|2.34.2|
|exceptiongroup|1.3.1|rich|15.0.0|
|executing|2.2.1|rich-toolkit|0.20.1|
|**fastapi**|**0.138.1 ⬆️ 0.139.0**|rsa|4.9.1|
|**fastapi-cli**|**0.0.27 ⬆️ 0.0.29**|ruamel.yaml|0.19.1|
|**fastapi-core**|**0.138.1 ⬆️ 0.139.0**|ruamel.yaml.clib|0.2.15|
|fastar|0.11.0|**s3transfer**|**0.19.0 ⬆️ 0.19.1**|
|**filelock**|**3.29.4 ⬆️ 3.29.7**|scikit-learn|1.6.1|
|flask|2.2.5|scipy|1.18.0|
|font-ttf-dejavu-sans-mono|2.37|seaborn|0.13.2|
|font-ttf-inconsolata|3.000|seaborn-base|0.13.2|
|font-ttf-source-code-pro|2.038|**setuptools**|**82.0.1 ⬆️ 83.0.0**|
|font-ttf-ubuntu|0.83|shellingham|1.5.4|
|fontconfig|2.18.1|six|1.17.0|
|fonts-conda-ecosystem|1|smmap|5.0.3|
|fonts-conda-forge|1|sniffio|1.3.1|
|fonttools|4.63.0|sqlalchemy|2.0.51|
|freetype|2.14.3|sqlparse|0.5.5|
|fribidi|1.0.16|stack_data|0.6.3|
|frozenlist|1.8.0|starlette|1.3.1|
|fsspec_wrapper|0.1.15|statsmodels|0.14.6|
|gdk-pixbuf|2.44.7|threadpoolctl|3.6.0|
|gitdb|4.0.12|tk|8.6.13|
|**gitpython**|**3.1.50 ⬆️ 3.1.51**|tomli|2.4.1|
|glib-tools|2.88.2|tornado|6.5.7|
|**google-auth**|**2.55.1 ⬆️ 2.55.2**|tqdm|4.68.3|
|graphite2|1.3.15|traitlets|5.15.1|
|graphviz|14.1.2|typer|0.26.8|
|greenlet|3.5.3|**typing-extensions**|**4.15.0 ⬆️ 4.16.0**|
|gtk3|3.24.52|typing-inspection|0.4.2|
|gts|0.7.6|**typing_extensions**|**4.15.0 ⬆️ 4.16.0**|
|h11|0.16.0|tzdata|2025c|
|h2|4.3.0|unixodbc|2.3.14|
|harfbuzz|14.2.1|urllib3|2.7.0|
|hicolor-icon-theme|0.17|**uvicorn**|**0.49.0 ⬆️ 0.51.0**|
|hpack|4.2.0|**uvicorn-standard**|**0.49.0 ⬆️ 0.51.0**|
|httpcore|1.0.9|uvloop|0.22.1|
|httptools|0.8.0|vine|5.1.0|
|httpx|0.28.1|virtualenv|21.5.0|
|hyperframe|6.1.0|watchfiles|1.2.0|
|icu|78.3|wayland|1.25.0|
|idna|3.18|**wcwidth**|**0.8.1 ⬆️ 0.8.2**|
|importlib-metadata|8.8.0|**websockets**|**16.0 ⬆️ 16.1**|
|ipykernel|7.3.0|werkzeug|3.1.8|
|ipython|9.14.0|widgetsnbextension|4.0.15|
|ipython_pygments_lexers|1.1.1|wrapt|2.2.2|
|ipywidgets|8.1.7|xcb-util|0.4.1|
|isodate|0.7.2|xcb-util-cursor|0.1.6|
|itsdangerous|2.2.0|xcb-util-image|0.4.0|
|jedi|0.20.0|xcb-util-keysyms|0.4.1|
|jinja2|3.1.6|xcb-util-renderutil|0.3.10|
|jmespath|1.1.0|xcb-util-wm|0.4.2|
|jupyter_client|8.9.1|xgboost|2.1.4|
|jupyter_core|5.9.1|xkeyboard-config|2.48|
|jupyterlab_widgets|3.0.16|xlrd|2.0.2|
|keyutils|1.6.3|xorg-libice|1.1.2|
|kiwisolver|1.5.0|xorg-libsm|1.2.6|
|kombu|5.5.4|xorg-libx11|1.8.13|
|krb5|1.22.2|xorg-libxau|1.0.12|
|lcms2|2.19.1|xorg-libxcomposite|0.4.7|
|ld_impl_linux-64|2.45.1|xorg-libxcursor|1.2.3|
|lerc|4.1.0|xorg-libxdamage|1.1.6|
|libabseil|20250127.1|xorg-libxdmcp|1.1.5|
|libblas|3.11.0|xorg-libxext|1.3.7|
|libboost|1.90.0|xorg-libxfixes|6.0.2|
|libbrotlicommon|1.2.0|xorg-libxi|1.8.3|
|libbrotlidec|1.2.0|xorg-libxinerama|1.1.6|
|libbrotlienc|1.2.0|xorg-libxrandr|1.5.5|
|libcblas|3.11.0|xorg-libxrender|0.9.12|
|libclang-cpp22.1|22.1.8|xorg-libxtst|1.2.5|
|libclang13|22.1.8|xorg-libxxf86vm|1.1.7|
|libcups|2.3.3|xorg-xorgproto|2025.1|
|libdeflate|1.25|yaml|0.2.5|
|libdrm|2.4.127|yarl|1.24.2|
|libedit|3.1.20250104|zeromq|4.3.5|
|libegl|1.7.0|zipp|4.1.0|
|libegl-devel|1.7.0|zlib-ng|2.3.3|
|libexpat|2.8.1|zstd|1.5.7|
|libffi|3.5.2|**absl-py**|**2.4.0 ⬆️ 2.5.0**|
|libfreetype|2.14.3|adlfs|2025.8.0|
|libfreetype6|2.14.3|alembic|1.18.5|
|libgcc|15.2.0|azure-datalake-store|0.0.53|
|libgcc-ng|15.2.0|azure-identity|1.25.3|
|libgd|2.3.3|azure-keyvault-secrets|4.11.0|
|libgfortran|15.2.0|azureml-synapse|0.0.1|
|libgfortran5|15.2.0|catboost|1.2.10|
|libgl|1.7.0|clr-loader|0.3.1|
|libgl-devel|1.7.0|cmdstanpy|1.3.0|
|libglib|2.88.2|colorlog|6.10.1|
|libglvnd|1.7.0|convertdate|2.4.1|
|libglx|1.7.0|fabric-analytics-notebook-plugin|0.0.3.post8|
|libglx-devel|1.7.0|fabric-analytics-sdk|0.0.3.post8|
|libgomp|15.2.0|fastjsonschema|2.21.2|
|**libharfbuzz**|**14.2.1**|flaml|2.5.0.post6|
|**libharfbuzz-devel**|**14.2.1**|**flt-python**|**1.6.1 ⬆️ 1.7.1**|
|libiconv|1.18|fluent-logger|0.10.0|
|**libjpeg-turbo**|**3.1.4.1 ⬆️ 3.2.0**|fsspec|2026.6.0|
|liblapack|3.11.0|geoanalytics-fabric|2.0.0|
|liblightgbm|4.6.0|gson|0.0.4|
|libllvm22|22.1.8|hcrystalball|0.1.10|
|liblzma|5.8.3|**holidays**|**0.99 ⬆️ 0.100**|
|libmpdec|4.0.0|importlib-resources|7.1.0|
|libntlm|1.8|**impulse-python-handler**|**1.5.223168344 ⬆️ 1.5.226604159**|
|libopenblas|0.3.33|joblib|1.4.2|
|libopengl|1.7.0|joblibspark|0.6.0|
|libpciaccess|0.19|jsonschema|4.26.0|
|libpng|1.6.58|jsonschema-specifications|2025.9.1|
|libpq|18.4|jupyter-ui-poll|1.1.0|
|librsvg|2.62.3|kqlmagiccustom|0.1.115+fabric.post26|
|libsodium|1.0.22|library-metadata-cooker|3.7.0.0|
|libsqlite|3.53.3|**lunardate**|**0.2.2 ⬆️ 0.3.0**|
|libstdcxx|15.2.0|mako|1.3.12|
|libstdcxx-ng|15.2.0|msal|1.37.0|
|**libtiff**|**4.7.1 ⬆️ 4.7.2**|msal-extensions|1.3.1|
|libuuid|2.42.2|msgpack|1.2.1|
|libuv|1.52.1|nbformat|5.10.4|
|libvulkan-loader|1.4.341.0|**nltk**|**3.9.4 ⬆️ 3.10.0**|
|libwebp-base|1.6.0|notebookutils|1.1.15.41.20260524.4|
|libxcb|1.17.0|optuna|3.6.1|
|libxcrypt|4.4.36|pandasnet|1.0|
|libxgboost|2.1.4|powerbiclient|3.1.1|
|libxkbcommon|1.13.2|prophet|1.3.0|
|libxml2|2.15.3|prose-pandas2pyspark|10.16.0|
|libxml2-16|2.15.3|prose-suggestions|10.16.0|
|libxslt|1.1.43|py4j|0.10.9.9|
|libzlib|1.3.2|pyarrow|24.0.0|
|lightgbm|4.6.0|**pydeequ**|**1.0.0+msft.1 ⬆️ 1.5.0+msft.1**|
|markdown-it-py|4.2.0|pyjwt|2.13.0|
|markupsafe|3.0.3|pyluach|2.3.0|
|matplotlib|3.10.9|pymeeus|0.5.12|
|matplotlib-base|3.10.9|pyspark|4.1.1.5.5.20260428.5|
|matplotlib-inline|0.2.2|pythonnet|3.1.0|
|mdurl|0.1.2|referencing|0.37.0|
|mlflow-skinny|2.22.0|rgf-python|3.12.0|
|multidict|6.7.1|rouge-score|0.1.2|
|munkres|1.1.4|**rpds-py**|**2026.5.1 ⬆️ 2026.6.3**|
|mypy|1.20.2|semantic-link-sempy|0.14.1|
|mypy_extensions|1.1.0|spark-mssql-connector-fabric41|1.1.0.217307560|
|**narwhals**|**2.22.1 ⬆️ 2.23.0**|sqlanalyticsfabricconnectorpy|1.0.1|
|ncurses|6.6|stanio|0.5.1|
|nest-asyncio2|1.7.2|synapseml|1.1.3+spark4.1|
|numpy|2.4.1|synapseml-internal|1.1.3.0+spark4.1|
|ocl-icd|2.3.4|synapseml-mlflow|2.0.4|
|opencl-headers|2025.06.13|synapseml-utils|1.1.14|
|openjpeg|2.5.4|tenacity|9.1.4|
|openldap|2.6.13|workalendar|17.0.0|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|jta|1.1|
|JLargeArrays|1.5|jts-core|1.20.0|
|JTransforms|3.1|jul-to-slf4j|2.0.17|
|RoaringBitmap|1.3.0|juniversalchardet|2.4.0|
|ST4|4.0.4|**kafka-clients**|**3.9.1 ⬆️ 3.9.2**|
|TokenLibrary-assembly|5.0.0-dev.189919691|kryo-shaded|4.0.3|
|VegasConnector|4.1.0|lapack|3.0.4|
|**aircompressor**|**2.0.2 ⬆️ 2.0.3**|lenses|2.13-0.11.15|
|algebra|2.13-2.8.0|leveldbjni-all|1.8|
|aliyun-java-sdk-core|4.5.10|libfb303|0.9.3|
|aliyun-java-sdk-kms|2.11.0|libthrift|0.16.0|
|aliyun-java-sdk-ram|3.1.0|log4j|1.2-api-2.24.3|
|aliyun-sdk-oss|3.13.2|log4j-api|2.24.3|
|ammonite|2.13.17-3.0.3|log4j-core|2.24.3|
|ammonite-compiler|2.13.17_2.13.17-3.0.3|log4j-layout-template-json|2.24.3|
|ammonite-compiler-interface|2.13.17_2.13.17-3.0.3|log4j-slf4j2-impl|2.24.3|
|ammonite-interp|2.13.17_2.13.17-3.0.3|**lz4-java**|**1.8.0 ⬆️ 1.8.1**|
|ammonite-interp-api|2.13.17_2.13.17-3.0.3|mainargs|2.13-0.7.6|
|ammonite-repl|2.13.17_2.13.17-3.0.3|metrics-core|4.2.37|
|ammonite-repl-api|2.13.17_2.13.17-3.0.3|metrics-graphite|4.2.37|
|ammonite-runtime|2.13.17_2.13.17-3.0.3|metrics-healthchecks|4.2.9|
|ammonite-terminal|2.13.17_2.13-3.0.3|metrics-jakarta-servlet|4.2.19|
|ammonite-util|2.13.17_2.13-3.0.3|metrics-jakarta-servlets|4.2.19|
|analyticsaccelerator-s3|1.3.0|metrics-jmx|4.2.37|
|antlr-runtime|3.5.2|metrics-json|4.2.37|
|antlr4-runtime|4.13.1|metrics-jvm|4.2.37|
|aopalliance-repackaged|3.0.6|metrics4-scala|2.13-4.2.9|
|arpack|3.0.4|minlog|1.3.0|
|arpack_combined_all|0.1|**netty-all**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|arrow-compression|18.3.0|**netty-buffer**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|arrow-format|18.3.0|**netty-codec**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|arrow-memory-core|18.3.0|**netty-codec-base**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|arrow-memory-netty|18.3.0|**netty-codec-classes-quic**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|arrow-memory-netty-buffer-patch|18.3.0|**netty-codec-compression**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|arrow-vector|18.3.0|**netty-codec-dns**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|audience-annotations|0.12.0|**netty-codec-http**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|avro|1.12.1|**netty-codec-http2**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|avro-ipc|1.12.1|**netty-codec-http3**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|avro-mapred|1.12.1|**netty-codec-marshalling**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|azure-data-lake-store-sdk|2.3.9|**netty-codec-native-quic**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-aarch_64**|
|azure-keyvault-core|1.0.0|**netty-codec-native-quic**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-x86_64**|
|azure-storage|7.0.1|**netty-codec-native-quic**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-osx-aarch_64**|
|blas|3.0.4|**netty-codec-native-quic**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-osx-x86_64**|
|breeze|2.13-2.1.0|**netty-codec-native-quic**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-windows-x86_64**|
|breeze-macros|2.13-2.1.0|**netty-codec-protobuf**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|bsp4j|2.1.1|**netty-codec-socks**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|bundle|2.29.52|**netty-common**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|cats-kernel|2.13-2.8.0|**netty-handler**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|chill|2.13-0.10.0|**netty-handler-proxy**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|chill-java|0.10.0|**netty-resolver**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|class-path-util|2.13-0.1.4|**netty-resolver-dns**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|common|2.13-4.13.10|netty-tcnative-boringssl-static|2.0.74.Final-linux-aarch_64|
|commons-cli|1.10.0|netty-tcnative-boringssl-static|2.0.74.Final-linux-x86_64|
|commons-codec|1.19.0|netty-tcnative-boringssl-static|2.0.74.Final-osx-aarch_64|
|commons-collections4|4.5.0|netty-tcnative-boringssl-static|2.0.74.Final-osx-x86_64|
|commons-compiler|3.1.9|netty-tcnative-boringssl-static|2.0.74.Final-windows-x86_64|
|commons-compress|1.28.0|netty-tcnative-classes|2.0.74.Final|
|commons-crypto|1.1.0|**netty-transport**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|commons-dbcp|1.4|**netty-transport-classes-epoll**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|commons-io|2.21.0|**netty-transport-classes-io_uring**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|commons-lang|2.6|**netty-transport-classes-kqueue**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|commons-lang3|3.19.0|**netty-transport-native-epoll**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-aarch_64**|
|commons-math3|3.6.1|**netty-transport-native-epoll**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-riscv64**|
|commons-pool|1.5.4|**netty-transport-native-epoll**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-x86_64**|
|commons-pool2|2.12.1|**netty-transport-native-io_uring**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-aarch_64**|
|commons-text|1.14.0|**netty-transport-native-io_uring**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-riscv64**|
|compress-lzf|1.1.2|**netty-transport-native-io_uring**|**4.2.7.Final-linux-aarch_64 ⬆️ 4.2.15.Final-linux-x86_64**|
|curator-client|5.9.0|**netty-transport-native-kqueue**|**4.2.7.Final-osx-aarch_64 ⬆️ 4.2.15.Final-osx-aarch_64**|
|curator-framework|5.9.0|**netty-transport-native-kqueue**|**4.2.7.Final-osx-aarch_64 ⬆️ 4.2.15.Final-osx-x86_64**|
|curator-recipes|5.9.0|**netty-transport-native-unix-common**|**4.2.7.Final ⬆️ 4.2.15.Final**|
|datanucleus-api-jdo|4.2.4|nimbus-jose-jwt|9.37.2|
|datanucleus-core|4.1.17|objenesis|3.4|
|datanucleus-rdbms|4.1.19|okhttp|3.12.12|
|datasketches-java|6.2.0|okio|1.17.6|
|datasketches-memory|3.0.2|opencsv|2.3|
|dependency|2.13-0.3.2|opentracing-api|0.33.0|
|dependency-interface|2.13-0.3.2|opentracing-noop|0.33.0|
|derby|10.16.1.1|opentracing-util|0.33.0|
|derbyshared|10.16.1.1|orc-core|2.2.1-shaded-protobuf|
|derbytools|10.16.1.1|orc-format|1.1.1-shaded-protobuf|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|orc-mapreduce|2.2.1-shaded-protobuf|
|esdk-obs-java|3.20.4.2|orc-shims|2.2.1|
|failureaccess|1.0.3|org.eclipse.lsp4j.generator|0.20.1|
|fansi|2.13-0.5.1|org.eclipse.lsp4j.jsonrpc|0.20.1|
|fastparse|2.13-3.1.1|org.eclipse.xtend.lib|2.28.0|
|flatbuffers-java|25.2.10|org.eclipse.xtend.lib.macro|2.28.0|
|**flt-spark-sql-extensions**|**1.6.1 ⬆️ 1.7.1**|org.eclipse.xtext.xbase.lib|2.28.0|
|**fmlv-utils**|**1.6.1 ⬆️ 1.7.1**|oro|2.0.8|
|gcs-connector-hadoop3|2.2.28-shaded|os-lib|2.13-0.11.5|
|geny|2.13-1.1.1|os-zip|0.11.5|
|gson|2.8.9|osgi-resource-locator|1.0.3|
|guava|33.4.8-jre|paranamer|2.8.3|
|**hadoop-aliyun**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parquet-column|1.16.0|
|**hadoop-annotations**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parquet-common|1.16.0|
|**hadoop-aws**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parquet-encoding|1.16.0|
|**hadoop-azure**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parquet-format-structures|1.16.0|
|**hadoop-azure-datalake**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parquet-hadoop|1.16.0|
|**hadoop-client-api**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|**parquet-hadoop-ms**|**4.1.1.5.5.20260618.5 ⬆️ 4.1.1.5.5.20260717.1**|
|**hadoop-client-runtime**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parquet-jackson|1.16.0|
|**hadoop-cloud-storage**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|parsers|2.13-4.13.10|
|**hadoop-huaweicloud**|**3.4.2.5.5.20260618.5 ⬆️ 3.4.2.5.5.20260717.1**|pickle|1.5|
|hadoop-shaded-guava|1.4.0|pprint|2.13-0.9.0|
|hive-common|2.3.10|profiler|1.1.1|
|hive-exec|2.3.10-core|py4j|0.10.9.9|
|hive-metastore|2.3.10|requests|2.13-0.9.0|
|hive-serde|2.3.10|rocksdbjni|9.8.4|
|hive-shims|0.23-2.3.10|scala-collection-compat|2.13-2.11.0|
|hive-shims|2.3.10|scala-compiler|2.13.17|
|hive-shims-common|2.3.10|scala-library|2.13.17|
|hive-shims-scheduler|2.3.10|scala-parallel-collections|2.13-1.2.0|
|hive-storage-api|2.8.1|scala-parser-combinators|2.13-2.4.0|
|hk2-api|3.0.6|scala-reflect|2.13.17|
|hk2-locator|3.0.6|scala-xml|2.13-2.4.0|
|hk2-utils|3.0.6|scalameta|2.13-4.13.10|
|httpclient|4.5.14|scalaparse|2.13-3.1.1|
|httpcore|4.4.16|scalapb-runtime|2.13-0.11.15|
|httpmime|4.5.14|scalatra-common-jakarta|2.13-3.0.0|
|iceberg-spark-runtime|4.1_2.13-1.11.0|scalatra-jakarta|2.13-3.0.0|
|icu4j|77.1|scalatra-metrics-jakarta|2.13-3.0.0|
|impulse-core_spark|2.13-1.5.214702911|semanticdb-shared|2.13-4.13.10|
|impulse-exception_java17|2.13-1.5.214702911|slf4j-api|2.0.17|
|impulse-telemetry-common|2.13-1.5.214702911|snappy-java|1.1.10.8|
|impulse-telemetry-mds_spark|2.13-1.5.214702911|sourcecode|2.13-0.4.4|
|impulse-telemetry-pulse_spark|2.13-1.5.214702911|**spark-arsenal**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|ini4j|0.5.4|**spark-avro**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|interface|1.0.28|**spark-catalyst**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|io|2.13-4.13.10|**spark-common-utils**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|istack-commons-runtime|4.1.2|**spark-common-utils-java**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|ivy|2.5.1|**spark-connect**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jackson-annotations|2.20|**spark-core**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jackson-core|2.20.0|**spark-enhancement**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jackson-databind|2.20.0|**spark-graphx**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jackson-dataformat-cbor|2.20.0|**spark-hadoop-cloud**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jackson-datatype-jsr310|2.20.0|**spark-hive**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jackson-module-scala|2.13-2.20.0|**spark-kvstore**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.activation-api|2.1.3|**spark-launcher**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.annotation-api|2.1.1|**spark-microsoft-tools**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.inject-api|2.0.1|**spark-mllib**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.servlet-api|5.0.0|**spark-mllib-local**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.validation-api|3.0.2|**spark-network-common**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.ws.rs-api|3.0.0|**spark-network-shuffle**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jakarta.xml.bind-api|4.0.2|**spark-onesecurity-client**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|janino|3.1.9|**spark-onesecurity-common**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|java-diff-utils|4.16|**spark-onesecurity-server**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|java-xmlbuilder|1.2|**spark-pipelines**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javaparser-core|3.2.12|**spark-repl**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javassist|3.30.2-GA|**spark-sketch**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javatuples|1.2|**spark-sql**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javax.annotation-api|1.3.2|**spark-sql-api**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javax.jdo|3.2.0-m3|**spark-sql-kafka**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javax.servlet-api|4.0.1|**spark-streaming**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|javolution|5.5.1|**spark-streaming-kafka**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jaxb-core|4.0.5|**spark-tags**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jaxb-runtime|4.0.5|**spark-token-provider-kafka**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jcip-annotations|1.0-1|**spark-unsafe**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jcl-over-slf4j|2.0.17|**spark-variant**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jdo-api|3.0.1|**spark-yarn**|**2.13-4.1.1.5.5.20260618.5 ⬆️ 2.13-4.1.1.5.5.20260717.1**|
|jdom2|2.0.6|spire|2.13-0.18.0|
|jersey-client|3.0.18|spire-macros|2.13-0.18.0|
|jersey-common|3.0.18|spire-platform|2.13-0.18.0|
|jersey-container-servlet|3.0.18|spire-util|2.13-0.18.0|
|jersey-container-servlet-core|3.0.18|stax-api|1.0.1|
|jersey-hk2|3.0.18|stream|2.9.8|
|jersey-server|3.0.18|threeten-extra|1.8.0|
|jettison|1.5.4|tink|1.16.0|
|jetty-util|11.0.26|transaction-api|1.1|
|jetty-util-ajax|11.0.26|trees|2.13-4.13.10|
|jjwt-api|0.12.6|**trident-core**|**1.3.4 ⬆️ 1.4.4**|
|jjwt-impl|0.12.6|tridenttokenlibrary-assembly|2.5.1|
|jjwt-jackson|0.12.6|typename|2.13-1.1.0|
|jline|2.14.6|ujson|2.13-4.3.2|
|jline|3.29.0-jdk8|univocity-parsers|2.9.1|
|joda-time|2.14.0|upack|2.13-4.3.2|
|jodd-core|3.5.2|upickle|2.13-4.3.2|
|json|1.8|upickle-core|2.13-4.3.2|
|json|20231013|upickle-implicits|2.13-4.3.2|
|json-simple|1.1|wildfly-openssl|2.2.5.Final|
|json4s-ast|2.13-4.0.7|xbean-asm9-shaded|4.28|
|json4s-core|2.13-4.0.7|xmlschema-core|2.3.1|
|json4s-jackson|2.13-4.0.7|xz|1.10|
|json4s-jackson-core|2.13-4.0.7|**zookeeper**|**3.8.4.5.5.20260618.5 ⬆️ 3.8.4.5.5.20260717.1**|
|json4s-scalap|2.13-4.0.7|**zookeeper-jute**|**3.8.4.5.5.20260618.5 ⬆️ 3.8.4.5.5.20260717.1**|
|jsr305|3.0.0|zstd-jni|1.5.7-6|

# R Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|DALEX|2.5.3|lhs|1.2.1|
|DBI|1.3.0|lifecycle|1.0.5|
|DiceDesign|1.10|lightgbm|4.6.0|
|FabricTelemetry|1.0.2|listenv|0.10.1|
|GPfit|1.0-9|litedown|0.9|
|KernSmooth|2.23-26|lobstr|1.2.1|
|MASS|7.3-65|lubridate|1.9.5|
|Matrix|1.7-5|magrittr|2.0.5|
|ModelMetrics|1.2.2.2|maps|3.4.3|
|R.methodsS3|1.8.2|markdown|2.0|
|R.oo|1.27.1|memoise|2.0.1|
|R.utils|2.13.0|methods|4.5.2|
|R6|2.6.1|mime|0.13|
|R6P|0.4.0|miniUI|0.1.2|
|RColorBrewer|1.1-3|modeldata|1.5.1|
|RODBC|1.3-26.1|modelenv|0.2.0|
|Rcpp|1.1.1|modelr|0.1.11|
|S7|0.2.1|munsell|0.5.1|
|SQUAREM|2026.1|nlme|3.1-169|
|TTR|0.24.4|nnet|7.3-20|
|V8|8.0.1|notebookutils|1.1.15.41.20260524.4|
|XML|3.99-0.22|numDeriv|2016.8-1.1|
|arrow|22.0.0|openssl|2.3.5|
|askpass|1.2.1|otel|0.2.0|
|assertthat|0.2.1|pROC|1.19.0.1|
|backports|1.5.1|parallel|4.5.2|
|base|4.5.2|parallelly|1.46.1|
|base64enc|0.1-6|parsnip|1.5.0|
|bigD|0.3.1|patchwork|1.3.2|
|bit|4.6.0|pillar|1.11.1|
|bit64|4.6.0-1|pkgbuild|1.4.8|
|bitops|1.0-9|pkgconfig|2.0.3|
|blob|1.3.0|pkgdown|2.2.0|
|brew|1.0-10|pkgload|1.5.1|
|brio|1.1.5|plotly|4.11.0|
|broom|1.0.12|plyr|1.8.9|
|bslib|0.10.0|praise|1.0.0|
|cachem|1.1.0|prettyunits|1.2.0|
|callr|3.7.6|processx|3.8.7|
|cards|0.7.1|prodlim|2026.03.11|
|cardx|0.3.2|profvis|0.4.0|
|caret|7.0-1|progress|1.2.3|
|cellranger|1.1.0|progressr|0.19.0|
|class|7.3-23|promises|1.5.0|
|cli|3.6.6|proxy|0.4-29|
|clipr|0.8.0|pryr|0.1.6|
|clock|0.7.4|ps|1.9.2|
|codetools|0.2-20|purrr|1.2.1|
|collections|0.3.12|quantmod|0.4.28|
|colorspace|2.1-2|ragg|1.5.2|
|commonmark|2.0.0|rappdirs|0.3.4|
|compiler|4.5.2|rbokeh|0.5.2|
|config|0.3.2|rcmdcheck|1.4.0|
|conflicted|1.2.0|reactR|0.6.1|
|coro|1.1.0|reactable|0.4.5|
|cpp11|0.5.4|readr|2.2.0|
|crayon|1.5.3|readxl|1.4.5|
|credentials|2.0.3|recipes|1.3.2|
|crosstalk|1.2.2|rematch|2.0.0|
|crul|1.6.0|rematch2|2.1.2|
|curl|7.0.0|remotes|2.5.0|
|data.table|1.17.8|reprex|2.1.1|
|datasets|4.5.2|reshape2|1.4.5|
|dbplyr|2.5.1|rjson|0.2.23|
|desc|1.4.3|rlang|1.2.0|
|devtools|2.4.6|rlist|0.4.6.2|
|diagram|1.6.5|rmarkdown|2.30|
|dials|1.4.2|roxygen2|7.3.3|
|diffobj|0.3.6|rpart|4.1.27|
|digest|0.6.39|rprojroot|2.1.1|
|doFuture|1.2.1|rsample|1.3.2|
|downlit|0.4.5|rstudioapi|0.18.0|
|dplyr|1.2.1|rversions|3.0.0|
|dtplyr|1.3.3|rvest|1.0.5|
|e1071|1.7-17|safetensors|0.2.0|
|ellipsis|0.3.3|sass|0.4.10|
|evaluate|1.0.5|scales|1.4.0|
|fansi|1.0.7|selectr|0.5-1|
|farver|2.1.2|sessioninfo|1.2.3|
|fastmap|1.2.0|sfd|0.1.0|
|fontawesome|0.5.3|shape|1.4.6.1|
|forcats|1.0.1|shiny|1.13.0|
|foreach|1.5.2|slider|0.3.3|
|fs|1.6.7|sourcetools|0.1.7-2|
|furrr|0.4.0|sparklyr|1.9.2|
|future|1.70.0|sparsevctrs|0.3.6|
|future.apply|1.20.2|splines|4.5.2|
|gargle|1.6.1|stats|4.5.2|
|generics|0.1.4|stats4|4.5.2|
|gert|2.3.1|stringi|1.8.7|
|ggplot2|4.0.2|stringr|1.6.0|
|gh|1.5.0|survival|3.8-6|
|gistr|0.9.0|sys|3.4.3|
|gitcreds|0.1.2|systemfonts|1.3.2|
|globals|0.19.1|tailor|0.1.0|
|glue|1.8.0|tcltk|4.5.2|
|googledrive|2.1.2|testthat|3.3.2|
|googlesheets4|1.1.2|textshaping|1.0.5|
|gower|1.0.2|tibble|3.3.1|
|grDevices|4.5.2|tidymodels|1.4.1|
|graphics|4.5.2|tidyr|1.3.2|
|grid|4.5.2|tidyselect|1.2.1|
|gridExtra|2.3|tidyverse|2.0.0|
|gt|1.3.0|timeDate|4052.112|
|gtable|0.3.6|timechange|0.4.0|
|gtsummary|2.5.0|tinytex|0.59|
|hardhat|1.4.3|tools|4.5.2|
|haven|2.5.5|torch|0.16.0|
|hexbin|1.28.5|triebeard|0.4.1|
|highcharter|0.9.4|tune|2.0.1|
|highr|0.12|tzdb|0.5.0|
|hms|1.1.4|urlchecker|1.0.1|
|htmltools|0.5.9|urltools|1.7.3.1|
|htmlwidgets|1.6.4|usethis|3.2.1|
|httpcode|0.3.0|utf8|1.2.6|
|httpuv|1.6.17|utils|4.5.2|
|httr|1.4.8|uuid|1.2-2|
|httr2|1.2.2|vctrs|0.7.2|
|iBreakDown|2.1.2|viridisLite|0.4.3|
|ids|1.0.1|vroom|1.7.1|
|igraph|2.1.4|waldo|0.6.2|
|infer|1.1.0|warp|0.2.3|
|ingredients|2.3.0|whisker|0.4.1|
|ini|0.3.1|withr|3.0.2|
|ipred|0.9-15|workflows|1.3.0|
|isoband|0.3.0|workflowsets|1.1.1|
|iterators|1.0.14|xfun|0.57|
|jquerylib|0.1.4|xgboost|3.1.1.1|
|jsonlite|2.0.0|xml2|1.5.2|
|juicyjuice|0.1.0|xopen|1.0.1|
|kernelshap|0.9.1|xtable|1.8-8|
|knitr|1.51|xts|0.14.2|
|labeling|0.4.3|yaml|2.3.12|
|later|1.4.8|yardstick|1.4.0|
|lattice|0.22-9|zip|2.3.3|
|lava|1.9.0|zoo|1.8-15|
|lazyeval|0.2.3|

