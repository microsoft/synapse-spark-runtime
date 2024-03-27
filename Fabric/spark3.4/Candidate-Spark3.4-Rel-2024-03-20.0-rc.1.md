# System Environment
*   **Vhd Release**: Spark3.4-Rel-2024-03-20.0-rc.1
*   **Operating System**: CBL-Mariner 2.0.20240301
*   **Java**: 11.0.22
*   **Scala**: 2.12.17
*   **Python**: 3.10/2.0.0
*   **Delta Lake**: 2.4.0.9

# New Features

|Id|Component|Title|Description|
|-----|-----|-----|-----|
|1280239|ExternalHiveMetastoreLibraries/spark34:0.0.5|Remove support of external hive metastore in spark 3.4|Remove support of external hive metastore in spark 3.4.|
|1296161|AutoscaleProbe:3.9.0|Release Autoscale Version 3.9.0|New Autoscale Version Contains Several BugFixes like Autoscale Stuck in Scale Dowm Validation, Fixes for incorrect metrics and Support for Autoscale in Case of Cluster Fragmentation|
|1294510|NotebookUtils:1.1.47|Update NotebookUtils version to 1.1.47 for Spark 3.4|Update NotebookUtils version for Spark 3.4 to 1.1.4 with a number of bug fixes and improvements, including support for fabric REST API call via notebookutils ( https://learn.microsoft.com/en-us/rest/api/fabric/articles/ ).|

# Improvements

|Id|Component|Title|Description|
|-----|-----|-----|-----|
|1276618|Conda:8.0.10|Update Conda version to 8.0.10 in Spark 3.4 to include flaml upgrade|Upgrade FLAML for multiple improvements.|
|1290308|Autotune:1.11.0|Bump autotune version to 1.11.0.|To align with the new 1.11.0 release, there are no client-side changes required. The key enhancements for the Autotune backend include fixes for the state store delta table compaction and an increase in cluster and streaming job resources to enhance system throughput.|
|1293790|ServiceConfigurationTemplates:spark/3.4.0|Add spark config for PBI spark native connector|Add spark config for PBI spark native connector|
|1298594|Conda:8.0.13|Update synapse python package list in spark 3.4|Update synapse python runtime 3.4 for GA.|
|1284642|Conda:8.0.12, LibraryManager:1.0.8|Support for updates in each individual Python/R environments|In this PR we refactor the versioning scheme use to track conda.tar versions|
|1294510|NotebookUtils:1.1.47|Update NotebookUtils version to 1.1.47 for Spark 3.4|Update NotebookUtils version for Spark 3.4 to 1.1.4 with a number of bug fixes and improvements, including support for fabric REST API call via notebookutils ( https://learn.microsoft.com/en-us/rest/api/fabric/articles/ ).|
|1288898|Wildfire/spark34:1.9.4|New spark 3.4 release|CVE fixes across Spark, Hadoop, Livy and Hive. Also, Livy carrying few changes related to REPL, SQL result and session warmup.|

# Bug Fixes

|Id|Component|Title|Description|
|-----|-----|-----|-----|
|1276537|SparkRPCHistoryServer:1.0.30|Fix a permissions issue in Spark UI|Fix a permission issue impacting running of Spark UI application|
|1300020|Conda:8.0.14|Using Conda tar built from main branch.|Update synapse python package list in spark 3.4|
|1285129|ServiceConfigurationTemplates:spark/3.4.0|Start Livy Web Server only after checking that OLC service is up|In Fabric, there is no dependency of Livy on OLC service. Sometimes Livy starts up and is ready to accept requests sooner than OLC service becomes ready. When this happens, we can get requests that later will fail, if they depend on OLC service.In this PR, we start Livy - but we pause before starting the Web Server (Livy component) and wait until OLC service is ready.|
|1280584|ServiceConfigurationTemplates:spark/3.4.0|Make explicit dependency between Livy and Yarn NM|When Livy submit a job to Yarn, Yarn NM might not be ready. By making Livy starts after Yarn NM is started, we can reduce the subtle timing issue related with the dependency.|
|1295591|ServiceConfigurationTemplates:spark/3.4.0|Reverts enablement of flag to check OLC status before starting Livy|Reverting change of start Livy Web Server only after checking that OLC service is up.|
|1277086|Conda:8.0.11|Fix Fabric runtime 1.2 to install semantic-link-sempy package|Install back semantic-link-sempy (v0.5.1) back to the default Fabric 1.2 runtime for machine learning.|
|1286656|LibraryManager:1.0.7|Fix bug for Synapse where session was kept alive if session library management failed|Resolved Synapse regression where a session library management fails but the session is not killed|
|1276600|SparkDiagnosticsLibrary:1.0.20|Fixed potential logging-related security issue|Fixed a potential security issue related to logging Spark configurations|
|1285604|OneLakeClientStarter:1.0.19.2|Fixes for OLC self signed certificate for Velox and Delta-Rust.|OLC certificates are currently not working for delta rust and Velox. This change fixes it.|
|1296161|AutoscaleProbe:3.9.0|Release Autoscale Version 3.9.0|New Autoscale Version Contains Several BugFixes like Autoscale Stuck in Scale Dowm Validation, Fixes for incorrect metrics and Support for Autoscale in Case of Cluster Fragmentation|
|1295322|TokenLibrary:4.0.3|Minor bug fix for TokenLibrary to address connectivity issue in CosmosDB Connector|Minor bug fix for TokenLibrary to address connectivity issue in CosmosDB Connector|
|1294510|NotebookUtils:1.1.47|Update NotebookUtils version to 1.1.47 for Spark 3.4|Update NotebookUtils version for Spark 3.4 to 1.1.4 with a number of bug fixes and improvements, including support for fabric REST API call via notebookutils ( https://learn.microsoft.com/en-us/rest/api/fabric/articles/ ).|
|1285491|CSparkMetricUpdate: 1.0.1|Redact information from telemetry|Redact sensitive information from telemetry|
|1269880|TokenLibrary:4.0.2|Minor bug fix on TokenLibrary|Minor bug fix on TokenLibrary for some internal use cases|

# Components

|Name|Version|
|-----|-----|
|**AutoscaleProbe**|**3.8.1.1 --> 3.9.0**|
|**Autotune**|**1.10.0.0 --> 1.11.0.0**|
|AzureMLExtensions|1.0.3|
|**CSparkMetricUpdate**|**1.0.0 --> 1.0.1**|
|**Conda**|**8.0.9 --> 8.0.14**|
|CosmosDBConnector|1.8.10|
|DWConnector|1.0.0|
|Delta|2.4.0.9|
|EventHubConnector|2.3.25|
|FsspecWrapper|1.0.14|
|Genesis|0.28.0|
|Gluten|0.5.4|
|HiveMetaStoreClient|1.1.17|
|Impulse|1.2.1|
|JupyterServices|0.0.4|
|KustoConnector|1.3.4|
|**LibraryManager**|**1.0.6 --> 1.0.8**|
|LibraryMetadataCooker|1.0.0|
|MMLSpark|1.4.14|
|MachineLearningPredict|1.0.0|
|MlflowLibrary|2.6.0|
|MySQLJavaConnector|1.0.2|
|**NotebookUtils**|**1.1.46 --> 1.1.48**|
|**OneLakeClientStarter**|**1.0.19.1 --> 1.0.19.2**|
|**OnelakeSparkCatalog**|**0.1.3**|
|Peregrine|0.10.3|
|PostgreSQLJDBCDriver|1.0.2|
|Python|3.10/2.0.0|
|R|1.0.3|
|SQLServerODBCDriver|18.1.0|
|SStreamOnSparkJar|2.3.5|
|SparkAdvisor|0.0.15|
|**SparkDiagnosticsLibrary**|**1.0.19 --> 1.0.20**|
|SparkLighter|2.0.8|
|SparkNativeParquetWriter|0.12.1|
|**SparkRPCHistoryServer**|**1.0.29 --> 1.0.30**|
|SparklyrConnector|1.0.0|
|**TokenLibrary**|**4.0.1 --> 4.0.3**|
|**TridentCore**|**1.1.41 --> 1.2.6**|
|TridentTokenLibrary|1.6.2|
|Vegas|3.4.08.6|
|**Wildfire**|**1.9.3 --> 1.9.5**|

# Python Modules
### Environment: Synapse

|Name|Version|
|-----|-----|
|_libgcc_mutex|0.1|
|_openmp_mutex|4.5|
|_py-xgboost-mutex|2.0|
|**absl-py**|**1.4.0 --> 2.1.0**|
|adal|1.2.7|
|**adlfs**|**2023.4.0 --> 2023.10.0**|
|**aiohttp**|**3.8.5 --> 3.9.3**|
|aiosignal|1.3.1|
|**alsa-lib**|**1.2.9 --> 1.2.11**|
|anyio|3.7.1|
|applicationinsights|0.11.10|
|**argcomplete**|**2.1.2 --> 3.2.3**|
|argon2-cffi|23.1.0|
|argon2-cffi-bindings|21.2.0|
|**arrow**|**1.2.3 --> 1.3.0**|
|asttokens|2.4.1|
|astunparse|1.6.3|
|async-timeout|4.0.3|
|attr|2.5.1|
|**attrs**|**23.1.0 --> 23.2.0**|
|**aws-c-auth**|**0.7.3 --> 0.7.11**|
|**aws-c-cal**|**0.6.1 --> 0.6.9**|
|**aws-c-common**|**0.9.0 --> 0.9.12**|
|aws-c-compression|0.2.17|
|**aws-c-event-stream**|**0.3.1 --> 0.4.1**|
|**aws-c-http**|**0.7.11 --> 0.8.0**|
|**aws-c-io**|**0.13.32 --> 0.14.0**|
|**aws-c-mqtt**|**0.9.3 --> 0.10.1**|
|**aws-c-s3**|**0.3.14 --> 0.4.9**|
|**aws-c-sdkutils**|**0.1.12 --> 0.1.13**|
|aws-checksums|0.1.17|
|**aws-crt-cpp**|**0.21.0 --> 0.26.0**|
|**aws-sdk-cpp**|**1.10.57 --> 1.11.210**|
|**azure-ai-ml**|**1.9.0 --> 1.12.1**|
|azure-common|1.1.28|
|**azure-core**|**1.29.3 --> 1.30.1**|
|azure-datalake-store|0.0.51|
|azure-graphrbac|0.61.1|
|**azure-identity**|**1.12.0 --> 1.15.0**|
|**azure-mgmt-authorization**|**3.0.0 --> 4.0.0**|
|**azure-mgmt-containerregistry**|**10.1.0 --> 10.3.0**|
|azure-mgmt-core|1.4.0|
|**azure-mgmt-keyvault**|**10.2.3 --> 10.3.0**|
|**azure-mgmt-network**|**21.0.1 --> 25.2.0**|
|**azure-mgmt-resource**|**22.0.0 --> 23.0.1**|
|**azure-mgmt-storage**|**21.0.0 --> 21.1.0**|
|**azure-storage-blob**|**12.13.0 --> 12.19.0**|
|**azure-storage-file-datalake**|**12.8.0 --> 12.14.0**|
|**azure-storage-file-share**|**12.13.0 --> 12.15.0**|
|azure-synapse-ml-predict|1.0.0|
|**azureml-core**|**1.53.0 --> 1.55.0**|
|**azureml-dataprep**|**4.12.1 --> 5.1.6**|
|**azureml-dataprep-native**|**38.0.0 --> 41.0.0**|
|**azureml-dataprep-rslex**|**2.19.1 --> 2.22.2**|
|**azureml-dataset-runtime**|**1.53.0 --> 1.55.0**|
|**azureml-mlflow**|**1.53.0 --> 1.55.0**|
|**azureml-opendatasets**|**1.53.0 --> 1.55.0**|
|azureml-synapse|0.0.1|
|**azureml-telemetry**|**1.53.0 --> 1.55.0**|
|backcall|0.2.0|
|backports-tempfile|1.0|
|backports-weakref|1.0.post1|
|**bcrypt**|**3.2.2 --> 4.1.2**|
|beautifulsoup4|4.12.2|
|blas|1.0|
|**bleach**|**6.0.0 --> 6.1.0**|
|**blinker**|**1.6.2 --> 1.7.0**|
|**brotli**|**1.0.9 --> 1.1.0**|
|**brotli-bin**|**1.0.9 --> 1.1.0**|
|**brotli-python**|**1.0.9 --> 1.1.0**|
|bzip2|1.0.8|
|**c-ares**|**1.19.1 --> 1.27.0**|
|ca-certificates|2024.2.2|
|cached-property|1.5.2|
|cached_property|1.5.2|
|**cachetools**|**5.3.1 --> 5.3.3**|
|**cairo**|**1.16.0 --> 1.18.0**|
|certifi|2024.2.2|
|cffi|1.16.0|
|charset-normalizer|3.3.2|
|click|8.1.7|
|cloudpickle|2.2.1|
|clr_loader|0.2.6|
|colorama|0.4.6|
|**comm**|**0.1.4 --> 0.2.2**|
|conda-package-handling|2.2.0|
|conda-package-streaming|0.9.0|
|**configparser**|**5.3.0 --> 6.0.1**|
|contextlib2|21.6.0|
|contourpy|1.2.0|
|control-script|1.0.3|
|**cryptography**|**42.0.4 --> 41.0.7**|
|**cryptography**|**42.0.4 --> 42.0.5**|
|cycler|0.12.1|
|**dash**|**2.13.0 --> 2.16.1**|
|dash-core-components|2.0.0|
|dash-html-components|2.0.0|
|dash-table|5.0.0|
|dash_cytoscape|0.2.0|
|**databricks-cli**|**0.17.7 --> 0.18.0**|
|dbus|1.13.6|
|debugpy|1.8.1|
|decorator|5.1.1|
|defusedxml|0.7.1|
|**dill**|**0.3.7 --> 0.3.8**|
|**distlib**|**0.3.7 --> 0.3.8**|
|**docker-py**|**6.1.3 --> 7.0.0**|
|entrypoints|0.4|
|et_xmlfile|1.1.0|
|exceptiongroup|1.2.0|
|executing|2.0.1|
|**expat**|**2.5.0 --> 2.6.2**|
|**filelock**|**3.12.3 --> 3.13.1**|
|**flask**|**2.3.3 --> 3.0.2**|
|flatbuffers|23.5.26|
|fluent-logger|0.10.0|
|font-ttf-dejavu-sans-mono|2.37|
|font-ttf-inconsolata|3.000|
|font-ttf-source-code-pro|2.038|
|font-ttf-ubuntu|0.83|
|fontconfig|2.14.2|
|fonts-conda-ecosystem|1|
|fonts-conda-forge|1|
|**fonttools**|**4.42.1 --> 4.50.0**|
|fonttools|4.49.0|
|fqdn|1.5.1|
|freetype|2.12.1|
|**frozenlist**|**1.4.0 --> 1.4.1**|
|**fsspec**|**2023.6.0 --> 2024.2.0**|
|fsspec_wrapper|0.1.13|
|fusepy|3.0.1|
|**gast**|**0.4.0 --> 0.5.4**|
|**geographiclib**|**1.52 --> 2.0**|
|**geopy**|**2.3.0 --> 2.4.1**|
|gettext|0.21.1|
|**gevent**|**22.10.2 --> 23.9.0.post1**|
|gflags|2.2.2|
|giflib|5.2.1|
|**gitdb**|**4.0.10 --> 4.0.11**|
|**gitpython**|**3.1.32 --> 3.1.42**|
|**glib**|**2.76.4 --> 2.80.0**|
|**glib-tools**|**2.76.4 --> 2.80.0**|
|glog|0.6.0|
|**gmp**|**6.2.1 --> 6.3.0**|
|gmpy2|2.1.2|
|**google-api-core**|**2.11.1 --> 2.17.1**|
|**google-auth**|**2.17.3 --> 2.28.2**|
|**google-auth-oauthlib**|**1.0.0 --> 1.2.0**|
|google-pasta|0.2.0|
|**googleapis-common-protos**|**1.60.0 --> 1.63.0**|
|graphite2|1.3.13|
|**greenlet**|**2.0.2 --> 3.0.3**|
|**grpcio**|**1.54.3 --> 1.59.3**|
|**gst-plugins-base**|**1.22.5 --> 1.22.9**|
|**gstreamer**|**1.22.5 --> 1.22.9**|
|**h5py**|**3.9.0 --> 3.10.0**|
|**harfbuzz**|**7.3.0 --> 8.3.0**|
|**hdf5**|**1.14.2 --> 1.14.3**|
|html5lib|1.1|
|humanfriendly|10.0|
|**icu**|**72.1 --> 73.2**|
|idna|3.6|
|**imageio**|**2.31.1 --> 2.33.1**|
|**importlib-metadata**|**6.8.0 --> 7.0.2**|
|**importlib_metadata**|**6.8.0 --> 7.0.2**|
|**importlib_resources**|**6.0.1 --> 6.3.0**|
|impulse-python-handler|1.0.19.1.0.0|
|**interpret**|**0.4.3 --> 0.5.0**|
|**interpret-core**|**0.4.3 --> 0.5.0**|
|**ipykernel**|**6.25.1 --> 6.29.3**|
|**ipython**|**8.14.0 --> 8.22.2**|
|ipython|8.14.0|
|ipywidgets|8.1.2|
|ipywidgets|8.0.7|
|isodate|0.6.1|
|isoduration|20.11.0|
|itsdangerous|2.1.2|
|jedi|0.19.1|
|jeepney|0.8.0|
|**jinja2**|**3.1.2 --> 3.1.3**|
|jmespath|1.0.1|
|joblib|1.3.2|
|**jsonpickle**|**3.0.2 --> 3.0.3**|
|**jsonpointer**|**2.0 --> 2.4**|
|**jsonschema**|**4.19.0 --> 4.21.1**|
|**jsonschema-specifications**|**2023.7.1 --> 2023.12.1**|
|**jsonschema-with-format-nongpl**|**4.19.0 --> 4.21.1**|
|**jupyter-client**|**8.6.0 --> 8.6.1**|
|**jupyter-core**|**5.7.1 --> 5.7.2**|
|jupyter-ui-poll|0.2.2|
|**jupyter_client**|**8.3.1 --> 8.6.1**|
|**jupyter_core**|**5.3.1 --> 5.7.2**|
|**jupyter_events**|**0.7.0 --> 0.9.1**|
|jupyter_server|2.7.0|
|**jupyter_server_terminals**|**0.4.4 --> 0.5.3**|
|jupyterlab-widgets|3.0.10|
|**jupyterlab_pygments**|**0.2.2 --> 0.3.0**|
|**jupyterlab_widgets**|**3.0.8 --> 3.0.10**|
|**keras**|**2.12.0 --> 2.15.0**|
|keyutils|1.6.1|
|kiwisolver|1.4.5|
|**knack**|**0.10.1 --> 0.11.0**|
|krb5|1.21.2|
|lame|3.100|
|**lcms2**|**2.15 --> 2.16**|
|ld_impl_linux-64|2.40|
|lerc|4.0.0|
|liac-arff|2.5.0|
|**libabseil**|**20230125.3 --> 20230802.1**|
|**libaec**|**1.0.6 --> 1.1.2**|
|**libarrow**|**12.0.1 --> 14.0.2**|
|**libarrow-acero**|**14.0.2**|
|**libarrow-dataset**|**14.0.2**|
|**libarrow-flight**|**14.0.2**|
|**libarrow-flight-sql**|**14.0.2**|
|**libarrow-gandiva**|**14.0.2**|
|**libarrow-substrait**|**14.0.2**|
|**libbrotlicommon**|**1.0.9 --> 1.1.0**|
|**libbrotlidec**|**1.0.9 --> 1.1.0**|
|**libbrotlienc**|**1.0.9 --> 1.1.0**|
|libcap|2.69|
|libclang|15.0.7|
|libclang13|15.0.7|
|libcrc32c|1.1.2|
|libcups|2.3.3|
|**libcurl**|**8.2.1 --> 8.5.0**|
|**libdeflate**|**1.18 --> 1.19**|
|**libebm**|**0.4.3 --> 0.5.0**|
|libedit|3.1.20191231|
|libev|4.33|
|libevent|2.1.12|
|**libexpat**|**2.5.0 --> 2.6.2**|
|libffi|3.4.2|
|libflac|1.4.3|
|libgcc-ng|13.2.0|
|**libgcrypt**|**1.10.1 --> 1.10.3**|
|**libgfortran-ng**|**13.1.0 --> 13.2.0**|
|**libgfortran5**|**13.1.0 --> 13.2.0**|
|**libgirepository**|**1.78.1**|
|**libglib**|**2.76.4 --> 2.80.0**|
|libgomp|13.2.0|
|libgoogle-cloud|2.12.0|
|**libgpg-error**|**1.47 --> 1.48**|
|**libgrpc**|**1.54.3 --> 1.59.3**|
|**libhwloc**|**2.9.2 --> 2.9.3**|
|libiconv|1.17|
|**libjpeg-turbo**|**2.1.5.1 --> 3.0.0**|
|libllvm14|14.0.6|
|libllvm15|15.0.7|
|**libnghttp2**|**1.52.0 --> 1.58.0**|
|**libnl**|**3.9.0**|
|libnsl|2.0.1|
|libogg|1.3.4|
|libopus|1.3.1|
|**libparquet**|**14.0.2**|
|**libpng**|**1.6.39 --> 1.6.43**|
|**libpq**|**15.4 --> 16.2**|
|**libprotobuf**|**3.21.12 --> 4.24.4**|
|library-metadata-cooker|0.0.7|
|**libre2-11**|**2023.09.01**|
|**libsecret**|**0.18.8**|
|libsndfile|1.2.2|
|libsodium|1.0.18|
|**libsqlite**|**3.43.0 --> 3.45.2**|
|libssh2|1.11.0|
|**libstdcxx-ng**|**13.1.0 --> 13.2.0**|
|**libsystemd0**|**254 --> 255**|
|**libthrift**|**0.18.1 --> 0.19.0**|
|**libtiff**|**4.5.1 --> 4.6.0**|
|libutf8proc|2.8.0|
|libuuid|2.38.1|
|**libuv**|**1.46.0 --> 1.48.0**|
|libvorbis|1.3.7|
|**libwebp-base**|**1.3.1 --> 1.3.2**|
|libxcb|1.15|
|libxcrypt|4.4.36|
|**libxgboost**|**1.7.6 --> 2.0.3**|
|**libxkbcommon**|**1.5.0 --> 1.6.0**|
|**libxml2**|**2.11.5 --> 2.12.5**|
|**libxslt**|**1.1.37 --> 1.1.39**|
|libzlib|1.2.13|
|**lightgbm**|**4.0.0 --> 4.2.0**|
|**llvm-openmp**|**16.0.6 --> 17.0.6**|
|**llvmlite**|**0.40.1 --> 0.42.0**|
|**lxml**|**4.9.3 --> 5.1.0**|
|lz4-c|1.9.4|
|**markdown**|**3.4.4 --> 3.5.1**|
|**markupsafe**|**2.1.3 --> 2.1.5**|
|**marshmallow**|**3.20.1 --> 3.21.1**|
|**matplotlib**|**3.7.2 --> 3.8.2**|
|matplotlib|3.8.3|
|**matplotlib-base**|**3.7.2 --> 3.8.2**|
|matplotlib-inline|0.1.6|
|**mistune**|**3.0.1 --> 3.0.2**|
|**mkl**|**2021.4.0 --> 2023.2.0**|
|**mkl-service**|**2.4.0 --> 2.4.1**|
|**mkl_fft**|**1.3.1 --> 1.3.8**|
|**mkl_random**|**1.2.2 --> 1.2.5**|
|ml_dtypes|0.2.0|
|**mlflow-skinny**|**2.6.0 --> 2.9.2**|
|**mltable**|**1.5.0 --> 1.6.1**|
|mpc|1.3.1|
|**mpfr**|**4.2.0 --> 4.2.1**|
|**mpg123**|**1.31.3 --> 1.32.4**|
|mpmath|1.3.0|
|**msal**|**1.23.0 --> 1.28.0**|
|**msal**|**1.23.0 --> 1.27.0**|
|**msal_extensions**|**1.0.0 --> 1.1.0**|
|**msgpack**|**1.0.5 --> 1.0.8**|
|msrest|0.7.1|
|msrestazure|0.6.4|
|**multidict**|**6.0.4 --> 6.0.5**|
|**multiprocess**|**0.70.15 --> 0.70.16**|
|munkres|1.1.4|
|mypy|1.4.1|
|mypy-extensions|1.0.0|
|mysql-common|8.0.33|
|mysql-libs|8.0.33|
|**nbclient**|**0.8.0 --> 0.10.0**|
|**nbconvert-core**|**7.8.0 --> 7.16.2**|
|**nbformat**|**5.9.2 --> 5.10.2**|
|ncurses|6.4|
|**ncurses**|**6.4 --> 6.4.20240210**|
|ndg-httpsclient|0.5.1|
|nest-asyncio|1.6.0|
|**networkx**|**3.1 --> 3.2.1**|
|**notebookutils**|**3.4.1-20240110.4 --> 3.4.1-20240309.2**|
|nspr|4.35|
|**nss**|**3.92 --> 3.98**|
|**numba**|**0.57.1 --> 0.59.0**|
|numpy|1.23.5|
|numpy|1.26.4|
|**numpy-base**|**1.24.3 --> 1.26.4**|
|oauthlib|3.2.2|
|**onnx**|**1.15.0**|
|**opencensus**|**0.11.2 --> 0.11.4**|
|opencensus-context|0.1.3|
|**opencensus-ext-azure**|**1.1.9 --> 1.1.13**|
|**openjpeg**|**2.5.0 --> 2.5.2**|
|openpyxl|3.1.2|
|openssl|3.2.1|
|opt_einsum|3.3.0|
|**orc**|**1.9.0 --> 1.9.2**|
|**overrides**|**7.4.0 --> 7.7.0**|
|**packaging**|**23.0 --> 24.0**|
|packaging|23.2|
|**pandas**|**1.5.3 --> 2.2.1**|
|pandas|1.5.3|
|pandasql|0.7.3|
|pandocfilters|1.5.0|
|**paramiko**|**3.3.1 --> 3.4.0**|
|parso|0.8.3|
|**pathos**|**0.3.1 --> 0.3.2**|
|**pathspec**|**0.11.2 --> 0.12.1**|
|**patsy**|**0.5.3 --> 0.5.6**|
|**pcre2**|**10.40 --> 10.43**|
|pexpect|4.9.0|
|pickleshare|0.7.5|
|pillow|10.2.0|
|pip|23.1.2|
|pip|22.3.1|
|**pixman**|**0.40.0 --> 0.43.2**|
|**pkginfo**|**1.9.6 --> 1.10.0**|
|pkgutil-resolve-name|1.3.10|
|**platformdirs**|**4.2.0 --> 3.11.0**|
|platformdirs|4.2.0|
|**plotly**|**5.16.1 --> 5.18.0**|
|ply|3.11|
|**portalocker**|**2.7.0 --> 2.8.2**|
|powerbiclient|3.1.1|
|**pox**|**0.3.3 --> 0.3.4**|
|**ppft**|**1.7.6.7 --> 1.7.6.8**|
|**prettytable**|**3.8.0 --> 3.9.0**|
|**prometheus_client**|**0.17.1 --> 0.20.0**|
|**prompt-toolkit**|**3.0.43 --> 3.0.42**|
|prompt-toolkit|3.0.43|
|**prompt_toolkit**|**3.0.39 --> 3.0.42**|
|**protobuf**|**4.21.12 --> 4.24.4**|
|psutil|5.9.8|
|pthread-stubs|0.4|
|ptyprocess|0.7.0|
|pulseaudio-client|16.1|
|pure-eval|0.2.2|
|pure_eval|0.2.2|
|**py-xgboost**|**1.7.6 --> 2.0.3**|
|py4j|0.10.9.7|
|**pyarrow**|**11.0.0 --> 14.0.2**|
|**pyasn1**|**0.4.8 --> 0.5.1**|
|**pyasn1-modules**|**0.2.7 --> 0.3.0**|
|**pycairo**|**1.26.0**|
|**pycosat**|**0.6.4 --> 0.6.6**|
|pycparser|2.21|
|**pydash**|**5.1.2 --> 7.0.5**|
|pygments|2.17.2|
|**pygobject**|**3.48.1**|
|pyjwt|2.8.0|
|pynacl|1.5.0|
|**pyodbc**|**4.0.39 --> 5.0.1**|
|**pyopenssl**|**23.2.0 --> 23.3.0**|
|**pyparsing**|**3.1.1 --> 3.1.2**|
|pyperclip|1.8.2|
|pyqt|5.15.9|
|pyqt5-sip|12.12.2|
|pysocks|1.7.1|
|**pyspark**|**3.5.0 --> 3.5.1**|
|pyspark|3.4.1.5.3.20230713|
|python|3.10.13|
|**python**|**3.10.12 --> 3.10.14**|
|**python-dateutil**|**2.8.2 --> 2.9.0.post0**|
|**python-dateutil**|**2.8.2 --> 2.9.0**|
|**python-fastjsonschema**|**2.18.0 --> 2.19.1**|
|**python-flatbuffers**|**23.5.26 --> 24.3.7**|
|python-json-logger|2.0.7|
|python_abi|3.10|
|**pythonnet**|**3.0.1 --> 3.0.3**|
|pytorch|2.0.1|
|pytorch-mutex|1.0|
|**pytz**|**2023.3 --> 2023.4**|
|pytz|2024.1|
|pyu2f|0.1.5|
|pywin32-on-windows|0.1.0|
|pyyaml|6.0.1|
|pyzmq|25.1.2|
|qt-main|5.15.8|
|**rdma-core**|**28.9 --> 50.0**|
|**re2**|**2023.03.02 --> 2023.09.01**|
|readline|8.2|
|**referencing**|**0.30.2 --> 0.33.0**|
|**regex**|**2023.8.8 --> 2023.12.25**|
|requests|2.31.0|
|**requests-oauthlib**|**1.3.1 --> 1.4.0**|
|retrying|1.3.3|
|rfc3339-validator|0.1.4|
|rfc3986-validator|0.1.1|
|**rpds-py**|**0.10.0 --> 0.18.0**|
|rsa|4.9|
|**ruamel.yaml**|**0.17.32 --> 0.18.5**|
|ruamel.yaml.clib|0.2.7|
|ruamel_yaml|0.15.80|
|**s2n**|**1.3.49 --> 1.4.1**|
|**salib**|**1.4.7 --> 1.4.8**|
|**scikit-learn**|**1.3.0 --> 1.3.2**|
|**scipy**|**1.10.1 --> 1.11.4**|
|**seaborn**|**0.12.2 --> 0.13.1**|
|**seaborn-base**|**0.12.2 --> 0.13.1**|
|secretstorage|3.3.3|
|send2trash|1.8.2|
|**setuptools**|**68.1.2 --> 69.2.0**|
|**shap**|**0.42.1 --> 0.44.0**|
|**sip**|**6.7.11 --> 6.7.12**|
|six|1.16.0|
|slicer|0.0.7|
|**smmap**|**3.0.5 --> 5.0.0**|
|snappy|1.1.10|
|**sniffio**|**1.3.0 --> 1.3.1**|
|**soupsieve**|**2.3.2.post1 --> 2.5**|
|**sqlalchemy**|**2.0.20 --> 2.0.28**|
|sqlanalyticsconnectorpy|1.0.1|
|sqlparse|0.4.4|
|stack-data|0.6.3|
|stack_data|0.6.2|
|**statsmodels**|**0.14.0 --> 0.14.1**|
|strictyaml|1.7.3|
|sympy|1.12|
|synapseml-cognitive|1.0.2|
|synapseml-core|1.0.2|
|synapseml-deep-learning|1.0.2|
|synapseml-internal|1.0.2.1.dev1|
|synapseml-lightgbm|1.0.2|
|synapseml-opencv|1.0.2|
|synapseml-vw|1.0.2|
|tabulate|0.9.0|
|**tbb**|**2021.10.0 --> 2021.11.0**|
|tenacity|8.2.3|
|**tensorboard**|**2.12.3 --> 2.15.2**|
|tensorboard-data-server|0.7.0|
|**tensorflow**|**2.12.1 --> 2.15.0**|
|**tensorflow-base**|**2.12.1 --> 2.15.0**|
|**tensorflow-estimator**|**2.12.1 --> 2.15.0**|
|**termcolor**|**2.3.0 --> 2.4.0**|
|**terminado**|**0.17.1 --> 0.18.1**|
|**threadpoolctl**|**3.2.0 --> 3.3.0**|
|tinycss2|1.2.1|
|tk|8.6.13|
|toml|0.10.2|
|tomli|2.0.1|
|**toolz**|**0.12.0 --> 0.12.1**|
|tornado|6.4|
|**tqdm**|**4.66.1 --> 4.66.2**|
|**traitlets**|**5.9.0 --> 5.14.2**|
|typed-ast|1.5.5|
|**types-python-dateutil**|**2.8.19.20240311**|
|**typing-extensions**|**4.9.0 --> 4.10.0**|
|**typing_extensions**|**4.5.0 --> 4.10.0**|
|typing_utils|0.1.0|
|**tzdata**|**2023c --> 2024a**|
|tzdata|2024.1|
|**ucx**|**1.14.1 --> 1.15.0**|
|**unicodedata2**|**15.0.0 --> 15.1.0**|
|unixodbc|2.3.12|
|uri-template|1.3.0|
|**urllib3**|**1.26.16 --> 2.1.0**|
|urllib3|2.2.1|
|virtualenv|20.23.1|
|wcwidth|0.2.13|
|webcolors|1.13|
|webencodings|0.5.1|
|**websocket-client**|**1.6.2 --> 1.7.0**|
|**werkzeug**|**2.3.7 --> 3.0.1**|
|wheel|0.42.0|
|widgetsnbextension|4.0.10|
|**wrapt**|**1.15.0 --> 1.14.1**|
|xcb-util|0.4.0|
|xcb-util-image|0.4.0|
|xcb-util-keysyms|0.4.0|
|xcb-util-renderutil|0.3.9|
|xcb-util-wm|0.4.1|
|**xgboost**|**1.7.6 --> 2.0.3**|
|**xkeyboard-config**|**2.39 --> 2.41**|
|xorg-kbproto|1.0.7|
|xorg-libice|1.1.1|
|xorg-libsm|1.2.4|
|**xorg-libx11**|**1.8.6 --> 1.8.7**|
|xorg-libxau|1.0.11|
|xorg-libxdmcp|1.1.3|
|xorg-libxext|1.3.4|
|xorg-libxrender|0.9.11|
|xorg-renderproto|0.11.1|
|xorg-xextproto|7.3.0|
|xorg-xf86vidmodeproto|2.3.1|
|xorg-xproto|7.0.31|
|xz|5.2.6|
|yaml|0.2.5|
|**yarl**|**1.9.2 --> 1.9.4**|
|**zeromq**|**4.3.4 --> 4.3.5**|
|**zipp**|**3.16.2 --> 3.17.0**|
|zlib|1.2.13|
|zope.event|5.0|
|**zope.interface**|**6.0 --> 6.2**|
|**zstandard**|**0.19.0 --> 0.22.0**|
|zstd|1.5.5|

### Environment: Fabric

|Name|Version|
|-----|-----|
|_openmp_mutex|4.5|
|_py-xgboost-mutex|2.0|
|absl-py|2.0.0|
|adal|1.2.7|
|adlfs|2023.4.0|
|aiohttp|3.8.6|
|aiosignal|1.3.1|
|alembic|1.12.0|
|alsa-lib|1.2.10|
|ansi2html|1.8.0|
|anyio|3.7.1|
|appdirs|1.4.4|
|argon2-cffi|23.1.0|
|argon2-cffi-bindings|21.2.0|
|arrow|1.3.0|
|astor|0.8.1|
|asttokens|2.4.0|
|astunparse|1.6.3|
|async-timeout|4.0.3|
|atk-1.0|2.38.0|
|attr|2.5.1|
|attrs|23.1.0|
|autopage|0.5.2|
|aws-c-auth|0.7.3|
|aws-c-cal|0.6.1|
|aws-c-common|0.9.0|
|aws-c-compression|0.2.17|
|aws-c-event-stream|0.3.1|
|aws-c-http|0.7.11|
|aws-c-io|0.13.32|
|aws-c-mqtt|0.9.3|
|aws-c-s3|0.3.14|
|aws-c-sdkutils|0.1.12|
|aws-checksums|0.1.17|
|aws-crt-cpp|0.21.0|
|aws-sdk-cpp|1.10.57|
|azure-core|1.29.4|
|azure-datalake-store|0.0.51|
|azure-identity|1.14.1|
|azure-storage-blob|12.18.3|
|azure-storage-file-datalake|12.12.0|
|azure-synapse-ml-predict|1.0.0|
|azureml-synapse|0.0.1|
|backcall|0.2.0|
|backoff|1.11.1|
|backports|1.0|
|backports.functools_lru_cache|1.6.5|
|bcrypt|4.0.1|
|beautifulsoup4|4.12.2|
|blas|1.0|
|bleach|6.1.0|
|blinker|1.6.3|
|brotli|1.0.9|
|brotli-bin|1.0.9|
|brotli-python|1.0.9|
|bzip2|1.0.8|
|c-ares|1.20.1|
|ca-certificates|2023.7.22|
|cached-property|1.5.2|
|cached_property|1.5.2|
|cachetools|5.3.2|
|cairo|1.18.0|
|catboost|1.1.1|
|certifi|2023.7.22|
|cffi|1.16.0|
|charset-normalizer|3.3.1|
|chroma-hnswlib|0.7.3|
|chromadb|0.4.13|
|click|8.1.7|
|cliff|4.2.0|
|cloudpickle|2.2.1|
|clr_loader|0.2.6|
|cmaes|0.10.0|
|cmd2|2.4.3|
|colorama|0.4.6|
|coloredlogs|15.0.1|
|colorlog|6.7.0|
|comm|0.1.4|
|conda-package-handling|2.2.0|
|conda-package-streaming|0.9.0|
|configparser|5.3.0|
|contextlib2|21.6.0|
|contourpy|1.1.1|
|cryptography|41.0.5|
|cycler|0.12.1|
|cython|3.0.4|
|dash|2.14.0|
|dash-core-components|2.0.0|
|dash-html-components|2.0.0|
|dash-table|5.0.0|
|dash_cytoscape|0.2.0|
|databricks-cli|0.18.0|
|dataclasses|0.8|
|datasets|2.14.6|
|dbus|1.13.6|
|debugpy|1.8.0|
|decorator|5.1.1|
|defusedxml|0.7.1|
|dill|0.3.7|
|diskcache|5.6.3|
|distlib|0.3.7|
|docker-py|6.1.3|
|docker-pycreds|0.4.0|
|entrypoints|0.4|
|et_xmlfile|1.1.0|
|exceptiongroup|1.1.3|
|executing|1.2.0|
|expat|2.5.0|
|fastapi|0.103.2|
|filelock|3.11.0|
|**flaml**|**2.1.1post3 --> 2.1.1post4**|
|flask|3.0.0|
|flatbuffers|23.5.26|
|fluent-logger|0.10.0|
|font-ttf-dejavu-sans-mono|2.37|
|font-ttf-inconsolata|3.000|
|font-ttf-source-code-pro|2.038|
|font-ttf-ubuntu|0.83|
|fontconfig|2.14.2|
|fonts-conda-ecosystem|1|
|fonts-conda-forge|1|
|fonttools|4.43.1|
|fqdn|1.5.1|
|freetype|2.12.1|
|fribidi|1.0.10|
|frozenlist|1.4.0|
|fsspec|2023.10.0|
|fsspec_wrapper|0.1.12|
|gast|0.4.0|
|gdk-pixbuf|2.42.10|
|geographiclib|1.52|
|geopy|2.3.0|
|gettext|0.21.1|
|gevent|23.9.0.post1|
|gflags|2.2.2|
|giflib|5.2.1|
|gitdb|4.0.11|
|gitpython|3.1.40|
|glib|2.78.0|
|glib-tools|2.78.0|
|glog|0.6.0|
|gmp|6.2.1|
|gmpy2|2.1.2|
|google-auth|2.23.3|
|google-auth-oauthlib|1.0.0|
|google-pasta|0.2.0|
|graphite2|1.3.13|
|graphviz|8.1.0|
|greenlet|3.0.1|
|grpcio|1.54.3|
|gson|0.0.3|
|gst-plugins-base|1.22.6|
|gstreamer|1.22.6|
|gtk2|2.24.33|
|gts|0.7.6|
|h11|0.14.0|
|h5py|3.10.0|
|harfbuzz|8.2.1|
|hdf5|1.14.2|
|holidays|0.35|
|html5lib|1.1|
|huggingface_hub|0.18.0|
|humanfriendly|10.0|
|icu|73.2|
|idna|3.4|
|imageio|2.31.1|
|importlib-metadata|6.8.0|
|importlib-resources|6.1.0|
|importlib_metadata|6.8.0|
|importlib_resources|6.1.0|
|impulse-python-handler|1.0.19.1.0.0|
|intel-openmp|2021.4.0|
|interpret|0.4.3|
|interpret-core|0.4.3|
|ipykernel|6.26.0|
|ipython|8.14.0|
|ipywidgets|8.0.7|
|isodate|0.6.1|
|isoduration|20.11.0|
|itsdangerous|2.1.2|
|jaraco-context|4.3.0|
|jax|0.4.17|
|jaxlib|0.4.14|
|jedi|0.19.1|
|jinja2|3.1.2|
|joblib|1.3.2|
|joblibspark|0.5.2|
|json-tricks|3.17.3|
|jsonpointer|2.4|
|jsonschema|4.19.1|
|jsonschema-specifications|2023.7.1|
|jsonschema-with-format-nongpl|4.19.1|
|jupyter-ui-poll|0.2.2|
|jupyter_client|8.5.0|
|jupyter_core|5.4.0|
|jupyter_events|0.8.0|
|jupyter_server|2.7.3|
|jupyter_server_terminals|0.4.4|
|jupyterlab_pygments|0.2.2|
|jupyterlab_widgets|3.0.9|
|keras|2.12.0|
|keras-preprocessing|1.1.2|
|keyutils|1.6.1|
|kiwisolver|1.4.5|
|krb5|1.21.2|
|lame|3.100|
|lcms2|2.15|
|ld_impl_linux-64|2.40|
|lerc|4.0.0|
|liac-arff|2.5.0|
|libabseil|20230125.3|
|libaec|1.1.2|
|libarrow|12.0.1|
|libbrotlicommon|1.0.9|
|libbrotlidec|1.0.9|
|libbrotlienc|1.0.9|
|libcap|2.69|
|libclang|15.0.7|
|libclang13|15.0.7|
|libcrc32c|1.1.2|
|libcups|2.3.3|
|libcurl|8.4.0|
|libdeflate|1.19|
|libebm|0.4.3|
|libedit|3.1.20191231|
|libev|4.33|
|libevent|2.1.12|
|libexpat|2.5.0|
|libffi|3.4.2|
|libflac|1.4.3|
|libgcc-ng|13.2.0|
|libgcrypt|1.10.1|
|libgd|2.3.3|
|libgfortran-ng|13.2.0|
|libgfortran5|13.2.0|
|libglib|2.78.0|
|libgoogle-cloud|2.12.0|
|libgpg-error|1.47|
|libgrpc|1.54.3|
|libhwloc|2.9.3|
|libiconv|1.17|
|libjpeg-turbo|2.1.5.1|
|libllvm14|14.0.6|
|libllvm15|15.0.7|
|libnghttp2|1.52.0|
|libnsl|2.0.1|
|libnuma|2.0.16|
|libogg|1.3.4|
|libopus|1.3.1|
|libpng|1.6.39|
|libpq|15.4|
|libprotobuf|3.21.12|
|libpulsar|3.2.0|
|library-metadata-cooker|0.0.7|
|librsvg|2.56.3|
|libsndfile|1.2.2|
|libsodium|1.0.18|
|libsqlite|3.43.2|
|libssh2|1.11.0|
|libstdcxx-ng|13.2.0|
|libsystemd0|254|
|libthrift|0.18.1|
|libtiff|4.6.0|
|libtool|2.4.7|
|libutf8proc|2.8.0|
|libuuid|2.38.1|
|libuv|1.46.0|
|libvorbis|1.3.7|
|libwebp|1.3.2|
|libwebp-base|1.3.2|
|libxcb|1.15|
|libxgboost|1.7.6|
|libxkbcommon|1.6.0|
|libxml2|2.11.5|
|libxslt|1.1.37|
|libzlib|1.2.13|
|lightgbm|4.0.0|
|lime|0.2.0.1|
|llvm-openmp|17.0.3|
|llvmlite|0.40.1|
|lxml|4.9.3|
|lz4-c|1.9.4|
|mako|1.2.4|
|markdown|3.4.4|
|markdown-it-py|3.0.0|
|markupsafe|2.1.3|
|matplotlib|3.7.2|
|matplotlib-base|3.7.2|
|matplotlib-inline|0.1.6|
|mdurl|0.1.0|
|mistune|3.0.1|
|mkl|2021.4.0|
|mkl-service|2.4.0|
|mkl_fft|1.3.1|
|mkl_random|1.2.2|
|ml_dtypes|0.3.1|
|mlflow-skinny|2.6.0|
|monotonic|1.5|
|more-itertools|10.1.0|
|mpc|1.3.1|
|mpfr|4.2.1|
|mpg123|1.32.3|
|mpmath|1.3.0|
|msal|1.24.1|
|msal_extensions|1.0.0|
|msgpack|1.0.7|
|multidict|6.0.4|
|multiprocess|0.70.15|
|munkres|1.1.4|
|mypy|1.4.1|
|mypy-extensions|1.0.0|
|mysql-common|8.0.33|
|mysql-libs|8.0.33|
|nbclient|0.8.0|
|nbconvert-core|7.9.2|
|nbformat|5.9.2|
|ncurses|6.4|
|nest-asyncio|1.5.8|
|networkx|3.2|
|nltk|3.8.1|
|nni|2.10.1|
|**notebookutils**|**3.4.1-20240110.4 --> 3.4.1-20240309.2**|
|nspr|4.35|
|nss|3.94|
|numba|0.57.1|
|numpy|1.24.3|
|numpy-base|1.24.3|
|oauthlib|3.2.2|
|onnxruntime|1.16.1|
|openai|0.27.8|
|openjpeg|2.5.0|
|openpyxl|3.1.2|
|openssl|3.1.4|
|opt-einsum|3.3.0|
|opt_einsum|3.3.0|
|optuna|2.8.0|
|orc|1.9.0|
|overrides|7.4.0|
|packaging|23.2|
|pandas|2.0.3|
|pandas-stubs|2.1.1.230928|
|pandasql|0.7.3|
|pandocfilters|1.5.0|
|pango|1.50.14|
|paramiko|3.3.1|
|parso|0.8.3|
|pathos|0.3.1|
|pathtools|0.1.2|
|patsy|0.5.3|
|pbr|5.11.1|
|pcre2|10.40|
|pexpect|4.8.0|
|pickleshare|0.7.5|
|pillow|10.0.1|
|pip|23.1.2|
|pixman|0.42.2|
|pkgutil-resolve-name|1.3.10|
|platformdirs|3.5.1|
|plotly|5.16.1|
|ply|3.11|
|pooch|1.8.0|
|portalocker|2.8.2|
|posthog|3.0.2|
|powerbiclient|3.1.1|
|pox|0.3.3|
|ppft|1.7.6.7|
|prettytable|3.8.0|
|prometheus_client|0.17.1|
|prompt-toolkit|3.0.39|
|prompt_toolkit|3.0.39|
|protobuf|4.21.12|
|psutil|5.9.5|
|pthread-stubs|0.4|
|ptyprocess|0.7.0|
|pulsar-client|3.3.0|
|pulseaudio-client|16.1|
|pure_eval|0.2.2|
|py-xgboost|1.7.6|
|py4j|0.10.9.7|
|pyarrow|12.0.1|
|pyasn1|0.5.0|
|pyasn1-modules|0.3.0|
|pycosat|0.6.6|
|pycparser|2.21|
|pydantic|1.10.9|
|pygments|2.16.1|
|pyjwt|2.8.0|
|pynacl|1.5.0|
|pyodbc|4.0.39|
|pyopenssl|23.2.0|
|pyparsing|3.0.9|
|pyperclip|1.8.2|
|pypika|0.48.9|
|pyqt|5.15.9|
|pyqt5-sip|12.12.2|
|pysocks|1.7.1|
|pyspark|3.4.1.5.3.20230713|
|python|3.10.12|
|python-dateutil|2.8.2|
|python-fastjsonschema|2.18.1|
|python-flatbuffers|23.5.26|
|python-graphviz|0.20.1|
|python-json-logger|2.0.7|
|python-tzdata|2023.3|
|python-xxhash|3.4.1|
|python_abi|3.10|
|pythonnet|3.0.1|
|pythonwebhdfs|0.2.3|
|pytorch|2.0.1|
|pytorch-mutex|1.0|
|pytz|2023.3.post1|
|pyu2f|0.1.5|
|pywin32-on-windows|0.1.0|
|pyyaml|6.0.1|
|pyzmq|25.1.1|
|qt-main|5.15.8|
|rdma-core|28.9|
|re2|2023.03.02|
|readline|8.2|
|referencing|0.30.2|
|regex|2023.8.8|
|requests|2.31.0|
|requests-oauthlib|1.3.1|
|responses|0.23.3|
|retrying|1.3.3|
|rfc3339-validator|0.1.4|
|rfc3986-validator|0.1.1|
|rich|13.6.0|
|rouge-score|0.1.2|
|rpds-py|0.10.6|
|rsa|4.9|
|ruamel.yaml|0.17.32|
|ruamel.yaml.clib|0.2.7|
|ruamel_yaml|0.15.80|
|s2n|1.3.49|
|sacremoses|0.0.53|
|salib|1.4.7|
|schema|0.7.5|
|scikit-learn|1.3.0|
|scipy|1.10.1|
|seaborn|0.12.2|
|seaborn-base|0.12.2|
|**semantic-link-sempy**|**0.6.0**|
|send2trash|1.8.2|
|sentence-transformers|2.0.0|
|sentry-sdk|1.32.0|
|seqeval|1.2.2|
|setproctitle|1.3.3|
|setuptools|68.2.2|
|shap|0.42.1|
|shellingham|1.5.4|
|simplejson|3.19.2|
|sip|6.7.12|
|six|1.16.0|
|slicer|0.0.7|
|smmap|5.0.0|
|snappy|1.1.10|
|sniffio|1.3.0|
|soupsieve|2.5|
|sqlalchemy|2.0.22|
|sqlanalyticsconnectorpy|1.0.1|
|sqlparse|0.4.4|
|stack_data|0.6.2|
|starlette|0.27.0|
|statsmodels|0.14.0|
|stevedore|5.1.0|
|sympy|1.12|
|synapseml-cognitive|1.0.2|
|synapseml-core|1.0.2|
|synapseml-deep-learning|1.0.2|
|synapseml-internal|1.0.2.1.dev1|
|synapseml-lightgbm|1.0.2|
|synapseml-mlflow|1.0.23|
|synapseml-opencv|1.0.2|
|synapseml-utils|1.0.19.post1|
|synapseml-vw|1.0.2|
|tabulate|0.9.0|
|tbb|2021.10.0|
|tenacity|8.2.3|
|tensorboard|2.12.3|
|tensorboard-data-server|0.7.0|
|tensorflow|2.12.1|
|tensorflow-base|2.12.1|
|tensorflow-estimator|2.12.1|
|termcolor|2.3.0|
|terminado|0.17.1|
|threadpoolctl|3.2.0|
|tiktoken|0.5.1|
|tinycss2|1.2.1|
|tk|8.6.13|
|tokenizers|0.13.3|
|toml|0.10.2|
|tomli|2.0.1|
|toolz|0.12.0|
|tornado|6.3.3|
|tqdm|4.66.1|
|traitlets|5.12.0|
|transformers|4.26.0|
|treeinterpreter|0.2.2|
|typed-ast|1.5.5|
|typeguard|2.13.3|
|typer|0.9.0|
|types-python-dateutil|2.8.19.14|
|types-pytz|2023.3.1.1|
|types-pyyaml|6.0.12.12|
|typing-extensions|4.8.0|
|typing_extensions|4.5.0|
|typing_utils|0.1.0|
|tzdata|2023c|
|ucx|1.14.1|
|unicodedata2|15.1.0|
|unixodbc|2.3.12|
|uri-template|1.3.0|
|urllib3|1.26.17|
|uvicorn|0.23.2|
|virtualenv|20.23.1|
|wandb|0.15.12|
|wcwidth|0.2.8|
|webcolors|1.13|
|webencodings|0.5.1|
|websocket-client|1.6.4|
|websockets|12.0|
|werkzeug|3.0.1|
|wheel|0.41.2|
|widgetsnbextension|4.0.9|
|wolframalpha|5.0.0|
|wrapt|1.15.0|
|xcb-util|0.4.0|
|xcb-util-image|0.4.0|
|xcb-util-keysyms|0.4.0|
|xcb-util-renderutil|0.3.9|
|xcb-util-wm|0.4.1|
|xgboost|1.7.6|
|xkeyboard-config|2.40|
|xmltodict|0.13.0|
|xorg-kbproto|1.0.7|
|xorg-libice|1.1.1|
|xorg-libsm|1.2.4|
|xorg-libx11|1.8.7|
|xorg-libxau|1.0.11|
|xorg-libxdmcp|1.1.3|
|xorg-libxext|1.3.4|
|xorg-libxrender|0.9.11|
|xorg-renderproto|0.11.1|
|xorg-xextproto|7.3.0|
|xorg-xf86vidmodeproto|2.3.1|
|xorg-xproto|7.0.31|
|xxhash|0.8.2|
|xz|5.2.6|
|yaml|0.2.5|
|yarl|1.9.2|
|zeromq|4.3.5|
|zipp|3.17.0|
|zlib|1.2.13|
|zope.event|5.0|
|zope.interface|6.1|
|zstandard|0.21.0|
|zstd|1.5.5|
|_libgcc_mutex|0.1|

# Java and Scala Libraries

|Name|Version|
|-----|-----|
|HikariCP|2.5.1|
|JLargeArrays|1.5|
|JTransforms|3.1|
|RoaringBitmap|0.9.38|
|ST4|4.0.4|
|SparkCustomEvents|3.4.0-1.0.0|
|**SparkCustomEvents**|**3.4.0-1.0.0 --> 3.4.0-1.0.1**|
|**TokenLibrary-assembly**|**4.0.0 --> 4.0.3**|
|VegasConnector|3.4.08|
|activation|1.1.1|
|aircompressor|0.21|
|algebra|2.12-2.0.1|
|aliyun-java-sdk-core|4.5.10|
|aliyun-java-sdk-kms|2.11.0|
|aliyun-java-sdk-ram|3.1.0|
|aliyun-sdk-oss|3.13.0|
|annotations|7.0.0|
|antlr-runtime|3.5.2|
|antlr4-runtime|4.9.3|
|aopalliance-repackaged|2.6.1|
|apiguardian-api|1.1.0|
|arpack|3.0.3|
|arpack_combined_all|0.1|
|arrow-format|1.0.0|
|arrow-memory-core|1.0.0|
|arrow-memory-netty|1.0.0|
|arrow-vector|1.0.0|
|audience-annotations|0.5.0|
|**autotune-client**|**2.12-1.10.0-3.4-117562362 --> 2.12-1.11.0-3.4-120040110**|
|**autotune-common**|**2.12-1.10.0-3.4-117562362 --> 2.12-1.11.0-3.4-120040110**|
|avro|1.11.3|
|avro-ipc|1.11.3|
|avro-mapred|1.11.3|
|aws-java-sdk-bundle|1.12.262|
|azure-data-lake-store-sdk|2.3.9|
|azure-eventhubs|3.3.0|
|azure-eventhubs-spark|2.12-2.3.22|
|azure-keyvault-core|1.0.0|
|azure-storage|7.0.1|
|azure-synapse-ml-pandas|2.12-0.1.1|
|azure-synapse-ml-predict|2.12-1.0|
|blas|3.0.3|
|bonecp|0.8.0.RELEASE|
|breeze|2.12-2.1.0|
|breeze-macros|2.12-2.1.0|
|cats-kernel|2.12-2.1.1|
|chill|2.12-0.10.0|
|chill-java|0.10.0|
|client-sdk|1.24.1|
|commons-cli|1.5.0|
|commons-codec|1.15|
|commons-collections|3.2.2|
|commons-collections4|4.4|
|commons-compiler|3.1.9|
|commons-compress|1.22|
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
|compress-lzf|1.1.2|
|config|1.3.4|
|cosmos-analytics-spark|3.4.1-connector-1.8.10|
|curator-client|2.13.0|
|curator-framework|2.13.0|
|curator-recipes|2.13.0|
|datanucleus-api-jdo|4.2.4|
|datanucleus-core|4.1.17|
|datanucleus-rdbms|4.1.19|
|delta-core|2.12-2.4.0.9|
|delta-iceberg|2.12-2.4.0.9|
|delta-storage|2.4.0.9|
|derby|0.14.2.0|
|dropwizard-metrics-hadoop-metrics2-reporter|0.1.2|
|flatbuffers-java|1.12.0|
|fluent-logger|0.3.4-jar-with-dependencies-provided|
|gcs-connector-hadoop3|2.2.11-shaded|
|genesis-client|2.12-0.28.0-jar-with-dependencies|
|gluten-velox-bundle-spark|3.4_2.12-mariner_2.0-1.2.0-SNAPSHOT|
|gson|2.8.9|
|guava|4.0.1|
|**hadoop-aliyun**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-annotations**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-aws**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-azure**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-azure-datalake**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|hadoop-azureml|1.0-fs|
|**hadoop-client-api**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-client-runtime**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-cloud-storage**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hadoop-openstack**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|hadoop-shaded-guava|1.1.1|
|**hadoop-yarn-server-web-proxy**|**3.3.4.5.3-117503204 --> 3.3.4.5.3-121327941**|
|**hdinsight-spark-metrics**|**3.4.0-1.0.0 --> 3.4.0-1.0.1**|
|hive-common|2.3.9|
|hive-exec|2.3.9-core|
|hive-llap-common|2.3.9|
|hive-metastore|2.3.9|
|hive-serde|2.3.9|
|hive-shims|0.23-2.3.9|
|hive-shims|2.3.9|
|hive-shims-common|2.3.9|
|hive-shims-scheduler|2.3.9|
|hive-storage-api|2.8.1|
|hk2-api|2.6.1|
|hk2-locator|2.6.1|
|hk2-utils|2.6.1|
|httpclient|4.5.14|
|httpclient5|5.1.3|
|httpcore|4.4.16|
|httpmime|4.5.14|
|httpmime|4.5.13|
|impulse-core_spark|3.4_2.12-1.0.19|
|impulse-telemetry-mds_spark|3.4_2.12-1.0.19|
|ini4j|0.5.4|
|isolation-forest|3.4.1_2.12-3.0.3|
|istack-commons-runtime|3.0.8|
|ivy|2.5.1|
|jackson-annotations|2.14.2|
|jackson-core|2.14.2|
|jackson-core-asl|1.9.13|
|jackson-databind|2.14.2|
|jackson-dataformat-cbor|2.14.2|
|jackson-datatype-jsr310|2.14.2|
|jackson-mapper-asl|1.9.13|
|jackson-module-scala|2.12-2.14.2|
|jakarta.annotation-api|1.3.5|
|jakarta.inject|2.6.1|
|jakarta.servlet-api|4.0.3|
|jakarta.validation-api|2.0.2|
|jakarta.ws.rs-api|2.1.6|
|jakarta.xml.bind-api|2.3.2|
|janino|3.1.9|
|javassist|3.25.0-GA|
|javatuples|1.2|
|javax.jdo|3.2.0-m3|
|javolution|5.5.1|
|jaxb-api|2.2.11|
|jaxb-runtime|2.3.2|
|jcl-over-slf4j|2.0.6|
|jdo-api|3.0.1|
|jdom2|2.0.6|
|jersey-client|2.36|
|jersey-common|2.36|
|jersey-container-servlet|2.36|
|jersey-container-servlet-core|2.36|
|jersey-hk2|2.36|
|jersey-server|2.36|
|jettison|1.1|
|jetty-util|9.4.53.v20231009|
|jetty-util-ajax|9.4.53.v20231009|
|jline|2.14.6|
|joda-time|2.12.2|
|jodd-core|3.5.2|
|jsch|0.1.54|
|json|1|
|json|3|
|json|1.8|
|json-simple|1.1.1|
|json-simple|1.1|
|json4s-ast|2.12-3.7.0-M11|
|json4s-core|2.12-3.7.0-M11|
|json4s-jackson|2.12-3.7.0-M11|
|json4s-scalap|2.12-3.7.0-M11|
|jsr305|3.0.0|
|jta|1.1|
|jul-to-slf4j|2.0.6|
|junit-jupiter|5.5.2|
|junit-jupiter-api|5.5.2|
|junit-jupiter-engine|5.5.2|
|junit-jupiter-params|5.5.2|
|junit-platform-commons|1.5.2|
|junit-platform-engine|1.5.2|
|kafka-clients|3.3.2|
|kryo-shaded|4.0.2|
|kusto-data|3.2.1-SynapseFabric|
|kusto-ingest|3.2.1-SynapseFabric|
|kusto-spark|3.0_2.12-3.1.16|
|lapack|3.0.3|
|leveldbjni-all|1.8|
|libfb303|0.9.3|
|libthrift|0.12.0|
|lightgbmlib|3.3.510|
|log4j|1.2-api-2.19.0|
|log4j-api|2.19.0|
|log4j-core|2.19.0|
|log4j-slf4j2-impl|2.19.0|
|lz4-java|1.8.0|
|mdsdclientdynamic|2.0|
|metrics-core|4.2.15|
|metrics-graphite|4.2.15|
|metrics-jmx|4.2.15|
|metrics-json|4.2.15|
|metrics-jvm|4.2.15|
|microsoft-catalog-metastore-client|1.1.17|
|microsoft-log4j-etwappender|1.0|
|minlog|1.3.0|
|mlflow-spark|2.6.0|
|mssql-jdbc|8.4.1.jre8|
|mysql-connector-java|8.0.18|
|netty-all|4.1.87.Final|
|netty-buffer|4.1.87.Final|
|netty-codec|4.1.87.Final|
|netty-codec-http|4.1.87.Final|
|netty-codec-http2|4.1.87.Final|
|netty-codec-socks|4.1.87.Final|
|netty-common|4.1.87.Final|
|netty-handler|4.1.87.Final|
|netty-handler-proxy|4.1.87.Final|
|netty-resolver|4.1.87.Final|
|netty-transport|4.1.87.Final|
|netty-transport-classes-epoll|4.1.87.Final|
|netty-transport-classes-kqueue|4.1.87.Final|
|netty-transport-native-epoll|4.1.87.Final-linux-x86_64|
|netty-transport-native-epoll|4.1.87.Final-linux-aarch_64|
|netty-transport-native-kqueue|4.1.87.Final-osx-aarch_64|
|netty-transport-native-kqueue|4.1.87.Final-osx-x86_64|
|netty-transport-native-unix-common|4.1.87.Final|
|**notebook-utils**|**3.4.1-20240110.4 --> 3.4.1-20240309.2**|
|objenesis|3.2|
|onnx-protobuf|2.12-0.9.3|
|onnxruntime_gpu|1.8.1|
|opencsv|2.3|
|opencv|3.2.0-1|
|opentest4j|1.2.0|
|opentracing-api|0.33.0|
|opentracing-noop|0.33.0|
|opentracing-util|0.33.0|
|orc-core|1.8.4-shaded-protobuf|
|orc-mapreduce|1.8.4-shaded-protobuf|
|orc-shims|1.8.4|
|oro|2.0.8|
|osgi-resource-locator|1.0.3|
|paranamer|2.8|
|parquet-column|1.12.3|
|parquet-common|1.12.3|
|parquet-encoding|1.12.3|
|parquet-format-structures|1.12.3|
|parquet-hadoop|1.12.3|
|parquet-jackson|1.12.3|
|peregrine-spark|3.4.0-0.10.4|
|pickle|1.3|
|postgresql|2.2.9|
|protobuf-java|2.5.0|
|proton-j|0.33.8|
|py4j|0.10.9.7|
|qpid-proton-j-extensions|1.2.4|
|resilience4j-core|1.7.1|
|resilience4j-retry|1.7.1|
|rocksdbjni|7.9.2|
|scala-collection-compat|2.12-2.7.0|
|scala-compiler|2.12.17|
|scala-java8-compat|2.12-0.9.0|
|scala-library|2.12.17|
|scala-parser-combinators|2.12-2.1.1|
|scala-reflect|2.12.17|
|scala-xml|2.12-2.1.0|
|scalactic|2.12-3.2.14|
|shims|0.9.38|
|slf4j-api|2.0.6|
|snappy-java|1.1.10.5|
|spark|3.4-rpc-history-server-app-listener_2.12-1.0.0|
|spark|3.4-rpc-history-server-core_2.12-1.0.0|
|spark|3.4-advisor-core_2.12-1.0.18|
|**spark-avro**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|spark-avro|2.12-3.4.1|
|**spark-catalyst**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-core**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-enhancement**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|spark-enhancementui|2.12-3.3.0|
|**spark-graphx**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-hadoop-cloud**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-hive**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|spark-kusto-synapse-connector|3.1_2.12-1.3.4|
|**spark-kvstore**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-launcher**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|spark-lighter-contract|2.12-2.0.8_spark-3.4.0|
|spark-lighter-core|2.12-2.0.8_spark-3.4.0|
|**spark-microsoft-tools**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-mllib**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-mllib-local**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-network-common**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-network-shuffle**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-repl**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-sketch**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-sql**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-sql-kafka**|**0_2.12-3.4.1.5.3-117503204 --> 0_2.12-3.4.1.5.3-121327941**|
|**spark-streaming**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-streaming-kafka**|**0_2.12-3.4.1.5.3-117503204 --> 0_2.12-3.4.1.5.3-121327941**|
|**spark-streaming-kafka**|**0_2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-tags**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-token-provider-kafka**|**0_2.12-3.4.1.5.3-117503204 --> 0_2.12-3.4.1.5.3-121327941**|
|**spark-unsafe**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark-yarn**|**2.12-3.4.1.5.3-117503204 --> 2.12-3.4.1.5.3-121327941**|
|**spark_diagnostic_cli**|**2.0.6_spark-3.4.1 --> 2.0.7_spark-3.4.1**|
|sparklyr-connector|1.0.0_spark-3.4.1|
|sparknativeparquetwriter|2.12-0.12.1|
|spire|2.12-0.17.0|
|spire-macros|2.12-0.17.0|
|spire-platform|2.12-0.17.0|
|spire-util|2.12-0.17.0|
|spray-json|2.12-1.3.5|
|sqlanalyticsconnector|3.4.1-1.0.0|
|stax-api|1.0.1|
|stream|2.9.6|
|structuredstreamforspark|2.12-3.4.1-2.3.5|
|synapseml|2.12-1.0.2|
|synapseml-cognitive|2.12-1.0.2|
|synapseml-core|2.12-1.0.2|
|synapseml-deep-learning|2.12-1.0.2|
|synapseml-internal|2.12-1.0.2.1-spark3.4|
|synapseml-lightgbm|2.12-1.0.2|
|synapseml-opencv|2.12-1.0.2|
|synapseml-vw|2.12-1.0.2|
|**synfs**|**3.4.1-20240110.4 --> 3.4.1-20240309.2**|
|threeten-extra|1.7.1|
|tink|1.7.0|
|transaction-api|1.1|
|**trident-core**|**1.1.41 --> 1.2.6**|
|tridentsystemtokenlibrary-assembly|1.6.2|
|tridenttokenlibrary-assembly|1.6.2|
|univocity-parsers|2.9.1|
|vavr|0.10.4|
|vavr-match|0.10.4|
|vw-jni|9.3.0|
|wildfly-openssl|1.0.7.Final|
|xbean-asm9-shaded|4.22|
|xz|1.9|
|**zookeeper**|**3.6.3.5.3-117503204 --> 3.6.3.5.3-121327941**|
|**zookeeper-jute**|**3.6.3.5.3-117503204 --> 3.6.3.5.3-121327941**|
|zstd-jni|1.5.2-5|

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
|**XML**|**3.99-0.16 --> 3.99-0.16.1**|
|arrow|12.0.0|
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
|broom.helpers|1.14.0|
|bslib|0.6.1|
|cachem|1.0.8|
|callr|3.7.3|
|caret|6.0-94|
|cellranger|1.1.0|
|class|7.3-22|
|**classInt**|**0.4-10**|
|cli|3.6.2|
|clipr|0.8.0|
|clock|0.7.0|
|codetools|0.2-19|
|collections|0.3.7|
|colorspace|2.1-0|
|**commonmark**|**1.9.0 --> 1.9.1**|
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
|ggplot2|3.4.2|
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
|gtsummary|1.7.2|
|**hardhat**|**1.3.0 --> 1.3.1**|
|haven|2.5.4|
|hexbin|1.28.3|
|highcharter|0.9.4|
|highr|0.10|
|hms|1.1.3|
|htmltools|0.5.7|
|htmlwidgets|1.6.4|
|httpcode|0.3.0|
|**httpuv**|**1.6.13 --> 1.6.14**|
|httr|1.4.7|
|httr2|1.0.0|
|ids|1.0.1|
|**igraph**|**1.5.1 --> 1.6.0**|
|**infer**|**1.0.5 --> 1.0.6**|
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
|labelled|2.12.0|
|later|1.3.2|
|lattice|0.22-5|
|lava|1.7.3|
|lazyeval|0.2.2|
|lhs|1.1.6|
|lifecycle|1.0.4|
|lightgbm|3.3.5|
|**listenv**|**0.9.0 --> 0.9.1**|
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
|**modeldata**|**1.2.0 --> 1.3.0**|
|modelenv|0.1.1|
|modelr|0.1.11|
|munsell|0.5.0|
|nlme|3.1-164|
|nnet|7.3-19|
|**notebookutils**|**3.4.1-20240110.4 --> 3.4.1-20240309.2**|
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
|**pkgload**|**1.3.3 --> 1.3.4**|
|plotly|4.10.2|
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
|**ps**|**1.7.5 --> 1.7.6**|
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
|rmarkdown|2.22|
|**roxygen2**|**7.3.0 --> 7.3.1**|
|rpart|4.1.23|
|rprojroot|2.0.4|
|rsample|1.2.0|
|rstudioapi|0.15.0|
|rversions|2.1.2|
|rvest|1.0.3|
|**s2**|**1.1.6**|
|sass|0.4.8|
|scales|1.3.0|
|selectr|0.4-2|
|sessioninfo|1.2.2|
|**sf**|**1.0-15**|
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
|tidymodels|1.1.0|
|**tidyr**|**1.3.0 --> 1.3.1**|
|tidyselect|1.2.0|
|tidyverse|2.0.0|
|timeDate|4032.109|
|**timechange**|**0.2.0 --> 0.3.0**|
|tinytex|0.49|
|tools|4.2.3|
|torch|0.11.0|
|triebeard|0.4.1|
|tune|1.1.2|
|tzdb|0.4.0|
|**units**|**0.8-5**|
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
|**withr**|**2.5.2 --> 3.0.0**|
|**wk**|**0.9.1**|
|workflows|1.1.3|
|workflowsets|1.0.1|
|xfun|0.41|
|xgboost|1.7.4.1|
|xml2|1.3.6|
|xopen|1.0.0|
|xtable|1.8-4|
|**xts**|**0.13.1 --> 0.13.2**|
|yaml|2.3.8|
|**yardstick**|**1.2.0 --> 1.3.0**|
|**zip**|**2.3.0 --> 2.3.1**|
|zoo|1.8-12|

