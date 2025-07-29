# AnalyticsReportRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instances** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_relationships import AnalyticsReportRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRelationships from a JSON string
analytics_report_relationships_instance = AnalyticsReportRelationships.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRelationships.to_json())

# convert the object into a dict
analytics_report_relationships_dict = analytics_report_relationships_instance.to_dict()
# create an instance of AnalyticsReportRelationships from a dict
analytics_report_relationships_from_dict = AnalyticsReportRelationships.from_dict(analytics_report_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


