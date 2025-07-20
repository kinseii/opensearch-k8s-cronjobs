# Cronjobs for OpenSearch in Kubernetes

## Cronjob `opensearch-cluster-fluent-bit-index-patterns-refresh`

[This cronjob](./index-patterns-refresh.yaml) triggers curl by cron to update all fields in OpenSearch index patterns. This prevents errors from occurring when retrieving identical fields
with different data types. However, it should be noted that such conflicting fields will be excluded from the search.
