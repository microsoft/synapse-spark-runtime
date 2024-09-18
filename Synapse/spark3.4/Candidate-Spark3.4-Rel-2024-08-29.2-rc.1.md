# System Environment
*   **Product**: Synapse Spark 3.4
*   **Vhd Release**: Spark3.4-Rel-2024-08-29.2-rc.1
*   **Operating System**: CBL-Mariner 2.0.20240829
*   **Apache Spark**: 3.4.3
*   **Java**: 11.0.24
*   **Scala**: 2.12.17
*   **Python**: 3.10/2.0.0
*   **Delta Lake**: 2.4.0.19

# New Features
|Id|Component|Description|
|-----|-----|-----|
|1440463|TridentCore:1.2.15, LakeMetastore:0.1.13|Add support for using Spark SQL on Mirror Databases in read-only mode, add support for using Spark SQL without requiring an attached lakehouse (must use full namespace of the form `<workspace>.<artifact>.<schema>.<table>`, fixes bug in resolving `global_temp` using onelake spark catalog, and improves user facing error reporting and logging for easier debugging|
|1420479|TokenLibrary:4.3.0, ServiceConfigurationTemplates:core-site.xml.liquid|Enabling Reading and Writing Internal Log Files to SystemStorage account with shorter lived tokens|
|1429897|Wildfire/spark34:1.9.13|Schema: resolve namespaces before setting them. CVE fixes in livy, make repl count user configurable.|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1440216|ServiceConfigurationTemplates:spark/3.4.0|We onboard a new feature in Livy that can expose the debug jupyter messages from kernel. In Cluster Service runtime, we add a feature flag to control this feature by using Livy conf.|
|1441785|NotebookUtils:1.1.54|Set no-symlinks=true to Improve Blobfusev2 performance|
|1440463|TridentCore:1.2.15, LakeMetastore:0.1.13|Add support for using Spark SQL on Mirror Databases in read-only mode, add support for using Spark SQL without requiring an attached lakehouse (must use full namespace of the form `<workspace>.<artifact>.<schema>.<table>`, fixes bug in resolving `global_temp` using onelake spark catalog, and improves user facing error reporting and logging for easier debugging|
|1440495|Conda:8.0.20|Renaming internal components, fixing argument issues, enhancing experiment tracking, and upgrading flaml version to 2.3.0.post1|
|1441419|TokenLibrary:4.3.2|Thwart burst mode access to TokenService|
|1441581|TridentTokenLibrary:1.9.5|Retries for IO errors when invoking TokenProvider|
|1424499|ServiceConfigurationTemplates:spark3.4|Add the SystemStorageAccountName and SystemStorageType keys to internal liquid config files|
|1427724|Conda:8.0.18|Improve automl experiences for low code automl template and UI settings, improve AI Samples by fixing some settings, and upgrading flaml version to 2.2.0.post1|
|1432059|NotebookUtils:1.1.53|Upgrade NotebookUtils to 1.1.3:  Improve help api doc, enable feature flag for Data Wrangler display entry by default, fix runMultiple "Index 962 out of bounds for length 13" issue, and add notebookutils.notebook.getDefinition and improve notebookutils.notebook.updateDefinition|
|1434474|Conda:8.0.19, R:1.0.7|Upgraded R version to address CVE-2024-27322.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1451703|TokenLibrary:4.2.2|Reverting change to fix regression with Managed VNet session startup|
|1444519|TridentCore:1.2.16, Wildfire/spark34:1.9.15|Fixes bug for spark sql queries on file when onelake spark catalog is enabled with no attached lakehouses to the session, and fixes a leak in driver logs when custom configuration is provided|
|1429357|LibraryMetadataCooker:2.0.2|Previously the jar metadata cooker version is incorrect, causing error in Library Management job.|
|1439914|DWConnector:1.0.3|Upgrade Synapse DW Connector to 2.1.5. Fixes temp files clean up after read and filter pushdown by removing unsupported Escape keyword from the SQL clauses constructed by the connector.|
|1440463|TridentCore:1.2.15, LakeMetastore:0.1.13|Add support for using Spark SQL on Mirror Databases in read-only mode, add support for using Spark SQL without requiring an attached lakehouse (must use full namespace of the form `<workspace>.<artifact>.<schema>.<table>`, fixes bug in resolving `global_temp` using onelake spark catalog, and improves user facing error reporting and logging for easier debugging|
|1429897|Wildfire/spark34:1.9.13|Schema: resolve namespaces before setting them. CVE fixes in livy, make repl count user configurable.|
|1432059|NotebookUtils:1.1.53|Upgrade NotebookUtils to 1.1.3:  Improve help api doc, enable feature flag for Data Wrangler display entry by default, fix runMultiple "Index 962 out of bounds for length 13" issue, and add notebookutils.notebook.getDefinition and improve notebookutils.notebook.updateDefinition|
|1434474|Conda:8.0.19, R:1.0.7|Upgraded R version to address CVE-2024-27322.|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|AutoscaleProbe|3.9.2|**OnelakeSparkCatalog**|**0.1.10 ⬆️ 0.1.13**|
|Autotune|1.11.1.1|Peregrine|0.10.4|
|AzureMLExtensions|1.0.4|PostgreSQLJDBCDriver|1.0.3|
|CSparkMetricUpdate|1.0.5|Python|3.10/2.0.0|
|**Conda**|**8.0.17 ⬆️ 8.0.20**|**R**|**1.0.6 ⬆️ 1.0.7**|
|CosmosDBConnector|2.1.1|SQLServerODBCDriver|18.1.0|
|DSCopilotInstaller|1.0.0|SStreamOnSparkJar|2.3.5.1|
|**DWConnector**|**1.0.2 ⬆️ 1.0.3**|SparkAdvisor|1.0.2|
|Delta|2.4.0.19|SparkDiagnosticsLibrary|1.0.24|
|EventHubConnector|2.3.26|SparkLighter|2.0.9|
|FabricDWConnector|1.0.10|SparkNativeParquetWriter|0.15.4|
|FsspecWrapper|1.0.15|SparkRPCHistoryServer|1.1.1|
|Genesis|0.30.0|SparklyrConnector|1.0.1|
|**GlutenUI**|**1.0.0**|TokenLibrary|4.2.2|
|HiveMetaStoreClient|1.1.21|**TridentCore**|**1.2.9 ⬆️ 1.2.16**|
|Impulse|1.2.5|**TridentTokenLibrary**|**1.9.4 ⬆️ 1.9.5**|
|KustoConnector|1.5.1|Vegas|3.4.09.01|
|LibraryManager|1.0.14|**Wildfire**|**1.9.12 ⬆️ 1.9.15**|
|**LibraryMetadataCooker**|**2.0.1 ⬆️ 2.0.2**|
|MMLSpark|1.4.17|
|MachineLearningPredict|1.0.1|
|MlflowLibrary|2.6.0.1|
|MySQLJavaConnector|1.0.3|
|**NotebookUtils**|**1.1.52 ⬆️ 1.1.54**|
|OneLakeClientStarter|1.0.20|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_libgcc_mutex|0.1|libwebp-base|1.3.2|
|_openmp_mutex|4.5|libxcb|1.15|
|_py-xgboost-mutex|2.0|libxcrypt|4.4.36|
|absl-py|2.1.0|libxgboost|2.0.3|
|adal|1.2.7|libxkbcommon|1.6.0|
|adlfs|2023.10.0|libxml2|2.12.5|
|aiohttp|3.9.3|libxslt|1.1.39|
|aiosignal|1.3.1|libzlib|1.2.13|
|alsa-lib|1.2.11|libzlib|1.3.1|
|anyio|3.7.1|lightgbm|4.2.0|
|applicationinsights|0.11.10|llvm-openmp|17.0.6|
|argcomplete|3.2.3|llvmlite|0.42.0|
|argon2-cffi|23.1.0|lxml|5.1.0|
|argon2-cffi-bindings|21.2.0|lz4-c|1.9.4|
|arrow|1.3.0|markdown|3.5.1|
|asttokens|2.4.1|markupsafe|2.1.5|
|astunparse|1.6.3|marshmallow|3.21.1|
|async-timeout|4.0.3|matplotlib|3.8.2|
|attr|2.5.1|**matplotlib**|**3.8.2 ⬆️ 3.9.2**|
|attrs|23.2.0|matplotlib-base|3.8.2|
|aws-c-auth|0.7.11|matplotlib-inline|0.1.7|
|aws-c-cal|0.6.9|matplotlib-inline|0.1.6|
|aws-c-common|0.9.12|mistune|3.0.2|
|aws-c-compression|0.2.17|mkl|2023.2.0|
|aws-c-event-stream|0.4.1|mkl-service|2.4.1|
|aws-c-http|0.8.0|mkl_fft|1.3.8|
|aws-c-io|0.14.0|mkl_random|1.2.5|
|aws-c-mqtt|0.10.1|ml_dtypes|0.2.0|
|aws-c-s3|0.4.9|mlflow-skinny|2.9.2|
|aws-c-sdkutils|0.1.13|mltable|1.6.1|
|aws-checksums|0.1.17|mpc|1.3.1|
|aws-crt-cpp|0.26.0|mpfr|4.2.1|
|aws-sdk-cpp|1.11.210|mpg123|1.32.4|
|azure-ai-ml|1.12.1|mpmath|1.3.0|
|azure-common|1.1.28|msal|1.27.0|
|azure-core|1.30.1|msal|1.30.0|
|azure-datalake-store|0.0.51|msal_extensions|1.1.0|
|azure-graphrbac|0.61.1|msgpack|1.0.8|
|azure-identity|1.15.0|msrest|0.7.1|
|azure-mgmt-authorization|4.0.0|msrestazure|0.6.4|
|azure-mgmt-containerregistry|10.3.0|multidict|6.0.5|
|azure-mgmt-core|1.4.0|multiprocess|0.70.16|
|azure-mgmt-keyvault|10.3.0|munkres|1.1.4|
|azure-mgmt-network|25.2.0|mypy|1.4.1|
|azure-mgmt-resource|23.0.1|mypy-extensions|1.0.0|
|azure-mgmt-storage|21.1.0|mysql-common|8.0.33|
|azure-storage-blob|12.19.0|mysql-libs|8.0.33|
|azure-storage-file-datalake|12.14.0|nbclient|0.10.0|
|azure-storage-file-share|12.15.0|nbconvert-core|7.16.2|
|azure-synapse-ml-predict|1.0.0|nbformat|5.10.2|
|azureml-core|1.55.0|ncurses|6.5|
|azureml-dataprep|5.1.6|ncurses|6.4|
|azureml-dataprep-native|41.0.0|ndg-httpsclient|0.5.1|
|azureml-dataprep-rslex|2.22.2|nest-asyncio|1.6.0|
|azureml-dataset-runtime|1.55.0|networkx|3.2.1|
|azureml-mlflow|1.55.0|**notebookutils**|**1.1.2.34.20240702.2 ⬆️ 1.1.3.34**|
|azureml-opendatasets|1.55.0|nspr|4.35|
|azureml-synapse|0.0.1|nss|3.98|
|azureml-telemetry|1.55.0|numba|0.59.0|
|backcall|0.2.0|numpy|1.23.5|
|backports-tempfile|1.0|**numpy**|**1.23.5 ⬆️ 2.1.1**|
|backports-weakref|1.0.post1|numpy-base|1.26.4|
|bcrypt|4.1.2|oauthlib|3.2.2|
|beautifulsoup4|4.12.2|onnx|1.15.0|
|blas|1.0|opencensus|0.11.4|
|bleach|6.1.0|opencensus-context|0.1.3|
|blinker|1.7.0|opencensus-ext-azure|1.1.13|
|brotli|1.1.0|openjpeg|2.5.2|
|brotli-bin|1.1.0|openpyxl|3.1.2|
|brotli-python|1.1.0|**openssl**|**3.3.1 ⬆️ 3.3.2**|
|bzip2|1.0.8|openssl|3.2.1|
|c-ares|1.27.0|opt_einsum|3.3.0|
|**ca-certificates**|**2024.2.2 ⬆️ 2024.8.30**|orc|1.9.2|
|ca-certificates|2024.2.2|overrides|7.7.0|
|cached-property|1.5.2|packaging|23.2|
|cached_property|1.5.2|packaging|24.1|
|cachetools|5.3.3|pandas|1.5.3|
|cairo|1.18.0|pandas|2.2.2|
|certifi|2024.2.2|pandasql|0.7.3|
|**certifi**|**2024.2.2 ⬆️ 2024.8.30**|pandocfilters|1.5.0|
|cffi|1.16.0|paramiko|3.4.0|
|**cffi**|**1.16.0 ⬆️ 1.17.1**|parso|0.8.4|
|charset-normalizer|3.3.2|parso|0.8.3|
|click|8.1.7|pathos|0.3.2|
|cloudpickle|2.2.1|pathspec|0.12.1|
|clr_loader|0.2.6|patsy|0.5.6|
|colorama|0.4.6|pcre2|10.43|
|comm|0.2.2|pexpect|4.9.0|
|conda-package-handling|2.2.0|pickleshare|0.7.5|
|conda-package-streaming|0.9.0|pillow|10.2.0|
|configparser|6.0.1|pillow|10.4.0|
|contextlib2|21.6.0|pip|22.3.1|
|contourpy|1.2.0|pip|23.1.2|
|**contourpy**|**1.2.1 ⬆️ 1.3.0**|pixman|0.43.2|
|control-script|1.0.3|pkginfo|1.10.0|
|**cryptography**|**43.0.0 ⬆️ 43.0.1**|pkgutil-resolve-name|1.3.10|
|cryptography|41.0.7|platformdirs|3.11.0|
|cycler|0.12.1|platformdirs|4.2.2|
|dash|2.16.1|plotly|5.18.0|
|dash-core-components|2.0.0|ply|3.11|
|dash-html-components|2.0.0|portalocker|2.8.2|
|dash-table|5.0.0|powerbiclient|3.1.1|
|dash_cytoscape|0.2.0|pox|0.3.4|
|databricks-cli|0.18.0|ppft|1.7.6.8|
|dbus|1.13.6|prettytable|3.9.0|
|debugpy|1.8.1|prometheus_client|0.20.0|
|debugpy|1.8.5|prompt-toolkit|3.0.42|
|decorator|5.1.1|prompt-toolkit|3.0.47|
|defusedxml|0.7.1|prompt_toolkit|3.0.42|
|dill|0.3.8|protobuf|4.24.4|
|distlib|0.3.8|psutil|5.9.8|
|docker-py|7.0.0|psutil|6.0.0|
|entrypoints|0.4|pthread-stubs|0.4|
|et_xmlfile|1.1.0|ptyprocess|0.7.0|
|exceptiongroup|1.2.0|pulseaudio-client|16.1|
|exceptiongroup|1.2.2|pure-eval|0.2.3|
|executing|2.0.1|pure_eval|0.2.2|
|**executing**|**2.0.1 ⬆️ 2.1.0**|py-xgboost|2.0.3|
|expat|2.6.2|py4j|0.10.9.7|
|filelock|3.13.1|pyarrow|14.0.2|
|flask|3.0.2|pyasn1|0.5.1|
|flatbuffers|23.5.26|pyasn1-modules|0.3.0|
|fluent-logger|0.10.0|pycairo|1.26.0|
|font-ttf-dejavu-sans-mono|2.37|pycosat|0.6.6|
|font-ttf-inconsolata|3.000|pycparser|2.21|
|font-ttf-source-code-pro|2.038|pycparser|2.22|
|font-ttf-ubuntu|0.83|pydash|7.0.5|
|fontconfig|2.14.2|pygments|2.17.2|
|fonts-conda-ecosystem|1|pygments|2.18.0|
|fonts-conda-forge|1|pygobject|3.48.1|
|fonttools|4.53.1|pyjwt|2.8.0|
|fonttools|4.49.0|pyjwt|2.9.0|
|fqdn|1.5.1|pynacl|1.5.0|
|freetype|2.12.1|pyodbc|5.0.1|
|frozenlist|1.4.1|pyopenssl|23.3.0|
|fsspec|2024.2.0|pyparsing|3.1.2|
|fsspec_wrapper|0.1.13|**pyparsing**|**3.1.2 ⬆️ 3.1.4**|
|fusepy|3.0.1|pyperclip|1.8.2|
|gast|0.5.4|pyqt|5.15.9|
|geographiclib|2.0|pyqt5-sip|12.12.2|
|geopy|2.4.1|pysocks|1.7.1|
|gettext|0.21.1|pyspark|3.4.1.5.3.20230713|
|gevent|23.9.0.post1|pyspark|20240404|
|gflags|2.2.2|python|3.10.13|
|giflib|5.2.1|python|3.10.14|
|gitdb|4.0.11|python-dateutil|2.9.0|
|gitpython|3.1.42|python-dateutil|2.9.0.post0|
|glib|2.80.0|python-fastjsonschema|2.19.1|
|glib-tools|2.80.0|python-flatbuffers|24.3.7|
|glog|0.6.0|python-json-logger|2.0.7|
|gmp|6.3.0|python_abi|3.10|
|gmpy2|2.1.2|pythonnet|3.0.3|
|google-api-core|2.17.1|pytorch|2.0.1|
|google-auth|2.28.2|pytorch-mutex|1.0|
|google-auth-oauthlib|1.2.0|pytz|2023.4|
|google-pasta|0.2.0|pytz|2024.1|
|googleapis-common-protos|1.63.0|pyu2f|0.1.5|
|graphite2|1.3.13|pywin32-on-windows|0.1.0|
|greenlet|3.0.3|pyyaml|6.0.1|
|grpcio|1.59.3|pyzmq|25.1.2|
|gst-plugins-base|1.22.9|**pyzmq**|**25.1.2 ⬆️ 26.2.0**|
|gstreamer|1.22.9|qt-main|5.15.8|
|h5py|3.10.0|rdma-core|50.0|
|harfbuzz|8.3.0|re2|2023.09.01|
|hdf5|1.14.3|readline|8.2|
|html5lib|1.1|referencing|0.33.0|
|humanfriendly|10.0|regex|2023.12.25|
|icu|73.2|requests|2.32.3|
|idna|3.6|requests|2.31.0|
|**idna**|**3.6 ⬆️ 3.8**|requests-oauthlib|1.4.0|
|imageio|2.33.1|retrying|1.3.3|
|importlib-metadata|7.0.2|rfc3339-validator|0.1.4|
|importlib_metadata|7.0.2|rfc3986-validator|0.1.1|
|importlib_resources|6.3.0|rpds-py|0.18.0|
|impulse-python-handler|1.0.22.1.0.0|rsa|4.9|
|interpret|0.5.0|ruamel.yaml|0.18.5|
|interpret-core|0.5.0|ruamel.yaml.clib|0.2.7|
|ipykernel|6.29.3|ruamel_yaml|0.15.80|
|ipykernel|6.29.5|s2n|1.4.1|
|ipython|8.14.0|salib|1.4.8|
|**ipython**|**8.14.0 ⬆️ 8.27.0**|scikit-learn|1.3.2|
|**ipywidgets**|**8.0.7 ⬆️ 8.1.5**|scipy|1.11.4|
|ipywidgets|8.0.7|seaborn|0.13.1|
|isodate|0.6.1|seaborn-base|0.13.1|
|isoduration|20.11.0|secretstorage|3.3.3|
|itsdangerous|2.1.2|send2trash|1.8.2|
|jedi|0.19.1|setuptools|69.2.0|
|jeepney|0.8.0|**setuptools**|**69.2.0 ⬆️ 73.0.1**|
|jinja2|3.1.3|shap|0.44.0|
|jmespath|1.0.1|sip|6.7.12|
|joblib|1.3.2|six|1.16.0|
|jsonpickle|3.0.3|slicer|0.0.7|
|jsonpointer|2.4|smmap|5.0.0|
|jsonschema|4.21.1|snappy|1.1.10|
|jsonschema-specifications|2023.12.1|sniffio|1.3.1|
|jsonschema-with-format-nongpl|4.21.1|soupsieve|2.5|
|jupyter-client|8.6.2|sqlalchemy|2.0.28|
|jupyter-core|5.7.2|sqlanalyticsconnectorpy|1.0.1|
|jupyter-ui-poll|0.2.2|sqlparse|0.4.4|
|jupyter-ui-poll|1.0.0|stack-data|0.6.3|
|jupyter_client|8.6.1|stack_data|0.6.2|
|jupyter_core|5.7.2|statsmodels|0.14.1|
|jupyter_events|0.9.1|strictyaml|1.7.3|
|jupyter_server|2.7.0|sympy|1.12|
|jupyter_server_terminals|0.5.3|synapseml-cognitive|1.0.4|
|**jupyterlab-widgets**|**3.0.11 ⬆️ 3.0.13**|synapseml-core|1.0.4|
|jupyterlab_pygments|0.3.0|synapseml-deep-learning|1.0.4|
|jupyterlab_widgets|3.0.10|synapseml-internal|1.0.4.0.dev1|
|keras|2.15.0|synapseml-lightgbm|1.0.4|
|keyutils|1.6.1|synapseml-opencv|1.0.4|
|**kiwisolver**|**1.4.5 ⬆️ 1.4.7**|synapseml-vw|1.0.4|
|kiwisolver|1.4.5|tabulate|0.9.0|
|knack|0.11.0|tbb|2021.11.0|
|krb5|1.21.2|tenacity|8.2.3|
|lame|3.100|tensorboard|2.15.2|
|lcms2|2.16|tensorboard-data-server|0.7.0|
|ld_impl_linux-64|2.40|tensorflow|2.15.0|
|lerc|4.0.0|tensorflow-base|2.15.0|
|liac-arff|2.5.0|tensorflow-estimator|2.15.0|
|libabseil|20230802.1|termcolor|2.4.0|
|libaec|1.1.2|terminado|0.18.1|
|libarrow|14.0.2|threadpoolctl|3.3.0|
|libarrow-acero|14.0.2|tinycss2|1.2.1|
|libarrow-dataset|14.0.2|tk|8.6.13|
|libarrow-flight|14.0.2|toml|0.10.2|
|libarrow-flight-sql|14.0.2|tomli|2.0.1|
|libarrow-gandiva|14.0.2|toolz|0.12.1|
|libarrow-substrait|14.0.2|tornado|6.4|
|libbrotlicommon|1.1.0|tornado|6.4.1|
|libbrotlidec|1.1.0|tqdm|4.66.2|
|libbrotlienc|1.1.0|traitlets|5.14.2|
|libcap|2.69|traitlets|5.14.3|
|libclang|15.0.7|typed-ast|1.5.5|
|libclang13|15.0.7|types-python-dateutil|2.8.19.20240311|
|libcrc32c|1.1.2|typing-extensions|4.10.0|
|libcups|2.3.3|typing-extensions|4.12.2|
|libcurl|8.5.0|typing_extensions|4.10.0|
|libdeflate|1.19|typing_utils|0.1.0|
|libebm|0.5.0|tzdata|2024a|
|libedit|3.1.20191231|tzdata|2024.1|
|libev|4.33|ucx|1.15.0|
|libevent|2.1.12|unicodedata2|15.1.0|
|libexpat|2.6.2|unixodbc|2.3.12|
|libffi|3.4.2|uri-template|1.3.0|
|libflac|1.4.3|urllib3|2.1.0|
|**libgcc**|**14.1.0**|urllib3|2.2.2|
|libgcc-ng|14.1.0|virtualenv|20.23.1|
|libgcc-ng|13.2.0|wcwidth|0.2.13|
|libgcrypt|1.10.3|webcolors|1.13|
|libgfortran-ng|13.2.0|webencodings|0.5.1|
|libgfortran5|13.2.0|websocket-client|1.7.0|
|libgirepository|1.78.1|werkzeug|3.0.1|
|libglib|2.80.0|wheel|0.42.0|
|libgomp|14.1.0|wheel|0.44.0|
|libgoogle-cloud|2.12.0|widgetsnbextension|4.0.10|
|libgpg-error|1.48|**widgetsnbextension**|**4.0.10 ⬆️ 4.0.13**|
|libgrpc|1.59.3|wrapt|1.14.1|
|libhwloc|2.9.3|xcb-util|0.4.0|
|libiconv|1.17|xcb-util-image|0.4.0|
|libjpeg-turbo|3.0.0|xcb-util-keysyms|0.4.0|
|libllvm14|14.0.6|xcb-util-renderutil|0.3.9|
|libllvm15|15.0.7|xcb-util-wm|0.4.1|
|libnghttp2|1.58.0|xgboost|2.0.3|
|libnl|3.9.0|xkeyboard-config|2.41|
|libnsl|2.0.1|xorg-kbproto|1.0.7|
|libogg|1.3.4|xorg-libice|1.1.1|
|libopus|1.3.1|xorg-libsm|1.2.4|
|libparquet|14.0.2|xorg-libx11|1.8.7|
|libpng|1.6.43|xorg-libxau|1.0.11|
|libpq|16.2|xorg-libxdmcp|1.1.3|
|libprotobuf|4.24.4|xorg-libxext|1.3.4|
|library-metadata-cooker|3.4.1.1|xorg-libxrender|0.9.11|
|libre2-11|2023.09.01|xorg-renderproto|0.11.1|
|libsecret|0.18.8|xorg-xextproto|7.3.0|
|libsndfile|1.2.2|xorg-xf86vidmodeproto|2.3.1|
|libsodium|1.0.18|xorg-xproto|7.0.31|
|libsqlite|3.45.2|xz|5.2.6|
|**libsqlite**|**3.45.2 ⬆️ 3.46.1**|yaml|0.2.5|
|libssh2|1.11.0|yarl|1.9.4|
|libstdcxx-ng|13.2.0|zeromq|4.3.5|
|libsystemd0|255|zipp|3.17.0|
|libthrift|0.19.0|zlib|1.2.13|
|libtiff|4.6.0|zope.event|5.0|
|libutf8proc|2.8.0|zope.interface|6.2|
|libuuid|2.38.1|zstandard|0.22.0|
|libuv|1.48.0|zstd|1.5.5|
|libvorbis|1.3.7|

# Java and Scala Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|HikariCP|2.5.1|json4s-ast|2.12-3.7.0-M11|
|JLargeArrays|1.5|json4s-core|2.12-3.7.0-M11|
|JTransforms|3.1|json4s-jackson|2.12-3.7.0-M11|
|RoaringBitmap|0.9.38|json4s-scalap|2.12-3.7.0-M11|
|ST4|4.0.4|jsr305|3.0.0|
|SparkCustomEvents|3.4.0-1.0.6|jta|1.1|
|TokenLibrary-assembly|4.2.2|jul-to-slf4j|2.0.6|
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
|azure-cosmos-analytics-spark|4_2-12_synapse-2.1.1|microsoft-log4j-etwappender|1.0|
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
|commons-codec|1.15|netty-transport-native-epoll|4.1.87.Final-linux-aarch_64|
|commons-collections|3.2.2|netty-transport-native-epoll|4.1.87.Final-linux-x86_64|
|commons-collections4|4.4|netty-transport-native-kqueue|4.1.87.Final-osx-x86_64|
|commons-compiler|3.1.9|netty-transport-native-kqueue|4.1.87.Final-osx-aarch_64|
|commons-compress|1.22|netty-transport-native-unix-common|4.1.87.Final|
|commons-crypto|1.1.0|**notebook-utils**|**1.1.2-spark34-20240702.2 ⬆️ 1.1.3-spark34**|
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
|delta-core|2.12-2.4.0.19|parquet-common|1.12.3|
|delta-iceberg|2.12-2.4.0.19|parquet-encoding|1.12.3|
|delta-storage|2.4.0.19|parquet-format-structures|1.12.3|
|derby|0.14.2.0|**parquet-hadoop-ms**|**1.12.3**|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|parquet-jackson|1.12.3|
|flatbuffers-java|1.12.0|peregrine-spark|3.4.0-0.10.4|
|fluent-logger|0.3.4-jar-with-dependencies-provided|pickle|1.3|
|gcs-connector-hadoop3|2.2.11-shaded|postgresql|2.2.9|
|genesis-client|2.12-0.28.0-jar-with-dependencies|protobuf-java|2.5.0|
|gson|2.8.9|proton-j|0.33.8|
|guava|4.0.1|py4j|0.10.9.7|
|**hadoop-aliyun**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|qpid-proton-j-extensions|1.2.4|
|**hadoop-annotations**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|rocksdbjni|7.9.2|
|**hadoop-aws**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scala-collection-compat|2.12-2.7.0|
|**hadoop-azure**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scala-compiler|2.12.17|
|**hadoop-azure-datalake**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scala-java8-compat|2.12-0.9.0|
|hadoop-azureml|1.0-fs|scala-library|2.12.17|
|**hadoop-client-api**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scala-parser-combinators|2.12-2.1.1|
|**hadoop-client-runtime**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scala-reflect|2.12.17|
|**hadoop-cloud-storage**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scala-xml|2.12-2.1.0|
|**hadoop-openstack**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|scalactic|2.12-3.2.14|
|hadoop-shaded-guava|1.1.1|shims|0.9.38|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.3.20240722.5 ⬆️ 3.3.4.5.3.20240828.1**|slf4j-api|2.0.6|
|hdinsight-spark-metrics|3.4.0-1.0.6|snappy-java|1.1.10.5|
|hive-common|2.3.9|spark|3.4-rpc-history-server-core_2.12-1.0.0|
|hive-exec|2.3.9-core|spark|3.4-advisor-core_2.12-1.0.18|
|hive-llap-common|2.3.9|spark|3.4-rpc-history-server-app-listener_2.12-1.0.0|
|hive-metastore|2.3.9|**spark-avro**|**2.12-3.4.1 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hive-serde|2.3.9|spark-avro|2.12-3.4.1|
|hive-shims|0.23-2.3.9|**spark-catalyst**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hive-shims|2.3.9|**spark-core**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hive-shims-common|2.3.9|**spark-enhancement**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hive-shims-scheduler|2.3.9|spark-enhancementui|2.12-3.3.0|
|hive-storage-api|2.8.1|**spark-graphx**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hk2-api|2.6.1|**spark-hadoop-cloud**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hk2-locator|2.6.1|**spark-hive**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|hk2-utils|2.6.1|spark-kusto-synapse-connector|3.4_2.12-1.5.1|
|httpclient|4.5.14|**spark-kvstore**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|httpclient5|5.1.3|**spark-launcher**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|httpcore|4.4.16|spark-lighter-contract|2.12-2.0.9_spark-3.4.0_20240703.5|
|httpmime|4.5.13|spark-lighter-core|2.12-2.0.11_spark-3.4.0_20240703.5|
|httpmime|4.5.14|**spark-microsoft-tools**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|impulse-core_spark|3.4_2.12-1.0.22|**spark-mllib**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|impulse-telemetry-mds_spark|3.4_2.12-1.0.22|**spark-mllib-local**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|ini4j|0.5.4|**spark-network-common**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|isolation-forest|3.4.2_2.12-3.0.4|**spark-network-shuffle**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|istack-commons-runtime|3.0.8|**spark-repl**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|ivy|2.5.1|**spark-sketch**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jackson-annotations|2.14.2|**spark-sql**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jackson-core|2.14.2|**spark-sql-kafka**|**0_2.12-3.4.3.5.3.20240722.5 ⬆️ 0_2.12-3.4.3.5.3.20240828.1**|
|jackson-core-asl|1.9.13|**spark-streaming**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jackson-databind|2.14.2|**spark-streaming-kafka**|**0_2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jackson-dataformat-cbor|2.14.2|**spark-streaming-kafka**|**0_2.12-3.4.3.5.3.20240722.5 ⬆️ 0_2.12-3.4.3.5.3.20240828.1**|
|jackson-datatype-jsr310|2.14.2|**spark-tags**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jackson-mapper-asl|1.9.13|**spark-token-provider-kafka**|**0_2.12-3.4.3.5.3.20240722.5 ⬆️ 0_2.12-3.4.3.5.3.20240828.1**|
|jackson-module-scala|2.12-2.14.2|**spark-unsafe**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jakarta.annotation-api|1.3.5|**spark-yarn**|**2.12-3.4.3.5.3.20240722.5 ⬆️ 2.12-3.4.3.5.3.20240828.1**|
|jakarta.inject|2.6.1|spark_diagnostic_cli|2.1.3_spark-3.4.1_20240731.2|
|jakarta.servlet-api|4.0.3|sparklyr-connector|3.4.1-1.0.0273341|
|jakarta.validation-api|2.0.2|sparknativeparquetwriter|2.12-0.15.4|
|jakarta.ws.rs-api|2.1.6|spire|2.12-0.17.0|
|jakarta.xml.bind-api|2.3.2|spire-macros|2.12-0.17.0|
|janino|3.1.9|spire-platform|2.12-0.17.0|
|javassist|3.25.0-GA|spire-util|2.12-0.17.0|
|javatuples|1.2|spray-json|2.12-1.3.5|
|javax.jdo|3.2.0-m3|stax-api|1.0.1|
|javolution|5.5.1|stream|2.9.6|
|jaxb-api|2.2.11|structuredstreamforspark|2.12-3.4.1-2.3.5|
|jaxb-runtime|2.3.2|synapseml-cognitive|2.12-1.0.4|
|jcl-over-slf4j|2.0.6|synapseml-core|2.12-1.0.4|
|jdo-api|3.0.1|synapseml-deep-learning|2.12-1.0.4|
|jdom2|2.0.6|synapseml-internal|2.12-1.0.4.0-spark3.4|
|jersey-client|2.36|synapseml-lightgbm|2.12-1.0.4|
|jersey-common|2.36|synapseml-opencv|2.12-1.0.4|
|jersey-container-servlet|2.36|synapseml-vw|2.12-1.0.4|
|jersey-container-servlet-core|2.36|**synfs**|**1.1.2-spark34-20240702.2 ⬆️ 1.1.3-spark34**|
|jersey-hk2|2.36|threeten-extra|1.7.1|
|jersey-server|2.36|tink|1.7.0|
|jettison|1.1|transaction-api|1.1|
|jetty-util|9.4.54.v20240208|**trident-core**|**1.2.9 ⬆️ 1.2.16**|
|jetty-util-ajax|9.4.54.v20240208|**tridenttokenlibrary-assembly**|**1.9.4 ⬆️ 1.9.5**|
|jline|2.14.6|univocity-parsers|2.9.1|
|joda-time|2.12.2|vw-jni|9.3.0|
|jodd-core|3.5.2|wildfly-openssl|1.0.7.Final|
|jsch|0.1.54|xbean-asm9-shaded|4.22|
|json|3|xz|1.9|
|json|1.8|**zookeeper**|**3.6.3.5.3.20240722.5 ⬆️ 3.6.3.5.3.20240828.1**|
|json|1|**zookeeper-jute**|**3.6.3.5.3.20240722.5 ⬆️ 3.6.3.5.3.20240828.1**|
|json-simple|1.1|zstd-jni|1.5.2-5|
|json-simple|1.1.1|

# R Libraries
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|**DBI**|**1.2.1 ⬆️ 1.2.3**|listenv|0.9.1|
|DiceDesign|1.10|lobstr|1.1.2|
|FabricTelemetry|1.0.2|lubridate|1.9.3|
|GPfit|1.0-8|magrittr|2.0.3|
|**KernSmooth**|**2.23-22 ⬆️ 2.23-24**|maps|3.4.2|
|MASS|7.3-60.0.1|**markdown**|**1.12 ⬆️ 1.13**|
|Matrix|1.6-5|memoise|2.0.1|
|ModelMetrics|1.2.2.2|**methods**|**4.2.3 ⬆️ 4.4.1**|
|R.methodsS3|1.8.2|mgcv|1.9-1|
|R.oo|1.26.0|mime|0.12|
|R.utils|2.12.3|miniUI|0.1.1.1|
|R6|2.5.1|**modeldata**|**1.3.0 ⬆️ 1.4.0**|
|R6P|0.3.0|modelenv|0.1.1|
|RColorBrewer|1.1-3|modelr|0.1.11|
|**RODBC**|**1.3-20 ⬆️ 1.3-23**|**munsell**|**0.5.0 ⬆️ 0.5.1**|
|**Rcpp**|**1.0.12 ⬆️ 1.0.13**|**nlme**|**3.1-164 ⬆️ 3.1-165**|
|SQUAREM|2021.1|nnet|7.3-19|
|TTR|0.24.4|**notebookutils**|**1.1.2.34.20240702.2 ⬆️ 1.1.3.34**|
|**V8**|**4.4.1 ⬆️ 5.0.0**|numDeriv|2016.8-1.1|
|**XML**|**3.99-0.16.1 ⬆️ 3.99-0.17**|**openssl**|**2.1.1 ⬆️ 2.2.1**|
|**arrow**|**12.0.0 ⬆️ 17.0.0**|pROC|1.18.5|
|askpass|1.2.0|**parallel**|**4.2.3 ⬆️ 4.4.1**|
|assertthat|0.2.1|**parallelly**|**1.36.0 ⬆️ 1.38.0**|
|**backports**|**1.4.1 ⬆️ 1.5.0**|**parsnip**|**1.1.1 ⬆️ 1.2.1**|
|**base**|**4.2.3 ⬆️ 4.4.1**|patchwork|1.2.0|
|base64enc|0.1-3|pillar|1.9.0|
|bigD|0.2.0|**pkgbuild**|**1.4.2 ⬆️ 1.4.4**|
|bit|4.0.5|pkgconfig|2.0.3|
|bit64|4.0.5|**pkgdown**|**2.0.7 ⬆️ 2.1.0**|
|**bitops**|**1.0-7 ⬆️ 1.0-8**|**pkgload**|**1.3.4 ⬆️ 1.4.0**|
|blob|1.2.4|**plotly**|**4.10.2 ⬆️ 4.10.4**|
|brew|1.0-10|plyr|1.8.9|
|**brio**|**1.1.4 ⬆️ 1.1.5**|praise|1.0.0|
|**broom**|**1.0.5 ⬆️ 1.0.6**|prettyunits|1.2.0|
|**bslib**|**0.6.1 ⬆️ 0.8.0**|**processx**|**3.8.3 ⬆️ 3.8.4**|
|**cachem**|**1.0.8 ⬆️ 1.1.0**|**prodlim**|**2023.08.28 ⬆️ 2024.06.25**|
|**callr**|**3.7.3 ⬆️ 3.7.6**|profvis|0.3.8|
|**cards**|**0.2.0**|progress|1.2.3|
|caret|6.0-94|progressr|0.14.0|
|cellranger|1.1.0|**promises**|**1.2.1 ⬆️ 1.3.0**|
|class|7.3-22|proxy|0.4-27|
|classInt|0.4-10|pryr|0.1.6|
|**cli**|**3.6.2 ⬆️ 3.6.3**|**ps**|**1.7.6 ⬆️ 1.7.7**|
|clipr|0.8.0|purrr|1.0.2|
|**clock**|**0.7.0 ⬆️ 0.7.1**|**quantmod**|**0.4.25 ⬆️ 0.4.26**|
|**codetools**|**0.2-19 ⬆️ 0.2-20**|**ragg**|**1.2.7 ⬆️ 1.3.2**|
|collections|0.3.7|rappdirs|0.3.3|
|**colorspace**|**2.1-0 ⬆️ 2.1-1**|rbokeh|0.5.2|
|commonmark|1.9.1|rcmdcheck|1.4.0|
|**compiler**|**4.2.3 ⬆️ 4.4.1**|**reactR**|**0.5.0 ⬆️ 0.6.0**|
|config|0.3.2|reactable|0.4.4|
|conflicted|1.2.0|readr|2.1.5|
|**coro**|**1.0.3 ⬆️ 1.0.4**|readxl|1.4.3|
|cpp11|0.4.7|**recipes**|**1.0.9 ⬆️ 1.1.0**|
|**crayon**|**1.5.2 ⬆️ 1.5.3**|rematch|2.0.0|
|credentials|2.0.1|rematch2|2.1.2|
|crosstalk|1.2.1|**remotes**|**2.4.2.1 ⬆️ 2.5.0**|
|**crul**|**1.4.0 ⬆️ 1.5.0**|**reprex**|**2.1.0 ⬆️ 2.1.1**|
|**curl**|**5.1.0 ⬆️ 5.2.1**|reshape2|1.4.4|
|**data.table**|**1.14.10 ⬆️ 1.15.4**|rjson|0.2.21|
|**datasets**|**4.2.3 ⬆️ 4.4.1**|**rlang**|**1.1.3 ⬆️ 1.1.4**|
|**dbplyr**|**2.3.4 ⬆️ 2.5.0**|rlist|0.4.6.2|
|desc|1.4.3|**rmarkdown**|**2.22 ⬆️ 2.27**|
|devtools|2.4.5|**roxygen2**|**7.3.1 ⬆️ 7.3.2**|
|diagram|1.6.5|rpart|4.1.23|
|**dials**|**1.2.0 ⬆️ 1.3.0**|rprojroot|2.0.4|
|diffobj|0.3.5|**rsample**|**1.2.0 ⬆️ 1.2.1**|
|**digest**|**0.6.34 ⬆️ 0.6.36**|**rstudioapi**|**0.15.0 ⬆️ 0.16.0**|
|**doFuture**|**1.0.1**|rversions|2.1.2|
|**downlit**|**0.4.3 ⬆️ 0.4.4**|**rvest**|**1.0.3 ⬆️ 1.0.4**|
|dplyr|1.1.4|**s2**|**1.1.6 ⬆️ 1.1.7**|
|dtplyr|1.3.1|**safetensors**|**0.1.2**|
|e1071|1.7-14|**sass**|**0.4.8 ⬆️ 0.4.9**|
|ellipsis|0.3.2|scales|1.3.0|
|**evaluate**|**0.23 ⬆️ 0.24.0**|selectr|0.4-2|
|fansi|1.0.6|sessioninfo|1.2.2|
|**farver**|**2.1.1 ⬆️ 2.1.2**|**sf**|**1.0-15 ⬆️ 1.0-16**|
|**fastmap**|**1.1.1 ⬆️ 1.2.0**|**sfd**|**0.1.0**|
|fontawesome|0.5.2|**shape**|**1.4.6 ⬆️ 1.4.6.1**|
|forcats|1.0.0|**shiny**|**1.8.0 ⬆️ 1.9.1**|
|foreach|1.5.2|slider|0.3.1|
|**fs**|**1.6.3 ⬆️ 1.6.4**|sourcetools|0.1.7-1|
|furrr|0.3.1|**sparklyr**|**1.8.2 ⬆️ 1.8.6**|
|**future**|**1.33.1 ⬆️ 1.34.0**|**splines**|**4.2.3 ⬆️ 4.4.1**|
|**future.apply**|**1.11.1 ⬆️ 1.11.2**|**stats**|**4.2.3 ⬆️ 4.4.1**|
|gargle|1.5.2|**stats4**|**4.2.3 ⬆️ 4.4.1**|
|generics|0.1.3|**stringi**|**1.8.3 ⬆️ 1.8.4**|
|**gert**|**2.0.1 ⬆️ 2.1.1**|stringr|1.5.1|
|**ggplot2**|**3.4.2 ⬆️ 3.5.1**|**survival**|**3.5-7 ⬆️ 3.7-0**|
|**gh**|**1.4.0 ⬆️ 1.4.1**|sys|3.4.2|
|gistr|0.9.0|**systemfonts**|**1.0.5 ⬆️ 1.1.0**|
|gitcreds|0.1.2|**tcltk**|**4.2.3 ⬆️ 4.4.1**|
|**globals**|**0.16.2 ⬆️ 0.16.3**|**testthat**|**3.2.1 ⬆️ 3.2.1.1**|
|glue|1.7.0|**textshaping**|**0.3.7 ⬆️ 0.4.0**|
|googledrive|2.1.1|tibble|3.2.1|
|googlesheets4|1.1.1|**tidymodels**|**1.1.0 ⬆️ 1.2.0**|
|gower|1.0.1|tidyr|1.3.1|
|**grDevices**|**4.2.3 ⬆️ 4.4.1**|**tidyselect**|**1.2.0 ⬆️ 1.2.1**|
|**graphics**|**4.2.3 ⬆️ 4.4.1**|tidyverse|2.0.0|
|**grid**|**4.2.3 ⬆️ 4.4.1**|timeDate|4032.109|
|**gt**|**0.9.0 ⬆️ 0.11.0**|timechange|0.3.0|
|**gtable**|**0.3.4 ⬆️ 0.3.5**|**tinytex**|**0.49 ⬆️ 0.52**|
|**gtsummary**|**1.7.2 ⬆️ 2.0.0**|**tools**|**4.2.3 ⬆️ 4.4.1**|
|**hardhat**|**1.3.1 ⬆️ 1.4.0**|**torch**|**0.11.0 ⬆️ 0.13.0**|
|haven|2.5.4|triebeard|0.4.1|
|hexbin|1.28.3|**tune**|**1.1.2 ⬆️ 1.2.1**|
|highcharter|0.9.4|tzdb|0.4.0|
|**highr**|**0.10 ⬆️ 0.11**|units|0.8-5|
|hms|1.1.3|urlchecker|1.0.1|
|**htmltools**|**0.5.7 ⬆️ 0.5.8.1**|urltools|1.7.3|
|htmlwidgets|1.6.4|**usethis**|**2.2.2 ⬆️ 3.0.0**|
|httpcode|0.3.0|utf8|1.2.4|
|**httpuv**|**1.6.14 ⬆️ 1.6.15**|**utils**|**4.2.3 ⬆️ 4.4.1**|
|httr|1.4.7|**uuid**|**1.2-0 ⬆️ 1.2-1**|
|**httr2**|**1.0.0 ⬆️ 1.0.2**|vctrs|0.6.5|
|ids|1.0.1|viridisLite|0.4.2|
|**igraph**|**1.6.0 ⬆️ 2.0.3**|vroom|1.6.5|
|**infer**|**1.0.6 ⬆️ 1.0.7**|waldo|0.5.2|
|ini|0.3.1|warp|0.2.1|
|**ipred**|**0.9-14 ⬆️ 0.9-15**|whisker|0.4.1|
|isoband|0.2.7|**withr**|**3.0.0 ⬆️ 3.0.1**|
|iterators|1.0.14|**wk**|**0.9.1 ⬆️ 0.9.2**|
|jose|1.2.0|**workflows**|**1.1.3 ⬆️ 1.1.4**|
|jquerylib|0.1.4|**workflowsets**|**1.0.1 ⬆️ 1.1.0**|
|jsonlite|1.8.8|**xfun**|**0.41 ⬆️ 0.46**|
|juicyjuice|0.1.0|**xgboost**|**1.7.4.1 ⬆️ 1.7.8.1**|
|**knitr**|**1.45 ⬆️ 1.48**|xml2|1.3.6|
|labeling|0.4.3|**xopen**|**1.0.0 ⬆️ 1.0.1**|
|later|1.3.2|xtable|1.8-4|
|**lattice**|**0.22-5 ⬆️ 0.22-6**|**xts**|**0.13.2 ⬆️ 0.14.0**|
|lava|1.7.3|**yaml**|**2.3.8 ⬆️ 2.3.10**|
|lazyeval|0.2.2|**yardstick**|**1.3.0 ⬆️ 1.3.1**|
|**lhs**|**1.1.6 ⬆️ 1.2.0**|zip|2.3.1|
|lifecycle|1.0.4|zoo|1.8-12|
|**lightgbm**|**3.3.5 ⬆️ 4.5.0**|

