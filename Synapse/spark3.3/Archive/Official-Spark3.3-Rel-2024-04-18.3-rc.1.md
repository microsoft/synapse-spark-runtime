# System Environment
*   **Vhd Release**: Spark3.3-Rel-2024-04-18.3-rc.1
*   **Operating System**: Ubuntu 18.04.6 LTS
*   **Java**: 1.8.0_402
*   **Scala**: 2.12.15
*   **Python**: 3.10/1.0.5
*   **Delta Lake**: 2.2.0.11

# New Features

|Id|Component|Title|Description|
|-----|-----|-----|-----|
|1316504|Vegas:spark33/3.3.09|Intelligent Cache locality using consistent hashing|Intelligent cache uses placement information to schedule spark tasks on executors. Now we are using consistent hashing to provide locality information.|
|1309131|AutoscaleProbe:3.9.0|Release Autoscale Version 3.9.0|New Autoscale version contains several bug fixes like Autoscale Stuck in Scale Down validation, fixes for incorrect metrics and support for Autoscale in case of cluster fragmentation|
|1309490|Wildfire/spark33:1.7.54|New spark 3.3 stack release|New spark 3.3 stack release. add support for dedicated queues for listeners and CG fixes in spark code. Cred fix in livy code and avoid printing livy configs in livy server logs.|

# Improvements

|Id|Component|Title|Description|
|-----|-----|-----|-----|
|1312504|LibraryManagement:1.0.24|Library management release 1.0.24 with support for arcgis|This new release includes support for arcgis as well as security fixes|

# Bug Fixes

|Id|Component|Title|Description|
|-----|-----|-----|-----|
|1319096|TokenLibrary:3.6.4|The ClientCredsTokenProvider in Synapse will work in Sovereign Clouds with this change|Fixes the issue with the ClientCredsTokenProvider in Synapse not working in Sovereign Clouds due to the AADEndpoint being incorrect.|
|1299440|OneLakeClientStarter:1.0.19.2|Fix for CST clusters SSL configuration|CST clusters which currently use special ssl config is changed to ssl config of the production environment.|
|1305097|Wildfire/spark33:1.7.53|New spark 3.3 stack release. Consist of spark, hadoop, hive, livy and zookeeper release|Bug fix in hadoop code: use graceful decomission timeout based on nodeId instead of nodename.|
|1309131|AutoscaleProbe:3.9.0|Release Autoscale Version 3.9.0|New Autoscale version contains several bug fixes like Autoscale Stuck in Scale Down validation, fixes for incorrect metrics and support for Autoscale in case of cluster fragmentation|
|1309490|Wildfire/spark33:1.7.54|New spark 3.3 stack release|New spark 3.3 stack release. add support for dedicated queues for listeners and CG fixes in spark code. Cred fix in livy code and avoid printing livy configs in livy server logs.|
|1312504|LibraryManagement:1.0.24|Library management release 1.0.24 with support for arcgis|This new release includes support for arcgis as well as security fixes|
|1301017|SparkDiagnosticsLibrary:1.0.20|Optimizing Exception and Status Code Handling and enable executor level log|Enhancements include extending request connection timeout to 15s, re-generating signatures after 403 errors, logging additional request exceptions, and enabling executor log downstream.|

# Components

|Name|Version|
|-----|-----|
|**AutoscaleProbe**|**3.8.1.1 --> 3.9.0**|
|Autotune|1.11.0.0|
|AzureMLExtensions|1.0.3|
|**CDM**|**1.19.7 --> 1.19.5**|
|CSparkMetricUpdate|1.0.2|
|ClusterGateway|spark/2.4.4|
|Conda|1.0.20|
|CosmosDBConnector|1.8.10|
|**DWConnector**|**2.1.1 --> 2.1.2**|
|Delta|2.2.0.11|
|Dotnet|6.0.0|
|EventHubConnector|2.3.24|
|ExternalHiveMetastoreLibraries|0.0.6|
|FsspecWrapper|1.0.12|
|Genesis|0.27.0|
|HiveMetaStoreClient|1.1.17|
|Impulse|1.2.1|
|JupyterServices|0.0.2|
|KustoConnector|1.3.4|
|**LibraryManager**|**1.0.23 --> 1.0.25**|
|LibraryMetadataCooker|1.0.0|
|MMLSpark|1.4.12|
|MachineLearningPredict|1.0.1|
|MlflowLibrary|2.1.1|
|MySQLJavaConnector|1.0.2|
|NotebookUtils|1.1.41|
|**OneLakeClientStarter**|**1.0.19.1 --> 1.0.19.2**|
|OnelakeSparkCatalog|0.1.3|
|Peregrine|0.10.3|
|PostgreSQLJDBCDriver|1.0.2|
|Python|3.10/1.0.5|
|R|1.0.5|
|SQLServerODBCDriver|18.1.0|
|SStreamOnSparkJar|2.3.0|
|SparkAdvisor|0.0.14|
|SparkDiagnosticsLibrary|1.0.20|
|SparkInitialize|1.0.0|
|SparkLighter|2.0.7|
|SparkNativeParquetWriter|0.8.1|
|SparkRPCHistoryServer|1.0.28|
|SparklyrConnector|1.0.0|
|**TokenLibrary**|**3.5.8 --> 3.6.4**|
|TridentCore|1.2.6|
|**TridentTokenLibrary**|**1.6.2 --> 1.6.5**|
|VSANodeScanAgent|1.0.0|
|**Vegas**|**3.3.08.5 --> 3.3.09**|
|**VertiParquet**|**0.8.6 --> 0.8.4**|
|**Wildfire**|**1.7.52 --> 1.7.54**|

# Python Modules
### Environment: Synapse

|Name|Version|
|-----|-----|
|_libgcc_mutex|0.1|
|_openmp_mutex|4.5|
|_py-xgboost-mutex|2.0|
|_tflow_select|2.3.0|
|absl-py|1.3.0|
|adal|1.2.7|
|adlfs|0.7.7|
|aiohttp|3.8.3|
|aiosignal|1.3.1|
|anyio|3.6.2|
|aom|3.5.0|
|applicationinsights|0.11.10|
|argcomplete|2.0.0|
|argon2-cffi|21.3.0|
|argon2-cffi-bindings|21.2.0|
|arrow-cpp|9.0.0|
|asttokens|2.1.0|
|asttokens|2.4.1|
|astunparse|1.6.3|
|async-timeout|4.0.2|
|attrs|22.1.0|
|aws-c-cal|0.5.11|
|aws-c-common|0.6.2|
|aws-c-event-stream|0.2.7|
|aws-c-io|0.10.5|
|aws-checksums|0.1.11|
|aws-sdk-cpp|1.8.186|
|azure-common|1.1.28|
|azure-core|1.26.1|
|azure-datalake-store|0.0.51|
|azure-graphrbac|0.61.1|
|azure-identity|1.7.0|
|azure-mgmt-authorization|2.0.0|
|azure-mgmt-containerregistry|10.0.0|
|azure-mgmt-core|1.3.2|
|azure-mgmt-keyvault|10.1.0|
|azure-mgmt-resource|21.2.1|
|azure-mgmt-storage|20.1.0|
|azure-storage-blob|12.13.0|
|azure-synapse-ml-predict|1.0.0|
|azureml-core|1.47.0|
|azureml-dataprep|4.5.7|
|azureml-dataprep-native|38.0.0|
|azureml-dataprep-rslex|2.11.4|
|azureml-dataset-runtime|1.47.0|
|azureml-mlflow|1.47.0|
|azureml-opendatasets|1.47.0|
|azureml-synapse|0.0.1|
|azureml-telemetry|1.47.0|
|backcall|0.2.0|
|backports|1.0|
|backports-tempfile|1.0|
|backports-weakref|1.0.post1|
|backports.functools_lru_cache|1.6.4|
|bcrypt|4.0.1|
|beautifulsoup4|4.9.3|
|blas|2.116|
|blas-devel|3.9.0|
|bleach|5.0.1|
|blinker|1.5|
|blosc|1.21.1|
|bokeh|3.0.1|
|brotli|1.0.9|
|brotli-bin|1.0.9|
|brotli-python|1.0.9|
|brotlipy|0.7.0|
|brunsli|0.1|
|bzip2|1.0.8|
|c-ares|1.18.1|
|c-blosc2|2.4.3|
|ca-certificates|2022.9.24|
|ca-certificates|2024.2.2|
|cached-property|1.5.2|
|cached_property|1.5.2|
|cachetools|5.2.0|
|certifi|2022.9.24|
|cffi|1.15.1|
|cfitsio|4.1.0|
|charls|2.3.4|
|charset-normalizer|2.1.1|
|click|8.1.3|
|cloudpickle|2.2.0|
|colorama|0.4.6|
|coloredlogs|15.0.1|
|comm|0.2.2|
|conda-package-handling|1.9.0|
|configparser|5.3.0|
|contextlib2|21.6.0|
|**contourpy**|**1.2.0 --> 1.2.1**|
|contourpy|1.0.6|
|control-script|1.0.3|
|cryptography|38.0.3|
|cycler|0.11.0|
|cycler|0.12.1|
|cython|0.29.32|
|cytoolz|0.12.0|
|dash|1.21.0|
|dash-core-components|1.17.1|
|dash-html-components|1.1.4|
|dash-renderer|1.9.1|
|dash-table|4.12.0|
|dash_cytoscape|0.2.0|
|dask-core|2022.10.2|
|databricks-cli|0.17.3|
|dav1d|1.0.0|
|dbus|1.13.6|
|debugpy|1.8.1|
|debugpy|1.6.3|
|decorator|5.1.1|
|defusedxml|0.7.1|
|dill|0.3.6|
|distlib|0.3.6|
|distro|1.8.0|
|docker|6.0.1|
|dotnetcore2|3.1.23|
|entrypoints|0.4|
|et_xmlfile|1.0.1|
|exceptiongroup|1.2.0|
|executing|1.2.0|
|executing|2.0.1|
|expat|2.5.0|
|fastjsonschema|2.16.2|
|filelock|3.8.0|
|fire|0.4.0|
|flask|2.2.2|
|flask-compress|1.13|
|flatbuffers|2.0.7|
|fluent-logger|0.10.0|
|fontconfig|2.14.1|
|**fonttools**|**4.50.0 --> 4.51.0**|
|fonttools|4.38.0|
|freetype|2.12.1|
|frozenlist|1.3.3|
|fsspec|2022.10.0|
|fsspec_wrapper|0.1.7|
|fusepy|3.0.1|
|future|0.18.2|
|gast|0.4.0|
|gensim|4.2.0|
|geographiclib|1.52|
|geopy|2.1.0|
|gettext|0.21.1|
|gevent|22.10.1|
|gflags|2.2.2|
|giflib|5.2.1|
|gitdb|4.0.9|
|gitpython|3.1.29|
|glib|2.74.1|
|glib-tools|2.74.1|
|glog|0.6.0|
|gmp|6.2.1|
|gmpy2|2.1.2|
|google-auth|2.14.0|
|google-auth-oauthlib|0.4.6|
|google-pasta|0.2.0|
|greenlet|1.1.3.post0|
|grpc-cpp|1.46.4|
|grpcio|1.46.4|
|gst-plugins-base|1.14.0|
|gstreamer|1.14.0|
|h5py|3.7.0|
|hdf5|1.12.2|
|html5lib|1.1|
|humanfriendly|10.0|
|hummingbird-ml|0.4.0|
|icu|58.2|
|idna|3.4|
|imagecodecs|2022.9.26|
|imageio|2.9.0|
|importlib-metadata|5.0.0|
|impulse-python-handler|1.0.19.1.0.0|
|interpret|0.2.4|
|interpret-core|0.2.4|
|ipykernel|6.17.0|
|**ipykernel**|**6.17.0 --> 6.29.4**|
|ipython|8.6.0|
|**ipython**|**8.6.0 --> 8.23.0**|
|ipython-genutils|0.2.0|
|ipywidgets|8.1.2|
|ipywidgets|7.7.0|
|isodate|0.6.0|
|itsdangerous|2.1.2|
|jdcal|1.4.1|
|jedi|0.18.1|
|jedi|0.19.1|
|jeepney|0.8.0|
|jinja2|3.1.2|
|jmespath|1.0.1|
|joblib|1.2.0|
|jpeg|9e|
|jsonpickle|2.2.0|
|jsonschema|4.17.0|
|jupyter-client|8.6.1|
|jupyter-core|5.7.2|
|jupyter-server|1.23.0|
|jupyter_client|7.4.4|
|jupyter_core|4.11.2|
|jupyterlab-pygments|0.2.2|
|jupyterlab-widgets|3.0.3|
|jupyterlab-widgets|3.0.10|
|jxrlib|1.1|
|keras|2.8.0|
|keras-applications|1.0.8|
|keras-preprocessing|1.1.2|
|keras2onnx|1.6.5|
|keyutils|1.6.1|
|kiwisolver|1.4.4|
|kiwisolver|1.4.5|
|knack|0.10.0|
|kqlmagiccustom|0.1.114.post16|
|krb5|1.19.3|
|lcms2|2.14|
|ld_impl_linux-64|2.39|
|ld_impl_linux-64|2.40|
|lerc|4.0.0|
|liac-arff|2.5.0|
|libabseil|20220623.0|
|libaec|1.0.6|
|libavif|0.11.1|
|libblas|3.9.0|
|libbrotlicommon|1.0.9|
|libbrotlidec|1.0.9|
|libbrotlienc|1.0.9|
|libcblas|3.9.0|
|libclang|14.0.6|
|libcrc32c|1.1.2|
|libcurl|7.86.0|
|libdeflate|1.14|
|libedit|3.1.20191231|
|libev|4.33|
|libevent|2.1.10|
|libffi|3.4.2|
|libgcc-ng|12.2.0|
|libgcc-ng|13.2.0|
|libgfortran-ng|12.2.0|
|libgfortran5|12.2.0|
|libglib|2.74.1|
|libgomp|13.2.0|
|libgoogle-cloud|2.1.0|
|libiconv|1.17|
|liblapack|3.9.0|
|liblapacke|3.9.0|
|libllvm11|11.1.0|
|libnghttp2|1.47.0|
|libnsl|2.0.1|
|libnsl|2.0.0|
|libpng|1.6.38|
|libprotobuf|3.20.1|
|library-metadata-cooker|0.0.7|
|libsodium|1.0.18|
|libsqlite|3.39.4|
|**libsqlite**|**3.39.4 --> 3.45.3**|
|libssh2|1.10.0|
|libstdcxx-ng|12.2.0|
|libthrift|0.16.0|
|libtiff|4.4.0|
|libutf8proc|2.8.0|
|libuuid|2.32.1|
|libuuid|2.38.1|
|libuv|1.44.2|
|libwebp-base|1.2.4|
|libxcb|1.13|
|libxcrypt|4.4.36|
|libxgboost|1.7.1|
|libxml2|2.9.9|
|libzlib|1.2.13|
|libzopfli|1.0.3|
|lightgbm|3.2.1|
|lime|0.2.0.1|
|llvm-openmp|15.0.4|
|llvmlite|0.39.1|
|locket|1.0.0|
|lxml|4.8.0|
|lz4-c|1.9.3|
|markdown|3.3.4|
|markupsafe|2.1.1|
|**matplotlib**|**3.8.3 --> 3.8.4**|
|matplotlib|3.6.2|
|matplotlib-base|3.6.2|
|**matplotlib-inline**|**0.1.6 --> 0.1.7**|
|matplotlib-inline|0.1.6|
|mistune|2.0.4|
|mkl|2022.1.0|
|mkl-devel|2022.1.0|
|mkl-include|2022.1.0|
|mleap|0.17.0|
|mlflow-skinny|1.30.0|
|mpc|1.2.1|
|mpfr|4.1.0|
|mpmath|1.2.1|
|msal|2022.09.01|
|msal-extensions|0.3.1|
|msgpack|1.0.8|
|msrest|0.7.1|
|msrestazure|0.6.4|
|multidict|6.0.2|
|multiprocess|0.70.14|
|munkres|1.1.4|
|mypy|0.780|
|mypy-extensions|0.4.4|
|mypy-extensions|0.4.3|
|nbclassic|0.4.8|
|nbclient|0.7.0|
|nbconvert|7.2.3|
|nbformat|5.7.0|
|ncurses|6.3|
|ncurses|6.4.20240210|
|ndg-httpsclient|0.5.1|
|nest-asyncio|1.5.6|
|nest-asyncio|1.6.0|
|networkx|2.8.8|
|nltk|3.6.2|
|notebook|6.5.2|
|notebook-shim|0.2.2|
|notebookutils|3.3.0-20240213.4|
|numba|0.56.3|
|numpy|1.23.4|
|numpy|1.26.4|
|oauthlib|3.2.2|
|onnx|1.12.0|
|onnxconverter-common|1.7.0|
|onnxmltools|1.7.0|
|onnxruntime|1.13.1|
|openjpeg|2.5.0|
|openpyxl|3.0.7|
|openssl|1.1.1s|
|openssl|3.2.1|
|opt_einsum|3.3.0|
|orc|1.7.6|
|packaging|21.3|
|packaging|24.0|
|pandas|1.5.1|
|**pandas**|**1.5.1 --> 2.2.2**|
|pandasql|0.7.3|
|pandocfilters|1.5.0|
|paramiko|2.12.0|
|parquet-cpp|1.5.1|
|**parso**|**0.8.3 --> 0.8.4**|
|parso|0.8.3|
|partd|1.3.0|
|pathos|0.3.0|
|pathspec|0.10.1|
|patsy|0.5.3|
|pcre2|10.40|
|pexpect|4.8.0|
|pexpect|4.9.0|
|pickleshare|0.7.5|
|pillow|9.2.0|
|**pillow**|**9.2.0 --> 10.3.0**|
|pip|22.3.1|
|pkginfo|1.8.3|
|platformdirs|2.5.3|
|platformdirs|4.2.0|
|plotly|4.14.3|
|pmdarima|2.0.1|
|portalocker|2.6.0|
|pox|0.3.2|
|ppft|1.7.6.6|
|prettytable|3.2.0|
|prometheus-client|0.15.0|
|prompt-toolkit|3.0.32|
|prompt-toolkit|3.0.43|
|protobuf|3.20.1|
|psutil|5.9.4|
|psutil|5.9.8|
|pthread-stubs|0.4|
|ptyprocess|0.7.0|
|pure-eval|0.2.2|
|pure_eval|0.2.2|
|py-xgboost|1.7.1|
|py4j|0.10.9.5|
|py4j|0.10.9.7|
|pyarrow|9.0.0|
|pyasn1|0.4.8|
|pyasn1-modules|0.2.7|
|pycosat|0.6.4|
|pycparser|2.21|
|pygments|2.17.2|
|pygments|2.13.0|
|pyjwt|2.6.0|
|pynacl|1.5.0|
|pyodbc|4.0.34|
|pyopenssl|22.1.0|
|pyparsing|3.0.9|
|pyparsing|3.1.2|
|pyperclip|1.8.2|
|pyqt|5.9.2|
|pyrsistent|0.19.2|
|pysocks|1.7.1|
|pyspark|3.5.1|
|pyspark|3.3.1|
|python|3.10.14|
|python|3.10.6|
|python-dateutil|2.8.2|
|python-dateutil|2.9.0.post0|
|python-flatbuffers|2.0|
|python_abi|3.10|
|pytorch|1.13.0|
|pytorch-mutex|1.0|
|pytz|2022.6|
|pytz|2024.1|
|pyu2f|0.1.5|
|pywavelets|1.3.0|
|pyyaml|6.0|
|pyzmq|24.0.1|
|**pyzmq**|**24.0.1 --> 26.0.0**|
|qt|5.9.7|
|re2|2022.06.01|
|readline|8.1.2|
|readline|8.2|
|regex|2022.10.31|
|requests|2.28.1|
|requests-oauthlib|1.3.1|
|retrying|1.3.3|
|rsa|4.9|
|ruamel-yaml|0.17.4|
|ruamel-yaml-clib|0.2.6|
|ruamel_yaml|0.15.80|
|s2n|1.0.10|
|salib|1.4.6.1|
|scikit-image|0.19.3|
|scikit-learn|1.1.3|
|scipy|1.9.3|
|seaborn|0.11.1|
|seaborn-base|0.11.1|
|secretstorage|3.3.3|
|send2trash|1.8.0|
|setuptools|65.5.1|
|**setuptools**|**65.5.1 --> 69.5.1**|
|shap|0.39.0|
|sip|4.19.13|
|six|1.16.0|
|skl2onnx|1.8.0.1|
|sklearn-pandas|2.2.0|
|slicer|0.0.7|
|smart_open|6.2.0|
|smmap|3.0.5|
|snappy|1.1.9|
|sniffio|1.3.0|
|soupsieve|2.3.2.post1|
|sqlalchemy|1.4.43|
|sqlanalyticsconnectorpy|1.0.1|
|sqlite|3.39.4|
|sqlparse|0.4.3|
|stack-data|0.6.3|
|stack_data|0.6.0|
|statsmodels|0.13.5|
|sympy|1.11.1|
|synapseml-cognitive|1.0.2.dev1|
|synapseml-core|1.0.2.dev1|
|synapseml-deep-learning|1.0.2.dev1|
|synapseml-internal|1.0.2.1.dev1|
|synapseml-lightgbm|1.0.2.dev1|
|synapseml-opencv|1.0.2.dev1|
|synapseml-vw|1.0.2.dev1|
|tabulate|0.9.0|
|tbb|2021.6.0|
|tensorboard|2.8.0|
|tensorboard-data-server|0.6.0|
|tensorboard-plugin-wit|1.8.1|
|tensorflow|2.8.0|
|tensorflow-base|2.10.0|
|tensorflow-estimator|2.8.0|
|tensorflow-io-gcs-filesystem|0.27.0|
|termcolor|2.1.0|
|terminado|0.17.0|
|textblob|0.15.3|
|tf-estimator-nightly|2.8.0.dev2021122109|
|threadpoolctl|3.1.0|
|tifffile|2022.10.10|
|tinycss2|1.2.1|
|tk|8.6.12|
|tk|8.6.13|
|toolz|0.12.0|
|torchvision|0.14.0|
|tornado|6.2|
|tornado|6.4|
|tqdm|4.64.1|
|traitlets|5.5.0|
|traitlets|5.14.2|
|typed-ast|1.4.3|
|**typing-extensions**|**4.10.0 --> 4.11.0**|
|typing-extensions|4.4.0|
|typing_extensions|4.4.0|
|tzdata|2022f|
|tzdata|2024.1|
|unicodedata2|15.0.0|
|unixodbc|2.3.10|
|urllib3|1.26.4|
|virtualenv|20.14.0|
|wcwidth|0.2.13|
|wcwidth|0.2.5|
|webencodings|0.5.1|
|websocket-client|1.4.2|
|werkzeug|2.2.2|
|wheel|0.43.0|
|wheel|0.38.3|
|widgetsnbextension|4.0.10|
|widgetsnbextension|3.6.1|
|wrapt|1.14.1|
|xgboost|1.7.1|
|xorg-libxau|1.0.9|
|xorg-libxdmcp|1.1.3|
|xyzservices|2022.9.0|
|xz|5.2.6|
|yaml|0.2.5|
|yarl|1.8.1|
|zeromq|4.3.4|
|zfp|1.0.0|
|zipp|3.10.0|
|zlib|1.2.13|
|zlib-ng|2.0.6|
|zope.event|4.5.0|
|zope.interface|5.5.1|
|zstd|1.5.2|

### Environment: Fabric

|Name|Version|
|-----|-----|
|_openmp_mutex|4.5|
|_py-xgboost-mutex|2.0|
|absl-py|1.4.0|
|adal|1.2.7|
|adlfs|2023.1.0|
|aiohttp|3.8.4|
|aiosignal|1.3.1|
|alsa-lib|1.2.8|
|anyio|3.6.2|
|argcomplete|2.1.2|
|argon2-cffi|21.3.0|
|argon2-cffi-bindings|21.2.0|
|arrow-cpp|11.0.0|
|asttokens|2.2.1|
|astunparse|1.6.3|
|async-timeout|4.0.2|
|atk-1.0|2.38.0|
|attr|2.5.1|
|attrs|22.2.0|
|aws-c-auth|0.6.24|
|aws-c-cal|0.5.20|
|aws-c-common|0.8.11|
|aws-c-compression|0.2.16|
|aws-c-event-stream|0.2.18|
|aws-c-http|0.7.4|
|aws-c-io|0.13.17|
|aws-c-mqtt|0.8.6|
|aws-c-s3|0.2.4|
|aws-c-sdkutils|0.1.7|
|aws-checksums|0.1.14|
|aws-crt-cpp|0.19.7|
|aws-sdk-cpp|1.10.57|
|azure-common|1.1.28|
|azure-core|1.26.4|
|azure-datalake-store|0.0.51|
|azure-graphrbac|0.61.1|
|azure-identity|1.12.0|
|azure-mgmt-authorization|3.0.0|
|azure-mgmt-containerregistry|10.1.0|
|azure-mgmt-core|1.4.0|
|azure-mgmt-keyvault|10.2.1|
|azure-mgmt-resource|21.2.1|
|azure-mgmt-storage|20.1.0|
|azure-storage-blob|12.15.0|
|azure-storage-file-datalake|12.9.1|
|azure-synapse-ml-predict|1.0.0|
|azureml-core|1.49.0|
|azureml-synapse|0.0.1|
|backcall|0.2.0|
|backports|1.0|
|backports-tempfile|1.0|
|backports-weakref|1.0.post1|
|backports.functools_lru_cache|1.6.4|
|bcrypt|3.2.2|
|beautifulsoup4|4.11.2|
|bleach|6.0.0|
|blinker|1.6.1|
|brotli|1.0.9|
|brotli-bin|1.0.9|
|brotli-python|1.0.9|
|brotlipy|0.7.0|
|bzip2|1.0.8|
|c-ares|1.18.1|
|ca-certificates|2022.12.7|
|cached-property|1.5.2|
|cached_property|1.5.2|
|cachetools|5.3.0|
|cairo|1.16.0|
|certifi|2022.12.7|
|cffi|1.15.1|
|charset-normalizer|2.1.1|
|click|8.1.3|
|cloudpickle|2.2.1|
|colorama|0.4.6|
|comm|0.1.3|
|conda-package-handling|2.0.2|
|conda-package-streaming|0.7.0|
|configparser|5.3.0|
|contextlib2|21.6.0|
|contourpy|1.0.7|
|cryptography|40.0.1|
|cycler|0.11.0|
|dash|2.9.2|
|dash-core-components|2.0.0|
|dash-html-components|2.0.0|
|dash-table|5.0.0|
|dash_cytoscape|0.2.0|
|databricks-cli|0.17.6|
|dbus|1.13.6|
|debugpy|1.6.7|
|decorator|5.1.1|
|defusedxml|0.7.1|
|dill|0.3.6|
|distlib|0.3.6|
|docker-py|6.0.0|
|entrypoints|0.4|
|et_xmlfile|1.1.0|
|executing|1.2.0|
|expat|2.5.0|
|fftw|3.3.10|
|filelock|3.11.0|
|flask|2.2.3|
|flask-compress|1.13|
|flatbuffers|22.12.06|
|flit-core|3.8.0|
|fluent-logger|0.10.0|
|font-ttf-dejavu-sans-mono|2.37|
|font-ttf-inconsolata|3.000|
|font-ttf-source-code-pro|2.038|
|font-ttf-ubuntu|0.83|
|fontconfig|2.14.2|
|fonts-conda-ecosystem|1|
|fonts-conda-forge|1|
|fonttools|4.39.3|
|freetype|2.12.1|
|fribidi|1.0.10|
|frozenlist|1.3.3|
|fsspec|2023.4.0|
|fsspec_wrapper|0.1.9|
|gast|0.4.0|
|gdk-pixbuf|2.42.10|
|geographiclib|1.52|
|geopy|2.3.0|
|gettext|0.21.1|
|gevent|22.10.2|
|gflags|2.2.2|
|giflib|5.2.1|
|gitdb|4.0.10|
|gitpython|3.1.31|
|glib|2.74.1|
|glib-tools|2.74.1|
|glog|0.6.0|
|google-auth|2.17.2|
|google-auth-oauthlib|0.4.6|
|google-pasta|0.2.0|
|graphite2|1.3.13|
|graphviz|2.50.0|
|greenlet|2.0.2|
|grpcio|1.51.1|
|gson|0.0.3|
|gst-plugins-base|1.22.0|
|gstreamer|1.22.0|
|gstreamer-orc|0.4.33|
|gtk2|2.24.33|
|gts|0.7.6|
|h5py|3.8.0|
|harfbuzz|6.0.0|
|hdf5|1.14.0|
|html5lib|1.1|
|humanfriendly|10.0|
|icu|70.1|
|idna|3.4|
|imageio|2.25.0|
|importlib-metadata|5.2.0|
|importlib_metadata|5.2.0|
|importlib_resources|5.12.0|
|impulse-python-handler|1.0.19.1.0.0|
|interpret|0.3.1|
|interpret-core|0.3.1|
|ipykernel|6.22.0|
|ipython|8.9.0|
|ipywidgets|8.0.4|
|isodate|0.6.1|
|itsdangerous|2.1.2|
|jack|1.9.22|
|jedi|0.18.2|
|jeepney|0.8.0|
|jinja2|3.1.2|
|jmespath|1.0.1|
|joblib|1.2.0|
|jpeg|9e|
|jsonpickle|2.2.0|
|jsonschema|4.17.3|
|jupyter_client|8.1.0|
|jupyter_core|5.3.0|
|jupyter_events|0.6.3|
|jupyter_server|2.2.1|
|jupyter_server_terminals|0.4.4|
|jupyterlab_pygments|0.2.2|
|jupyterlab_widgets|3.0.7|
|keras|2.11.0|
|keras-preprocessing|1.1.2|
|keyutils|1.6.1|
|kiwisolver|1.4.4|
|knack|0.10.1|
|krb5|1.20.1|
|lame|3.100|
|lcms2|2.15|
|ld_impl_linux-64|2.40|
|lerc|4.0.0|
|liac-arff|2.5.0|
|libabseil|20220623.0|
|libaec|1.0.6|
|libarrow|11.0.0|
|libblas|3.9.0|
|libbrotlicommon|1.0.9|
|libbrotlidec|1.0.9|
|libbrotlienc|1.0.9|
|libcap|2.67|
|libcblas|3.9.0|
|libclang|15.0.7|
|libclang13|15.0.7|
|libcrc32c|1.1.2|
|libcups|2.3.3|
|libcurl|7.88.1|
|libdb|6.2.32|
|libdeflate|1.17|
|libebm|0.3.1|
|libedit|3.1.20191231|
|libev|4.33|
|libevent|2.1.10|
|libexpat|2.5.0|
|libffi|3.4.2|
|libflac|1.4.2|
|libgcc-ng|12.2.0|
|libgcrypt|1.10.1|
|libgd|2.3.3|
|libgfortran-ng|12.2.0|
|libgfortran5|12.2.0|
|libglib|2.74.1|
|libgoogle-cloud|2.7.0|
|libgpg-error|1.46|
|libgrpc|1.51.1|
|libhwloc|2.9.0|
|libiconv|1.17|
|liblapack|3.9.0|
|libllvm11|11.1.0|
|libllvm15|15.0.7|
|libnghttp2|1.52.0|
|libnsl|2.0.0|
|libogg|1.3.4|
|libopenblas|0.3.21|
|libopus|1.3.1|
|libpng|1.6.39|
|libpq|15.2|
|libprotobuf|3.21.12|
|library-metadata-cooker|0.0.7|
|librsvg|2.54.4|
|libsndfile|1.2.0|
|libsodium|1.0.18|
|libsqlite|3.40.0|
|libssh2|1.10.0|
|libstdcxx-ng|12.2.0|
|libsystemd0|253|
|libthrift|0.18.0|
|libtiff|4.5.0|
|libtool|2.4.7|
|libudev1|253|
|libutf8proc|2.8.0|
|libuuid|2.38.1|
|libuv|1.44.2|
|libvorbis|1.3.7|
|libwebp|1.2.4|
|libwebp-base|1.2.4|
|libxcb|1.13|
|libxgboost|1.7.1|
|libxkbcommon|1.5.0|
|libxml2|2.10.3|
|libxslt|1.1.37|
|libzlib|1.2.13|
|lightgbm|3.3.3|
|lime|0.2.0.1|
|llvm-openmp|16.0.1|
|llvmlite|0.39.1|
|lxml|4.9.2|
|lz4-c|1.9.4|
|markdown|3.4.1|
|markupsafe|2.1.2|
|matplotlib|3.6.3|
|matplotlib-base|3.6.3|
|matplotlib-inline|0.1.6|
|mistune|2.0.5|
|mkl|2022.2.1|
|mlflow-skinny|2.1.1|
|mpg123|1.31.3|
|msal|1.21.0|
|msal_extensions|1.0.0|
|msgpack|1.0.5|
|msrest|0.7.1|
|msrestazure|0.6.4|
|multidict|6.0.4|
|multiprocess|0.70.14|
|munkres|1.1.4|
|mypy|0.780|
|mypy-extensions|0.4.4|
|mysql-common|8.0.32|
|mysql-libs|8.0.32|
|nbclient|0.7.3|
|nbconvert-core|7.3.0|
|nbformat|5.8.0|
|ncurses|6.3|
|ndg-httpsclient|0.5.1|
|nest-asyncio|1.5.6|
|notebookutils|3.3.0-20240213.4|
|nspr|4.35|
|nss|3.89|
|numba|0.56.4|
|numpy|1.23.5|
|oauthlib|3.2.2|
|openjpeg|2.5.0|
|openpyxl|3.1.0|
|openssl|3.1.0|
|opt_einsum|3.3.0|
|orc|1.8.2|
|packaging|21.3|
|pandas|1.5.3|
|pandasql|0.7.3|
|pandocfilters|1.5.0|
|pango|1.50.14|
|paramiko|2.12.0|
|parquet-cpp|1.5.1|
|parso|0.8.3|
|pathos|0.3.0|
|pathspec|0.11.1|
|patsy|0.5.3|
|pcre2|10.40|
|pexpect|4.8.0|
|pickleshare|0.7.5|
|pillow|9.4.0|
|pip|23.0.1|
|pixman|0.40.0|
|pkginfo|1.9.6|
|pkgutil-resolve-name|1.3.10|
|platformdirs|3.2.0|
|plotly|5.13.0|
|ply|3.11|
|pooch|1.7.0|
|portalocker|2.7.0|
|pox|0.3.2|
|ppft|1.7.6.6|
|prettytable|3.6.0|
|prometheus_client|0.16.0|
|prompt-toolkit|3.0.38|
|protobuf|4.21.12|
|psutil|5.9.4|
|pthread-stubs|0.4|
|ptyprocess|0.7.0|
|pulseaudio|16.1|
|pulseaudio-client|16.1|
|pulseaudio-daemon|16.1|
|pure_eval|0.2.2|
|py-xgboost|1.7.1|
|py4j|0.10.9.5|
|pyarrow|11.0.0|
|pyasn1|0.4.8|
|pyasn1-modules|0.2.7|
|pycosat|0.6.4|
|pycparser|2.21|
|pygments|2.14.0|
|pyjwt|2.6.0|
|pynacl|1.5.0|
|pyodbc|4.0.35|
|pyopenssl|23.1.1|
|pyparsing|3.0.9|
|pyperclip|1.8.2|
|pyqt|5.15.7|
|pyqt5-sip|12.11.0|
|pyrsistent|0.19.3|
|pysocks|1.7.1|
|pyspark|3.3.1|
|python|3.10.10|
|python-dateutil|2.8.2|
|python-fastjsonschema|2.16.3|
|python-flatbuffers|23.1.21|
|python-graphviz|0.20.1|
|python-json-logger|2.0.7|
|python_abi|3.10|
|pytorch|1.13.1|
|pytz|2022.7.1|
|pyu2f|0.1.5|
|pywin32-on-windows|0.1.0|
|pyyaml|6.0|
|pyzmq|25.0.2|
|qt-main|5.15.8|
|re2|2023.02.01|
|readline|8.2|
|regex|2022.10.31|
|requests|2.28.2|
|requests-oauthlib|1.3.1|
|rfc3339-validator|0.1.4|
|rfc3986-validator|0.1.1|
|rsa|4.9|
|ruamel.yaml|0.17.21|
|ruamel.yaml.clib|0.2.7|
|ruamel_yaml|0.15.80|
|s2n|1.3.37|
|salib|1.4.7|
|scikit-learn|1.2.0|
|scipy|1.10.1|
|seaborn|0.12.2|
|seaborn-base|0.12.2|
|secretstorage|3.3.3|
|send2trash|1.8.0|
|setuptools|67.6.1|
|shap|0.41.0|
|sip|6.7.7|
|six|1.16.0|
|sleef|3.5.1|
|slicer|0.0.7|
|smmap|3.0.5|
|snappy|1.1.10|
|sniffio|1.3.0|
|soupsieve|2.3.2.post1|
|sqlalchemy|2.0.9|
|sqlanalyticsconnectorpy|1.0.1|
|sqlparse|0.4.3|
|stack_data|0.6.2|
|statsmodels|0.13.5|
|synapseml-cognitive|1.0.2.dev1|
|synapseml-core|1.0.2.dev1|
|synapseml-deep-learning|1.0.2.dev1|
|synapseml-internal|1.0.2.1.dev1|
|synapseml-lightgbm|1.0.2.dev1|
|synapseml-mlflow|1.0.23|
|synapseml-opencv|1.0.2.dev1|
|synapseml-utils|1.0.19.post1|
|synapseml-vw|1.0.2.dev1|
|tabulate|0.9.0|
|tbb|2021.8.0|
|tenacity|8.2.2|
|tensorboard|2.11.2|
|tensorboard-data-server|0.6.1|
|tensorboard-plugin-wit|1.8.1|
|tensorflow|2.11.0|
|tensorflow-base|2.11.0|
|tensorflow-estimator|2.11.0|
|termcolor|2.2.0|
|terminado|0.17.1|
|threadpoolctl|3.1.0|
|tinycss2|1.2.1|
|tk|8.6.12|
|toml|0.10.2|
|toolz|0.12.0|
|tornado|6.2|
|tqdm|4.65.0|
|traitlets|5.9.0|
|treeinterpreter|0.2.2|
|typed-ast|1.4.3|
|typing-extensions|4.5.0|
|typing_extensions|4.5.0|
|tzdata|2023c|
|unicodedata2|15.0.0|
|unixodbc|2.3.10|
|urllib3|1.26.14|
|virtualenv|20.19.0|
|wcwidth|0.2.6|
|webencodings|0.5.1|
|websocket-client|1.5.1|
|werkzeug|2.2.3|
|wheel|0.40.0|
|widgetsnbextension|4.0.7|
|wrapt|1.15.0|
|xcb-util|0.4.0|
|xcb-util-image|0.4.0|
|xcb-util-keysyms|0.4.0|
|xcb-util-renderutil|0.3.9|
|xcb-util-wm|0.4.1|
|xgboost|1.7.1|
|xkeyboard-config|2.38|
|xorg-kbproto|1.0.7|
|xorg-libice|1.0.10|
|xorg-libsm|1.2.3|
|xorg-libx11|1.8.4|
|xorg-libxau|1.0.9|
|xorg-libxdmcp|1.1.3|
|xorg-libxext|1.3.4|
|xorg-libxrender|0.9.10|
|xorg-renderproto|0.11.1|
|xorg-xextproto|7.3.0|
|xorg-xproto|7.0.31|
|xz|5.2.6|
|yaml|0.2.5|
|yarl|1.8.2|
|zeromq|4.3.4|
|zipp|3.15.0|
|zlib|1.2.13|
|zope.event|4.6|
|zope.interface|6.0|
|zstandard|0.19.0|
|zstd|1.5.2|
|_libgcc_mutex|0.1|

# Java and Scala Libraries

|Name|Version|
|-----|-----|
|HikariCP|2.5.1|
|JLargeArrays|1.5|
|JTransforms|3.1|
|RoaringBitmap|0.9.25|
|ST4|4.0.4|
|SparkCustomEvents|3.3.0-1.0.2|
|**TokenLibrary-assembly**|**3.5.8 --> 3.6.4**|
|**VegasConnector**|**3.3.08 --> 3.3.09**|
|activation|1.1.1|
|aircompressor|0.21|
|algebra|2.12-2.0.1|
|aliyun-java-sdk-core|4.5.10|
|aliyun-java-sdk-kms|2.11.0|
|aliyun-java-sdk-ram|3.1.0|
|aliyun-sdk-oss|3.13.0|
|annotations|7.0.0|
|antlr-runtime|3.5.2|
|antlr4-runtime|4.8|
|aopalliance-repackaged|2.6.1|
|apiguardian-api|1.1.0|
|arpack|2.2.1|
|arpack_combined_all|0.1|
|arrow-format|7.0.0|
|arrow-memory-core|7.0.0|
|arrow-memory-netty|7.0.0|
|arrow-vector|7.0.0|
|audience-annotations|0.5.0|
|autotune-client|2.12-1.11.0-3.3-120040110|
|autotune-common|2.12-1.11.0-3.3-120040110|
|avro|1.11.0|
|avro-ipc|1.11.0|
|avro-mapred|1.11.0|
|aws-java-sdk-bundle|1.11.1026|
|azure-data-lake-store-sdk|2.3.9|
|azure-eventhubs|3.3.0|
|azure-eventhubs-spark|2.12-2.3.22|
|azure-keyvault-core|1.0.0|
|azure-storage|7.0.1|
|azure-synapse-ml-pandas|2.12-0.1.1|
|azure-synapse-ml-predict|2.12-1.0|
|blas|2.2.1|
|bonecp|0.8.0.RELEASE|
|breeze|2.12-1.2|
|breeze-macros|2.12-1.2|
|cats-kernel|2.12-2.1.1|
|chill|2.12-0.10.0|
|chill-java|0.10.0|
|client-sdk|1.24.1|
|commons-cli|1.5.0|
|commons-codec|1.15|
|commons-collections|3.2.2|
|commons-collections4|4.4|
|commons-compiler|3.0.16|
|commons-compress|1.21|
|commons-crypto|1.1.0|
|commons-dbcp|1.4|
|commons-io|2.11.0|
|commons-lang|2.6|
|commons-lang3|3.12.0|
|commons-logging|1.1.3|
|commons-math3|3.6.1|
|commons-pool|1.5.4|
|commons-pool2|2.11.1|
|commons-text|1.10.0|
|compress-lzf|1.1|
|config|1.3.4|
|core|1.1.2|
|cos_api-bundle|5.6.19|
|cosmos-analytics-spark|3.3.1-connector-1.8.10|
|curator-client|2.13.0|
|curator-framework|2.13.0|
|curator-recipes|2.13.0|
|datanucleus-api-jdo|4.2.4|
|datanucleus-core|4.1.17|
|datanucleus-rdbms|4.1.19|
|delta-core|2.12-2.2.0.11|
|delta-iceberg|2.12-2.2.0.11|
|delta-storage|2.2.0.11|
|derby|0.14.2.0|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|
|flatbuffers-java|1.12.0|
|fluent-logger-jar-with-dependencies-jdk8|8|
|genesis-client|2.12-0.27.0-jar-with-dependencies|
|gluten-velox-bundle-spark|3.3_2.12-ubuntu_18.04-0.5.0-SNAPSHOT|
|**gson**|**2.8.6 --> 2.8.9**|
|guava|4.0.1|
|**hadoop-aliyun**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-annotations**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-aws**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-azure**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-azure-datalake**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|hadoop-azureml|1.0-fs|
|**hadoop-client-api**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-client-runtime**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-cloud-storage**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-cos**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|**hadoop-openstack**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|hadoop-shaded-guava|1.1.1|
|**hadoop-yarn-server-web-proxy**|**3.3.3.5.2-119960880 --> 3.3.3.5.2-122281848**|
|hdinsight-spark-metrics|3.3.0-1.0.2|
|hive-beeline|2.3.9|
|hive-cli|2.3.9|
|hive-common|2.3.9|
|hive-exec|2.3.9-core|
|hive-jdbc|2.3.9|
|hive-llap-common|2.3.9|
|hive-metastore|2.3.9|
|hive-serde|2.3.9|
|hive-service-rpc|3.1.2|
|hive-shims|0.23-2.3.9|
|hive-shims|2.3.9|
|hive-shims-common|2.3.9|
|hive-shims-scheduler|2.3.9|
|hive-storage-api|2.7.2|
|hive-vector-code-gen|2.3.9|
|hk2-api|2.6.1|
|hk2-locator|2.6.1|
|hk2-utils|2.6.1|
|httpclient|4.5.13|
|httpclient5|5.1.3|
|httpcore|4.4.14|
|httpmime|4.5.13|
|impulse-core_spark|3.3_2.12-1.0.19|
|impulse-telemetry-mds_spark|3.3_2.12-1.0.19|
|ini4j|0.5.4|
|isolation-forest|3.3.3_2.12-3.0.3|
|istack-commons-runtime|3.0.8|
|ivy|2.5.1|
|jackson-annotations|2.13.4|
|jackson-core|2.13.4|
|jackson-core-asl|1.9.13|
|**jackson-databind**|**2.13.4.1 --> 2.13.4.2**|
|jackson-dataformat-cbor|2.13.4|
|jackson-mapper-asl|1.9.13|
|jackson-module-scala|2.12-2.13.4|
|jakarta.annotation-api|1.3.5|
|jakarta.inject|2.6.1|
|jakarta.servlet-api|4.0.3|
|jakarta.validation-api|2.0.2|
|jakarta.ws.rs-api|2.1.6|
|jakarta.xml.bind-api|2.3.2|
|janino|3.0.16|
|javassist|3.25.0-GA|
|javatuples|1.2|
|javax.jdo|3.2.0-m3|
|javolution|5.5.1|
|jaxb-api|2.2.11|
|jaxb-runtime|2.3.2|
|jcl-over-slf4j|1.7.32|
|jdo-api|3.0.1|
|jdom2|2.0.6|
|jersey-client|2.36|
|jersey-common|2.36|
|jersey-container-servlet|2.36|
|jersey-container-servlet-core|2.36|
|jersey-hk2|2.36|
|jersey-server|2.36|
|jettison|1.1|
|**jetty-util**|**9.4.48.v20220622 --> 9.4.53.v20231009**|
|**jetty-util-ajax**|**9.4.48.v20220622 --> 9.4.53.v20231009**|
|jline|2.14.6|
|joda-time|2.10.13|
|jodd-core|3.5.2|
|jpam|1.1|
|jsch|0.1.54|
|**json**|**1 --> 3**|
|json|1.8|
|json|1|
|json-simple|1.1|
|json-simple|1.1.1|
|json4s-ast|2.12-3.7.0-M11|
|json4s-core|2.12-3.7.0-M11|
|json4s-jackson|2.12-3.7.0-M11|
|json4s-scalap|2.12-3.7.0-M11|
|jsr305|3.0.0|
|jta|1.1|
|jul-to-slf4j|1.7.32|
|junit-jupiter|5.5.2|
|junit-jupiter-api|5.5.2|
|junit-jupiter-engine|5.5.2|
|junit-jupiter-params|5.5.2|
|junit-platform-commons|1.5.2|
|junit-platform-engine|1.5.2|
|kafka-clients|2.8.1|
|kryo-shaded|4.0.2|
|kusto-data|3.2.1-SynapseFabric|
|kusto-ingest|3.2.1-SynapseFabric|
|kusto-spark|3.0_2.12-3.1.16|
|lapack|2.2.1|
|leveldbjni-all|1.8|
|libfb303|0.9.3|
|libthrift|0.12.0|
|lightgbmlib|3.3.510|
|log4j|1.2-api-2.17.2|
|log4j-api|2.17.2|
|log4j-core|2.17.2|
|log4j-slf4j-impl|2.17.2|
|lz4-java|1.8.0|
|mdsdclientdynamic|2.0|
|metrics-core|4.2.7|
|metrics-graphite|4.2.7|
|metrics-jmx|4.2.7|
|metrics-json|4.2.7|
|metrics-jvm|4.2.7|
|microsoft-catalog-metastore-client|1.1.17|
|microsoft-log4j-etwappender|1.0|
|minlog|1.3.0|
|mlflow-spark|2.1.1|
|mssql-jdbc|8.4.1.jre8|
|mysql-connector-java|8.0.18|
|netty-all|4.1.74.Final|
|netty-buffer|4.1.74.Final|
|netty-codec|4.1.74.Final|
|netty-common|4.1.74.Final|
|netty-handler|4.1.74.Final|
|netty-resolver|4.1.74.Final|
|netty-tcnative-classes|2.0.48.Final|
|netty-transport|4.1.74.Final|
|netty-transport-classes-epoll|4.1.74.Final|
|netty-transport-classes-kqueue|4.1.74.Final|
|netty-transport-native-epoll|4.1.74.Final-linux-x86_64|
|netty-transport-native-epoll|4.1.74.Final-linux-aarch_64|
|netty-transport-native-kqueue|4.1.74.Final-osx-x86_64|
|netty-transport-native-kqueue|4.1.74.Final-osx-aarch_64|
|netty-transport-native-unix-common|4.1.74.Final|
|notebook-utils|3.3.0-20240213.4|
|objenesis|3.2|
|onnx-protobuf|2.12-0.9.3|
|onnxruntime_gpu|1.8.1|
|opencsv|2.3|
|opencv|3.2.0-1|
|opentest4j|1.2.0|
|opentracing-api|0.33.0|
|opentracing-noop|0.33.0|
|opentracing-util|0.33.0|
|orc-core|1.7.6|
|orc-mapreduce|1.7.6|
|orc-shims|1.7.6|
|oro|2.0.8|
|osgi-resource-locator|1.0.3|
|paranamer|2.8|
|parquet-column|1.12.3|
|parquet-common|1.12.3|
|parquet-encoding|1.12.3|
|parquet-format-structures|1.12.3|
|parquet-hadoop|1.12.3|
|parquet-jackson|1.12.3|
|peregrine-spark|3.3.0-0.10.3|
|pickle|1.2|
|postgresql|2.2.9|
|protobuf-java|2.5.0|
|proton-j|0.33.8|
|py4j|0.10.9.5|
|qpid-proton-j-extensions|1.2.4|
|resilience4j-core|1.7.1|
|resilience4j-retry|1.7.1|
|rocksdbjni|6.20.3|
|scala-collection-compat|2.12-2.1.1|
|scala-compiler|2.12.15|
|scala-java8-compat|2.12-0.9.0|
|scala-library|2.12.15|
|scala-parser-combinators|2.12-1.1.2|
|scala-reflect|2.12.15|
|scala-xml|2.12-1.2.0|
|scalactic|2.12-3.2.14|
|shapeless|2.12-2.3.7|
|shims|0.9.25|
|slf4j-api|1.7.32|
|**snappy-java**|**1.1.8.4 --> 1.1.10.5**|
|spark|3.3-rpc-history-server-core_2.12-1.0.0|
|spark|3.3-advisor-core_2.12-1.0.18|
|spark|3.3-rpc-history-server-app-listener_2.12-1.0.0|
|**spark-avro**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-catalyst**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-cdm-connector-assembly-spark**|**3.3-1.19.7 --> 3.3-1.19.5**|
|**spark-core**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-enhancement**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|spark-enhancementui|2.12-3.0.0|
|**spark-graphx**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-hadoop-cloud**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-hive**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-hive-thriftserver**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|spark-kusto-synapse-connector|3.1_2.12-1.3.4|
|**spark-kvstore**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-launcher**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|spark-lighter-contract|2.12-2.0.7_spark-3.3.0|
|spark-lighter-core|2.12-2.0.7_spark-3.3.0|
|**spark-microsoft-tools**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-mllib**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-mllib-local**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-network-common**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-network-shuffle**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-repl**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-sketch**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-sql**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-sql-kafka**|**0_2.12-3.3.1.5.2-119960880 --> 0_2.12-3.3.1.5.2-122281848**|
|**spark-streaming**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-streaming-kafka**|**0_2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-streaming-kafka**|**0_2.12-3.3.1.5.2-119960880 --> 0_2.12-3.3.1.5.2-122281848**|
|**spark-tags**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-token-provider-kafka**|**0_2.12-3.3.1.5.2-119960880 --> 0_2.12-3.3.1.5.2-122281848**|
|**spark-unsafe**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|**spark-yarn**|**2.12-3.3.1.5.2-119960880 --> 2.12-3.3.1.5.2-122281848**|
|spark_diagnostic_cli|2.1.0_spark-3.3.0|
|sparklyr-connector|1.0.0_spark-3.3.1|
|sparknativeparquetwriter|2.12-0.8.1-spark-3.3|
|spire|2.12-0.17.0|
|spire-macros|2.12-0.17.0|
|spire-platform|2.12-0.17.0|
|spire-util|2.12-0.17.0|
|spray-json|2.12-1.3.5|
|**sqlanalyticsconnector**|**3.3.0-2.1.2 --> 3.3.0-2.1.3**|
|stax-api|1.0.1|
|stream|2.9.6|
|structuredstreamforspark|2.12-3.2.0-2.3.0|
|super-csv|2.2.0|
|synapseml|2.12-1.0.2-spark3.3|
|synapseml-cognitive|2.12-1.0.2-spark3.3|
|synapseml-core|2.12-1.0.2-spark3.3|
|synapseml-deep-learning|2.12-1.0.2-spark3.3|
|synapseml-internal|2.12-1.0.2.1-spark3.3|
|synapseml-lightgbm|2.12-1.0.2-spark3.3|
|synapseml-opencv|2.12-1.0.2-spark3.3|
|synapseml-vw|2.12-1.0.2-spark3.3|
|synfs|3.3.0-20240213.4|
|threeten-extra|1.5.0|
|tink|1.6.1|
|transaction-api|1.1|
|trident-core|1.2.6|
|**tridentsystemtokenlibrary-assembly**|**1.6.2 --> 1.6.5**|
|**tridenttokenlibrary-assembly**|**1.6.2 --> 1.6.5**|
|univocity-parsers|2.9.1|
|vavr|0.10.4|
|vavr-match|0.10.4|
|velocity|1.5|
|vw-jni|9.3.0|
|wildfly-openssl|1.0.7.Final|
|xbean-asm9-shaded|4.20|
|xz|1.8|
|**zookeeper**|**3.6.2.5.2-119960880 --> 3.6.2.5.2-122281848**|
|**zookeeper-jute**|**3.6.2.5.2-119960880 --> 3.6.2.5.2-122281848**|
|zstd-jni|1.5.2-1|

# R Libraries

|Name|Version|
|-----|-----|
|DBI|1.2.1|
|DiceDesign|1.10|
|FabricTelemetry|1.0.2|
|GPfit|1.0-8|
|KernSmooth|2.23-22|
|MASS|7.3-60.0.1|
|Matrix|1.6-5|
|ModelMetrics|1.2.2.2|
|R.methodsS3|1.8.2|
|R.oo|1.26.0|
|R.utils|2.12.3|
|R6|2.5.1|
|R6P|0.3.0|
|RColorBrewer|1.1-3|
|RODBC|1.3-20|
|Rcpp|1.0.12|
|SQUAREM|2021.1|
|TTR|0.24.4|
|V8|4.4.1|
|XML|3.99-0.16.1|
|arrow|10.0.1|
|askpass|1.2.0|
|assertthat|0.2.1|
|backports|1.4.1|
|base|4.2.3|
|base64enc|0.1-3|
|bigD|0.2.0|
|bit|4.0.5|
|bit64|4.0.5|
|bitops|1.0-7|
|blob|1.2.4|
|brew|1.0-10|
|brio|1.1.4|
|broom|1.0.5|
|bslib|0.6.1|
|cachem|1.0.8|
|callr|3.7.3|
|caret|6.0-93|
|cellranger|1.1.0|
|class|7.3-22|
|cli|3.6.2|
|clipr|0.8.0|
|clock|0.7.0|
|codetools|0.2-19|
|collections|0.3.7|
|colorspace|2.1-0|
|commonmark|1.9.1|
|compiler|4.2.3|
|config|0.3.2|
|conflicted|1.2.0|
|coro|1.0.3|
|cpp11|0.4.7|
|crayon|1.5.2|
|credentials|2.0.1|
|crosstalk|1.2.1|
|crul|1.4.0|
|curl|5.1.0|
|data.table|1.14.10|
|datasets|4.2.3|
|dbplyr|2.3.4|
|desc|1.4.3|
|devtools|2.4.5|
|diagram|1.6.5|
|dials|1.2.0|
|diffobj|0.3.5|
|digest|0.6.34|
|downlit|0.4.3|
|dplyr|1.1.4|
|dtplyr|1.3.1|
|e1071|1.7-14|
|ellipsis|0.3.2|
|evaluate|0.23|
|fansi|1.0.6|
|farver|2.1.1|
|fastmap|1.1.1|
|fontawesome|0.5.2|
|forcats|1.0.0|
|foreach|1.5.2|
|forge|0.2.0|
|fs|1.6.3|
|furrr|0.3.1|
|future|1.33.1|
|future.apply|1.11.1|
|gargle|1.5.2|
|generics|0.1.3|
|gert|2.0.1|
|ggplot2|3.4.0|
|gh|1.4.0|
|gistr|0.9.0|
|gitcreds|0.1.2|
|globals|0.16.2|
|glue|1.7.0|
|googledrive|2.1.1|
|googlesheets4|1.1.1|
|gower|1.0.1|
|grDevices|4.2.3|
|graphics|4.2.3|
|grid|4.2.3|
|gt|0.9.0|
|gtable|0.3.4|
|hardhat|1.3.0|
|haven|2.5.4|
|hexbin|1.28.3|
|highcharter|0.9.4|
|highr|0.10|
|hms|1.1.3|
|htmltools|0.5.7|
|htmlwidgets|1.6.4|
|httpcode|0.3.0|
|httpuv|1.6.14|
|httr|1.4.7|
|httr2|1.0.0|
|ids|1.0.1|
|igraph|1.5.1|
|infer|1.0.6|
|ini|0.3.1|
|ipred|0.9-14|
|isoband|0.2.7|
|iterators|1.0.14|
|jose|1.2.0|
|jquerylib|0.1.4|
|jsonlite|1.8.8|
|juicyjuice|0.1.0|
|knitr|1.45|
|labeling|0.4.3|
|later|1.3.2|
|lattice|0.22-5|
|lava|1.7.3|
|lazyeval|0.2.2|
|lhs|1.1.6|
|lifecycle|1.0.4|
|lightgbm|3.3.4|
|listenv|0.9.1|
|lobstr|1.1.2|
|lubridate|1.9.3|
|magrittr|2.0.3|
|maps|3.4.2|
|markdown|1.12|
|memoise|2.0.1|
|methods|4.2.3|
|mgcv|1.9-1|
|mime|0.12|
|miniUI|0.1.1.1|
|modeldata|1.3.0|
|modelenv|0.1.1|
|modelr|0.1.11|
|munsell|0.5.0|
|nlme|3.1-164|
|nnet|7.3-19|
|notebookutils|3.3.0-20240213.4|
|numDeriv|2016.8-1.1|
|openssl|2.1.1|
|pROC|1.18.5|
|parallel|4.2.3|
|parallelly|1.36.0|
|parsnip|1.1.1|
|patchwork|1.2.0|
|pillar|1.9.0|
|pkgbuild|1.4.2|
|pkgconfig|2.0.3|
|pkgdown|2.0.7|
|pkgload|1.3.4|
|plotly|4.10.1|
|plyr|1.8.9|
|praise|1.0.0|
|prettyunits|1.2.0|
|processx|3.8.3|
|prodlim|2023.08.28|
|profvis|0.3.8|
|progress|1.2.3|
|progressr|0.14.0|
|promises|1.2.1|
|proxy|0.4-27|
|pryr|0.1.6|
|ps|1.7.6|
|purrr|1.0.2|
|quantmod|0.4.25|
|r2d3|0.2.6|
|ragg|1.2.7|
|rappdirs|0.3.3|
|rbokeh|0.5.2|
|rcmdcheck|1.4.0|
|reactR|0.5.0|
|reactable|0.4.4|
|readr|2.1.5|
|readxl|1.4.3|
|recipes|1.0.9|
|rematch|2.0.0|
|rematch2|2.1.2|
|remotes|2.4.2.1|
|reprex|2.1.0|
|reshape2|1.4.4|
|rjson|0.2.21|
|rlang|1.1.3|
|rlist|0.4.6.2|
|rmarkdown|2.19|
|roxygen2|7.3.1|
|rpart|4.1.23|
|rprojroot|2.0.4|
|rsample|1.2.0|
|rstudioapi|0.15.0|
|rversions|2.1.2|
|rvest|1.0.3|
|sass|0.4.8|
|scales|1.3.0|
|selectr|0.4-2|
|sessioninfo|1.2.2|
|shape|1.4.6|
|shiny|1.8.0|
|slider|0.3.1|
|sourcetools|0.1.7-1|
|sparklyr|1.8.2|
|splines|4.2.3|
|stats|4.2.3|
|stats4|4.2.3|
|stringi|1.8.3|
|stringr|1.5.1|
|survival|3.5-7|
|sys|3.4.2|
|systemfonts|1.0.5|
|tcltk|4.2.3|
|testthat|3.2.1|
|textshaping|0.3.7|
|tibble|3.2.1|
|tidymodels|1.0.0|
|tidyr|1.3.1|
|tidyselect|1.2.0|
|tidyverse|1.3.2|
|timeDate|4032.109|
|timechange|0.3.0|
|tinytex|0.49|
|tools|4.2.3|
|torch|0.9.0|
|triebeard|0.4.1|
|tune|1.1.2|
|tzdb|0.4.0|
|urlchecker|1.0.1|
|urltools|1.7.3|
|usethis|2.2.2|
|utf8|1.2.4|
|utils|4.2.3|
|uuid|1.2-0|
|vctrs|0.6.5|
|viridisLite|0.4.2|
|vroom|1.6.5|
|waldo|0.5.2|
|warp|0.2.1|
|whisker|0.4.1|
|withr|3.0.0|
|workflows|1.1.3|
|workflowsets|1.0.1|
|xfun|0.41|
|xgboost|1.7.1.1|
|xml2|1.3.6|
|xopen|1.0.0|
|xtable|1.8-4|
|xts|0.13.2|
|yaml|2.3.8|
|yardstick|1.3.0|
|zip|2.3.1|
|zoo|1.8-12|
