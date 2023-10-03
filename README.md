# Synapse Spark Runtimes - Release Notes

[Apache Spark pools in Azure Synapse](https://learn.microsoft.com/en-us/azure/synapse-analytics/spark/apache-spark-version-support) use runtimes to tie together essential component versions such as Azure Synapse optimizations, packages, and connectors with a specific Apache Spark version. Each runtime will be upgraded periodically to include new improvements, features, and patches. When you create a serverless Apache Spark pool, you will have the option to select the corresponding Apache Spark version. Based on this, the pool will come pre-installed with the associated runtime components and packages. Azure Synapse Analytics supports multiple runtimes for Apache Spark.

This repo outlines every release of Synapse Spark Runtime, [along with the timetable of their support](https://learn.microsoft.com/en-us/azure/synapse-analytics/spark/runtime-for-apache-spark-lifecycle-and-supportability). Every version of Synapse Spark Runtime is enriched with features designed to augment the efficiency, user experience, and safety in the realm of big data analytics.

The patch policy differs based on the runtime lifecycle stage:
1. Generally Available (GA) runtime: Receive no upgrades on major versions (i.e. 3.x -> 4.x). And will upgrade a minor version (i.e. 3.x -> 3.y) as long as there are no deprecation or regression impacts.
1. Preview runtime: No major version upgrades unless strictly necessary. Minor versions (3.x -> 3.y) will be upgraded to add latest features to a runtime.
1. Long Term Support (LTS) runtime will be patched with security fixes only.
1. End of life announced (EOLA) runtime will not have bug and feature fixes. Security fixes will be backported based on risk assessment.
