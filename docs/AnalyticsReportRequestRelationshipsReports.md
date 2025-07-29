# AnalyticsReportRequestRelationshipsReports


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AnalyticsReportRequestRelationshipsReportsDataInner]**](AnalyticsReportRequestRelationshipsReportsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_request_relationships_reports import AnalyticsReportRequestRelationshipsReports

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequestRelationshipsReports from a JSON string
analytics_report_request_relationships_reports_instance = AnalyticsReportRequestRelationshipsReports.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequestRelationshipsReports.to_json())

# convert the object into a dict
analytics_report_request_relationships_reports_dict = analytics_report_request_relationships_reports_instance.to_dict()
# create an instance of AnalyticsReportRequestRelationshipsReports from a dict
analytics_report_request_relationships_reports_from_dict = AnalyticsReportRequestRelationshipsReports.from_dict(analytics_report_request_relationships_reports_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


