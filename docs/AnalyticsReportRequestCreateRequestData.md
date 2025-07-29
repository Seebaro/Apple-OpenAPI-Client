# AnalyticsReportRequestCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AnalyticsReportRequestCreateRequestDataAttributes**](AnalyticsReportRequestCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.analytics_report_request_create_request_data import AnalyticsReportRequestCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequestCreateRequestData from a JSON string
analytics_report_request_create_request_data_instance = AnalyticsReportRequestCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequestCreateRequestData.to_json())

# convert the object into a dict
analytics_report_request_create_request_data_dict = analytics_report_request_create_request_data_instance.to_dict()
# create an instance of AnalyticsReportRequestCreateRequestData from a dict
analytics_report_request_create_request_data_from_dict = AnalyticsReportRequestCreateRequestData.from_dict(analytics_report_request_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


