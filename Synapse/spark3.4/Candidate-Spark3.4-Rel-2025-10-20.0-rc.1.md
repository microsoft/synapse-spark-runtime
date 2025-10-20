# System Environment
*   **Product**: Synapse Spark 3.4
*   **VHD Name**: ede5237424f14c.vhd
*   **Vhd Release**: Spark3.4-Rel-2025-10-20.0-rc.1
*   **Operating System**: CBL-Mariner 2.0.20251010
*   **Apache Spark**: 3.4.3
*   **Java**: 11.0.27
*   **Scala**: 2.12.17
*   **Python**: 3.10/2.0.0
*   **Delta Lake**: 2.4.0.25

# New Features
|Id|Component|Description|
|-----|-----|-----|
|1693565|Wildfire/spark34:1.9.34.1|Introduces Spark 3.4 release with updates to Wildfire Spark, including enhanced logging for spark-submit processes to improve debugging and error identification.|
|1683712|Wildfire/spark34:1.9.33|Introduces Spark 3.4 release with updates to wildfire-spark.|


# Improvements
|Id|Component|Description|
|-----|-----|-----|
|1703358|FabricDWConnector:1.0.12|Updates Fabric DW Connector with changes to support workspace private link and improved endpoint handling using the new DW API and methods from Trident Core.|
|1702900|CSparkMetricsUpdate:1.0.12|Enhances security by sanitizing sensitive credentials from Spark execution logs, reducing exposure risks for credentials in CSparkSqlExecution events.|
|1693565|Wildfire/spark34:1.9.34.1|Introduces Spark 3.4 release with updates to Wildfire Spark, including enhanced logging for spark-submit processes to improve debugging and error identification.|
|1700969|KustoConnector:1.5.3|Upgraded connector version with updated CustomSparkMetric and TokenLib|
|1697419|Conda:8.0.43|Updates sempy and flaml in conda for Spark 3.4, incorporating bug fixes, improved error handling, enhanced functionality, and support for additional features like Fabric folders and ISO language codes.|
|1683712|Wildfire/spark34:1.9.33|Introduces Spark 3.4 release with updates to wildfire-spark.|


# Bug Fixes
|Id|Component|Description|
|-----|-----|-----|
|1799850|Wildfire/spark34:1.9.35|Spark 3.4 Release with changes in wildfire-spark, wildfire-hadoop|
|1756998|LibraryManager:1.0.30|LibraryManager update with security fixes to redact tokens from user-facing env.yml logs.|
|1711356|AutoscaleProbe:3.9.7|Introduces Autoscale probe version 3.9.7 with a bug fix for scaledown nodes having shuffle data, increasing the graceful decommission timeout to 20 hours to address `ShuffleFetchFailureException`.|
|1682041|OnelakeSparkCatalog:0.2.12, TridentCore:1.2.24, Delta:2.4.0.25|Fixes Delta.forName to support multipart names, enabling the use of Delta-specific syntaxes like merge, vacuum, and optimize with namespaces in Spark. Addresses an issue with Onelake Spark Catalog integration.|


# Components
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|**AutoscaleProbe**|**3.9.6 ⬆️ 3.9.7**|OneLakeClientStarter|1.0.26.2|
|Autotune|1.11.1.1|**OnelakeSparkCatalog**|**0.2.7 ⬆️ 0.2.12**|
|AzureMLExtensions|1.0.4|Peregrine|0.10.4|
|**Conda**|**8.0.42 ⬆️ 8.0.43**|PostgreSQLJDBCDriver|1.0.3|
|CosmosDBConnector|2.2.5|Python|3.10/2.0.0|
|**CSparkMetricUpdate**|**1.0.11 ⬆️ 1.0.12**|R|1.0.7|
|**Delta**|**2.4.0.24 ⬆️ 2.4.0.25**|SparkAdvisor|1.0.5|
|**DSCopilot**|**1.1.0 ⬆️ 1.2.0**|SparkDiagnosticsLibrary|1.0.31|
|DSCopilotInstaller|1.0.1|SparkLighter|2.1.0|
|DWConnector|1.0.4|SparklyrConnector|1.0.1|
|EventHubConnector|2.3.26|SparkNativeParquetWriter|1.2.0-20250515.2|
|ExternalHiveMetastoreLibraries|0.0.7|SparkRPCHistoryServer|1.6.0|
|**FabricDWConnector**|**1.0.11 ⬆️ 1.0.12**|SQLServerODBCDriver|18.1.0|
|FsspecWrapper|1.0.18|SStreamOnSparkJar|2.3.5.1|
|Genesis|0.33.1|TokenLibrary|4.3.8|
|HiveMetaStoreClient|1.1.21.2|**TridentCore**|**1.2.23 ⬆️ 1.2.25**|
|Impulse|1.2.5|**TridentTokenLibrary**|**1.9.10 ⬆️ 1.9.14**|
|**KustoConnector**|**1.5.1 ⬆️ 1.5.3**|Vegas|3.4.09.03|
|**LibraryManager**|**1.0.29 ⬆️ 1.0.30**|VPaaSClient|3.4.01|
|LibraryMetadataCooker|2.0.3|**Wildfire**|**1.9.32.1 ⬆️ 1.9.35.1**|
|MachineLearningPredict|1.0.2|
|MlflowLibrary|2.6.0.1|
|MMLSpark|1.4.20|
|MySQLJavaConnector|1.0.3|
|NotebookUtils|1.1.62.2|

# Python Modules
|Name|Version|Name|Version|
|-----|-----|-----|-----|
|_libgcc_mutex|0.1|**libuuid**|**2.38.1 ⬆️ 2.41.2**|
|_openmp_mutex|4.5|libuv|1.48.0|
|_py-xgboost-mutex|2.0|libvorbis|1.3.7|
|absl-py|2.1.0|libwebp-base|1.3.2|
|adal|1.2.7|libxcb|1.15|
|adlfs|2023.10.0|libxcrypt|4.4.36|
|aiohttp|3.9.3|libxgboost|2.0.3|
|aiosignal|1.3.1|libxkbcommon|1.6.0|
|alsa-lib|1.2.11|libxml2|2.12.5|
|anyio|3.7.1|libxslt|1.1.39|
|applicationinsights|0.11.10|libzlib|1.2.13|
|argcomplete|3.2.3|libzlib|1.3.1|
|argon2-cffi|23.1.0|lightgbm|4.2.0|
|argon2-cffi-bindings|21.2.0|llvm-openmp|17.0.6|
|arrow|1.3.0|llvmlite|0.42.0|
|asttokens|2.4.1|lxml|5.1.0|
|asttokens|3.0.0|lz4-c|1.9.4|
|astunparse|1.6.3|markdown|3.5.1|
|async-timeout|4.0.3|markupsafe|2.1.5|
|attr|2.5.1|marshmallow|3.21.1|
|attrs|23.2.0|matplotlib|3.8.2|
|aws-c-auth|0.7.11|**matplotlib**|**3.8.2 ⬆️ 3.10.7**|
|aws-c-cal|0.6.9|matplotlib-base|3.8.2|
|aws-c-common|0.9.12|matplotlib-inline|0.1.6|
|aws-c-compression|0.2.17|matplotlib-inline|0.1.7|
|aws-c-event-stream|0.4.1|mistune|3.0.2|
|aws-c-http|0.8.0|mkl|2023.2.0|
|aws-c-io|0.14.0|mkl-service|2.4.1|
|aws-c-mqtt|0.10.1|mkl_fft|1.3.8|
|aws-c-s3|0.4.9|mkl_random|1.2.5|
|aws-c-sdkutils|0.1.13|ml_dtypes|0.2.0|
|aws-checksums|0.1.17|mlflow-skinny|2.9.2|
|aws-crt-cpp|0.26.0|mltable|1.6.1|
|aws-sdk-cpp|1.11.210|mpc|1.3.1|
|azure-ai-ml|1.12.1|mpfr|4.2.1|
|azure-common|1.1.28|mpg123|1.32.4|
|azure-core|1.30.1|mpmath|1.3.0|
|azure-datalake-store|0.0.51|msal|1.27.0|
|azure-graphrbac|0.61.1|**msal**|**1.27.0 ⬆️ 1.34.0**|
|azure-identity|1.15.0|msal_extensions|1.1.0|
|azure-mgmt-authorization|4.0.0|msgpack|1.0.8|
|azure-mgmt-containerregistry|10.3.0|msrest|0.7.1|
|azure-mgmt-core|1.4.0|msrestazure|0.6.4|
|azure-mgmt-keyvault|10.3.0|multidict|6.0.5|
|azure-mgmt-network|25.2.0|multiprocess|0.70.16|
|azure-mgmt-resource|23.0.1|munkres|1.1.4|
|azure-mgmt-storage|21.1.0|mypy|1.4.1|
|azure-storage-blob|12.19.0|mypy-extensions|1.0.0|
|azure-storage-file-datalake|12.14.0|mypy-extensions|1.1.0|
|azure-storage-file-share|12.15.0|mysql-common|8.0.33|
|azureml-core|1.55.0|mysql-libs|8.0.33|
|azureml-dataprep|5.1.6|nbclient|0.10.0|
|azureml-dataprep-native|41.0.0|nbconvert-core|7.16.2|
|azureml-dataprep-rslex|2.22.2|nbformat|5.10.2|
|azureml-dataset-runtime|1.55.0|ncurses|6.4|
|azureml-mlflow|1.55.0|ncurses|6.5|
|azureml-opendatasets|1.55.0|ndg-httpsclient|0.5.1|
|azureml-synapse|0.0.1|nest-asyncio|1.6.0|
|azureml-telemetry|1.55.0|networkx|3.2.1|
|backcall|0.2.0|notebookutils|1.1.11.34.20250605.2|
|backports-tempfile|1.0|nspr|4.35|
|backports-weakref|1.0.post1|nss|3.98|
|bcrypt|4.1.2|numba|0.59.0|
|beautifulsoup4|4.12.2|numpy|1.23.5|
|blas|1.0|numpy|2.2.6|
|bleach|6.1.0|numpy-base|1.26.4|
|blinker|1.7.0|oauthlib|3.2.2|
|brotli|1.1.0|onnx|1.15.0|
|brotli-bin|1.1.0|opencensus|0.11.4|
|brotli-python|1.1.0|opencensus-context|0.1.3|
|bzip2|1.0.8|opencensus-ext-azure|1.1.13|
|c-ares|1.27.0|openjpeg|2.5.2|
|**ca-certificates**|**2024.2.2 ⬆️ 2025.10.5**|openpyxl|3.1.2|
|ca-certificates|2024.2.2|**openssl**|**3.2.1 ⬆️ 3.5.4**|
|cached-property|1.5.2|openssl|3.2.1|
|cached_property|1.5.2|opt_einsum|3.3.0|
|cachetools|5.3.3|orc|1.9.2|
|cairo|1.18.0|overrides|7.7.0|
|certifi|2024.2.2|packaging|25.0|
|**certifi**|**2025.6.15 ⬆️ 2025.10.5**|packaging|23.2|
|**cffi**|**1.16.0 ⬆️ 2.0.0**|pandas|1.5.3|
|cffi|1.16.0|**pandas**|**2.3.0 ⬆️ 2.3.3**|
|**charset-normalizer**|**3.3.2 ⬆️ 3.4.4**|pandasql|0.7.3|
|charset-normalizer|3.3.2|pandocfilters|1.5.0|
|click|8.1.7|paramiko|3.4.0|
|cloudpickle|2.2.1|parso|0.8.3|
|clr_loader|0.2.6|**parso**|**0.8.4 ⬆️ 0.8.5**|
|colorama|0.4.6|pathos|0.3.2|
|**comm**|**0.2.2 ⬆️ 0.2.3**|pathspec|0.12.1|
|comm|0.2.2|patsy|0.5.6|
|conda-package-handling|2.2.0|pcre2|10.43|
|conda-package-streaming|0.9.0|pexpect|4.9.0|
|configparser|6.0.1|pickleshare|0.7.5|
|contextlib2|21.6.0|pillow|10.2.0|
|contourpy|1.2.0|**pillow**|**11.2.1 ⬆️ 12.0.0**|
|contourpy|1.3.2|pip|23.1.2|
|control-script|1.0.3|pip|22.3.1|
|cryptography|41.0.7|pixman|0.43.2|
|**cryptography**|**45.0.4 ⬆️ 46.0.3**|pkginfo|1.10.0|
|cycler|0.12.1|pkgutil-resolve-name|1.3.10|
|dash|2.16.1|**platformdirs**|**4.3.8 ⬆️ 4.5.0**|
|dash-core-components|2.0.0|platformdirs|3.11.0|
|dash-html-components|2.0.0|plotly|5.18.0|
|dash-table|5.0.0|ply|3.11|
|dash_cytoscape|0.2.0|portalocker|2.8.2|
|databricks-cli|0.18.0|powerbiclient|3.1.1|
|dbus|1.13.6|pox|0.3.4|
|debugpy|1.8.1|ppft|1.7.6.8|
|**debugpy**|**1.8.1 ⬆️ 1.8.17**|prettytable|3.9.0|
|decorator|5.1.1|prometheus_client|0.20.0|
|decorator|5.2.1|prompt-toolkit|3.0.42|
|defusedxml|0.7.1|**prompt-toolkit**|**3.0.51 ⬆️ 3.0.52**|
|dill|0.3.8|prompt_toolkit|3.0.42|
|distlib|0.3.8|protobuf|4.24.4|
|docker-py|7.0.0|psutil|5.9.8|
|entrypoints|0.4|**psutil**|**7.0.0 ⬆️ 7.1.1**|
|et_xmlfile|1.1.0|pthread-stubs|0.4|
|exceptiongroup|1.2.0|ptyprocess|0.7.0|
|exceptiongroup|1.3.0|pulseaudio-client|16.1|
|executing|2.0.1|pure-eval|0.2.3|
|**executing**|**2.0.1 ⬆️ 2.2.1**|pure_eval|0.2.2|
|expat|2.6.2|py-xgboost|2.0.3|
|filelock|3.13.1|py4j|0.10.9.7|
|flask|3.0.2|pyarrow|14.0.2|
|flatbuffers|23.5.26|pyasn1|0.5.1|
|fluent-logger|0.10.0|pyasn1-modules|0.3.0|
|font-ttf-dejavu-sans-mono|2.37|pycairo|1.26.0|
|font-ttf-inconsolata|3.000|pycosat|0.6.6|
|font-ttf-source-code-pro|2.038|**pycparser**|**2.21 ⬆️ 2.23**|
|font-ttf-ubuntu|0.83|pycparser|2.21|
|fontconfig|2.14.2|pydash|7.0.5|
|fonts-conda-ecosystem|1|pygments|2.19.2|
|fonts-conda-forge|1|pygments|2.17.2|
|fonttools|4.49.0|pygobject|3.48.1|
|**fonttools**|**4.58.4 ⬆️ 4.60.1**|pyjwt|2.8.0|
|fqdn|1.5.1|pyjwt|2.10.1|
|freetype|2.12.1|pynacl|1.5.0|
|frozenlist|1.4.1|pyodbc|5.0.1|
|fsspec|2024.2.0|pyopenssl|23.3.0|
|fsspec_wrapper|0.1.13|**pyparsing**|**3.2.3 ⬆️ 3.2.5**|
|fusepy|3.0.1|pyparsing|3.1.2|
|gast|0.5.4|pyperclip|1.8.2|
|geographiclib|2.0|pyqt|5.15.9|
|geopy|2.4.1|pyqt5-sip|12.12.2|
|gettext|0.21.1|pysocks|1.7.1|
|gevent|23.9.0.post1|pyspark|20240404|
|gflags|2.2.2|pyspark|3.4.1.5.3.20230713|
|giflib|5.2.1|**python**|**3.10.13 ⬆️ 3.10.19**|
|gitdb|4.0.11|python|3.10.13|
|gitpython|3.1.42|python-dateutil|2.9.0.post0|
|glib|2.80.0|python-dateutil|2.9.0|
|glib-tools|2.80.0|python-fastjsonschema|2.19.1|
|glog|0.6.0|python-flatbuffers|24.3.7|
|gmp|6.3.0|python-json-logger|2.0.7|
|gmpy2|2.1.2|python_abi|3.10|
|google-api-core|2.17.1|pythonnet|3.0.3|
|google-auth|2.28.2|pytorch|2.0.1|
|google-auth-oauthlib|1.2.0|pytorch-mutex|1.0|
|google-pasta|0.2.0|pytz|2023.4|
|googleapis-common-protos|1.63.0|pytz|2025.2|
|graphite2|1.3.13|pyu2f|0.1.5|
|greenlet|3.0.3|pywin32-on-windows|0.1.0|
|grpcio|1.59.3|pyyaml|6.0.1|
|gst-plugins-base|1.22.9|**pyzmq**|**25.1.2 ⬆️ 27.1.0**|
|gstreamer|1.22.9|pyzmq|25.1.2|
|h5py|3.10.0|qt-main|5.15.8|
|harfbuzz|8.3.0|rdma-core|50.0|
|hdf5|1.14.3|re2|2023.09.01|
|html5lib|1.1|readline|8.2|
|humanfriendly|10.0|referencing|0.33.0|
|icu|73.2|regex|2023.12.25|
|**idna**|**3.10 ⬆️ 3.11**|**requests**|**2.31.0 ⬆️ 2.32.5**|
|idna|3.6|requests|2.31.0|
|imageio|2.33.1|requests-oauthlib|1.4.0|
|importlib-metadata|7.0.2|retrying|1.3.3|
|importlib_metadata|7.0.2|rfc3339-validator|0.1.4|
|importlib_resources|6.3.0|rfc3986-validator|0.1.1|
|impulse-python-handler|1.0.22.1.0.0|rpds-py|0.18.0|
|interpret|0.5.0|rsa|4.9|
|interpret-core|0.5.0|ruamel.yaml|0.18.5|
|ipykernel|6.29.3|ruamel.yaml.clib|0.2.7|
|**ipykernel**|**6.29.3 ⬆️ 7.0.1**|ruamel_yaml|0.15.80|
|ipython|8.14.0|s2n|1.4.1|
|ipython|8.37.0|salib|1.4.8|
|ipywidgets|8.0.7|scikit-learn|1.3.2|
|ipywidgets|8.1.7|scipy|1.11.4|
|isodate|0.6.1|seaborn|0.13.1|
|isoduration|20.11.0|seaborn-base|0.13.1|
|itsdangerous|2.1.2|secretstorage|3.3.3|
|jedi|0.19.2|send2trash|1.8.2|
|jedi|0.19.1|setuptools|80.9.0|
|jeepney|0.8.0|setuptools|69.2.0|
|jinja2|3.1.3|shap|0.44.0|
|jmespath|1.0.1|sip|6.7.12|
|joblib|1.3.2|six|1.17.0|
|jsonpickle|3.0.3|six|1.16.0|
|jsonpointer|2.4|slicer|0.0.7|
|jsonschema|4.21.1|smmap|5.0.0|
|jsonschema-specifications|2023.12.1|snappy|1.1.10|
|jsonschema-with-format-nongpl|4.21.1|sniffio|1.3.1|
|jupyter-client|8.6.3|soupsieve|2.5|
|**jupyter-core**|**5.8.1 ⬆️ 5.9.1**|sqlalchemy|2.0.28|
|jupyter-ui-poll|1.0.0|sqlanalyticsconnectorpy|1.0.1|
|jupyter-ui-poll|0.2.2|sqlparse|0.4.4|
|jupyter_client|8.6.1|stack-data|0.6.3|
|jupyter_core|5.7.2|stack_data|0.6.2|
|jupyter_events|0.9.1|statsmodels|0.14.1|
|jupyter_server|2.7.0|strictyaml|1.7.3|
|jupyter_server_terminals|0.5.3|sympy|1.12|
|jupyterlab-widgets|3.0.15|synapseml-cognitive|1.0.9|
|jupyterlab_pygments|0.3.0|synapseml-core|1.0.9|
|jupyterlab_widgets|3.0.10|synapseml-deep-learning|1.0.9|
|keras|2.15.0|synapseml-internal|1.0.9.0.dev1|
|keyutils|1.6.1|synapseml-lightgbm|1.0.9|
|**kiwisolver**|**1.4.5 ⬆️ 1.4.9**|synapseml-opencv|1.0.9|
|kiwisolver|1.4.5|synapseml-vw|1.0.9|
|knack|0.11.0|tabulate|0.9.0|
|krb5|1.21.2|tbb|2021.11.0|
|lame|3.100|tenacity|8.2.3|
|lcms2|2.16|tensorboard|2.15.2|
|ld_impl_linux-64|2.40|tensorboard-data-server|0.7.0|
|**ld_impl_linux-64**|**2.40 ⬆️ 2.44**|tensorflow|2.15.0|
|lerc|4.0.0|tensorflow-base|2.15.0|
|liac-arff|2.5.0|tensorflow-estimator|2.15.0|
|libabseil|20230802.1|termcolor|2.4.0|
|libaec|1.1.2|terminado|0.18.1|
|libarrow|14.0.2|threadpoolctl|3.3.0|
|libarrow-acero|14.0.2|tinycss2|1.2.1|
|libarrow-dataset|14.0.2|tk|8.6.13|
|libarrow-flight|14.0.2|toml|0.10.2|
|libarrow-flight-sql|14.0.2|**tomli**|**2.0.1 ⬆️ 2.3.0**|
|libarrow-gandiva|14.0.2|tomli|2.0.1|
|libarrow-substrait|14.0.2|toolz|0.12.1|
|libbrotlicommon|1.1.0|**tornado**|**6.4 ⬆️ 6.5.2**|
|libbrotlidec|1.1.0|tornado|6.4|
|libbrotlienc|1.1.0|tqdm|4.66.2|
|libcap|2.69|traitlets|5.14.3|
|libclang|15.0.7|traitlets|5.14.2|
|libclang13|15.0.7|typed-ast|1.5.5|
|libcrc32c|1.1.2|types-python-dateutil|2.8.19.20240311|
|libcups|2.3.3|typing-extensions|4.10.0|
|libcurl|8.5.0|**typing-extensions**|**4.10.0 ⬆️ 4.15.0**|
|libdeflate|1.19|typing_extensions|4.10.0|
|libebm|0.5.0|typing_utils|0.1.0|
|libedit|3.1.20191231|tzdata|2024a|
|libev|4.33|tzdata|2025.2|
|libevent|2.1.12|ucx|1.15.0|
|libexpat|2.6.2|unicodedata2|15.1.0|
|**libexpat**|**2.6.2 ⬆️ 2.7.1**|unixodbc|2.3.12|
|libffi|3.4.2|uri-template|1.3.0|
|**libffi**|**3.4.2 ⬆️ 3.5.2**|urllib3|2.5.0|
|libflac|1.4.3|urllib3|2.1.0|
|**libgcc**|**15.1.0 ⬆️ 15.2.0**|virtualenv|20.23.1|
|libgcc-ng|13.2.0|wcwidth|0.2.13|
|**libgcc-ng**|**13.2.0 ⬆️ 15.2.0**|**wcwidth**|**0.2.13 ⬆️ 0.2.14**|
|libgcrypt|1.10.3|webcolors|1.13|
|libgfortran-ng|13.2.0|webencodings|0.5.1|
|libgfortran5|13.2.0|websocket-client|1.7.0|
|libgirepository|1.78.1|werkzeug|3.0.1|
|libglib|2.80.0|wheel|0.42.0|
|**libgomp**|**15.1.0 ⬆️ 15.2.0**|wheel|0.45.1|
|libgoogle-cloud|2.12.0|widgetsnbextension|4.0.14|
|libgpg-error|1.48|widgetsnbextension|4.0.10|
|libgrpc|1.59.3|wrapt|1.14.1|
|libhwloc|2.9.3|xcb-util|0.4.0|
|libiconv|1.17|xcb-util-image|0.4.0|
|libjpeg-turbo|3.0.0|xcb-util-keysyms|0.4.0|
|libllvm14|14.0.6|xcb-util-renderutil|0.3.9|
|libllvm15|15.0.7|xcb-util-wm|0.4.1|
|liblzma|5.8.1|xgboost|2.0.3|
|libnghttp2|1.58.0|xkeyboard-config|2.41|
|libnl|3.9.0|xorg-kbproto|1.0.7|
|libnsl|2.0.1|xorg-libice|1.1.1|
|libogg|1.3.4|xorg-libsm|1.2.4|
|libopus|1.3.1|xorg-libx11|1.8.7|
|libparquet|14.0.2|xorg-libxau|1.0.11|
|libpng|1.6.43|xorg-libxdmcp|1.1.3|
|libpq|16.2|xorg-libxext|1.3.4|
|libprotobuf|4.24.4|xorg-libxrender|0.9.11|
|library-metadata-cooker|3.4.1.2|xorg-renderproto|0.11.1|
|libre2-11|2023.09.01|xorg-xextproto|7.3.0|
|libsecret|0.18.8|xorg-xf86vidmodeproto|2.3.1|
|libsndfile|1.2.2|xorg-xproto|7.0.31|
|libsodium|1.0.18|xz|5.2.6|
|libsqlite|3.45.2|yaml|0.2.5|
|**libsqlite**|**3.45.2 ⬆️ 3.50.4**|yarl|1.9.4|
|libssh2|1.11.0|zeromq|4.3.5|
|libstdcxx-ng|13.2.0|zipp|3.17.0|
|libsystemd0|255|zlib|1.2.13|
|libthrift|0.19.0|zope.event|5.0|
|libtiff|4.6.0|zope.interface|6.2|
|libutf8proc|2.8.0|zstandard|0.22.0|
|libuuid|2.38.1|zstd|1.5.5|

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
|**delta-storage**|**2.4.0.24 ⬆️ 2.4.0.25**|**parquet-hadoop-ms**|**3.4.3.5.3.20250511.1 ⬆️ 3.4.3.5.3.20250911.1**|
|derby|0.14.2.0|parquet-jackson|1.12.3|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|peregrine-spark|3.4.0-0.10.4|
|flatbuffers-java|1.12.0|pickle|1.3|
|fluent-logger|0.3.4-jar-with-dependencies-provided|postgresql|2.2.9|
|gcs-connector-hadoop3|2.2.11-shaded|protobuf-java|2.5.0|
|genesis-client|2.12-0.33.1-jar-with-dependencies|proton-j|0.33.8|
|gson|2.8.9|py4j|0.10.9.7|
|guava|4.0.1|qpid-proton-j-extensions|1.2.4|
|**hadoop-aliyun**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|rocksdbjni|7.9.2|
|**hadoop-annotations**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scala-collection-compat|2.12-2.7.0|
|**hadoop-aws**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scala-compiler|2.12.17|
|**hadoop-azure**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scala-java8-compat|2.12-0.9.0|
|**hadoop-azure-datalake**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scala-library|2.12.17|
|hadoop-azureml|1.0-fs|scala-parser-combinators|2.12-2.1.1|
|**hadoop-client-api**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scala-reflect|2.12.17|
|**hadoop-client-runtime**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scala-xml|2.12-2.1.0|
|**hadoop-cloud-storage**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|scalactic|2.12-3.2.14|
|**hadoop-openstack**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|shims|0.9.38|
|hadoop-shaded-guava|1.1.1|slf4j-api|2.0.6|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.3.20250511.1 ⬆️ 3.3.4.5.3.20250911.1**|snappy-java|1.1.10.5|
|**hdinsight-spark-metrics**|**3.4.0-1.0.10 ⬆️ 3.4.0-1.0.11**|spark|3.4-rpc-history-server-app-listener_2.12-1.0.0|
|hive-common|2.3.9|spark|3.4-rpc-history-server-core_2.12-1.0.0|
|hive-exec|2.3.9-core|spark|3.4-advisor-core_2.12-1.0.18|
|hive-llap-common|2.3.9|spark-avro|2.12-3.4.1|
|hive-metastore|2.3.9|**spark-avro**|**2.12-3.4.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hive-serde|2.3.9|**spark-catalyst**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hive-shims|2.3.9|**spark-core**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hive-shims|0.23-2.3.9|**spark-enhancement**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hive-shims-common|2.3.9|spark-enhancementui|2.12-3.3.0|
|hive-shims-scheduler|2.3.9|**spark-graphx**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hive-storage-api|2.8.1|**spark-hadoop-cloud**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hk2-api|2.6.1|**spark-hive**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|hk2-locator|2.6.1|**spark-kusto-synapse-connector**|**3.4_2.12-1.5.1 ⬆️ 3.4_2.12-1.5.3**|
|hk2-utils|2.6.1|**spark-kvstore**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|httpclient|4.5.14|**spark-launcher**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|httpclient5|5.1.3|spark-lighter-contract|2.12-2.0.9_spark-3.4.0_20240703.5|
|httpcore|4.4.16|spark-lighter-core|2.12-2.0.11_spark-3.4.0_20241101.1|
|httpmime|4.5.14|**spark-microsoft-tools**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|httpmime|4.5.13|**spark-mllib**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|impulse-core_spark|3.4_2.12-1.0.22|**spark-mllib-local**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|impulse-telemetry-mds_spark|3.4_2.12-1.0.22|**spark-network-common**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|ini4j|0.5.4|**spark-network-shuffle**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|isolation-forest|3.4.2_2.12-3.0.4|**spark-repl**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|istack-commons-runtime|3.0.8|**spark-sketch**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|ivy|2.5.1|**spark-sql**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|jackson-annotations|2.14.2|**spark-sql-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 0_2.12-3.4.3.5.3.20250911.1**|
|jackson-core|2.14.2|**spark-streaming**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|jackson-core-asl|1.9.13|**spark-streaming-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 0_2.12-3.4.3.5.3.20250911.1**|
|jackson-databind|2.14.2|**spark-streaming-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|jackson-dataformat-cbor|2.14.2|**spark-tags**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|jackson-datatype-jsr310|2.14.2|**spark-token-provider-kafka**|**0_2.12-3.4.3.5.3.20250511.1 ⬆️ 0_2.12-3.4.3.5.3.20250911.1**|
|jackson-mapper-asl|1.9.13|**spark-unsafe**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
|jackson-module-scala|2.12-2.14.2|**spark-yarn**|**2.12-3.4.3.5.3.20250511.1 ⬆️ 2.12-3.4.3.5.3.20250911.1**|
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
|json|3|**zookeeper**|**3.6.3.5.3.20250511.1 ⬆️ 3.6.3.5.3.20250911.1**|
|json|1.8|**zookeeper-jute**|**3.6.3.5.3.20250511.1 ⬆️ 3.6.3.5.3.20250911.1**|
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

