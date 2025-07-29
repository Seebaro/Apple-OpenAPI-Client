# AppsBetaTesterUsagesV1MetricResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppsBetaTesterUsagesV1MetricResponseDataInner]**](AppsBetaTesterUsagesV1MetricResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**included** | [**List[BetaTester]**](BetaTester.md) |  | [optional] 

## Example

```python
from openapi_client.models.apps_beta_tester_usages_v1_metric_response import AppsBetaTesterUsagesV1MetricResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppsBetaTesterUsagesV1MetricResponse from a JSON string
apps_beta_tester_usages_v1_metric_response_instance = AppsBetaTesterUsagesV1MetricResponse.from_json(json)
# print the JSON string representation of the object
print(AppsBetaTesterUsagesV1MetricResponse.to_json())

# convert the object into a dict
apps_beta_tester_usages_v1_metric_response_dict = apps_beta_tester_usages_v1_metric_response_instance.to_dict()
# create an instance of AppsBetaTesterUsagesV1MetricResponse from a dict
apps_beta_tester_usages_v1_metric_response_from_dict = AppsBetaTesterUsagesV1MetricResponse.from_dict(apps_beta_tester_usages_v1_metric_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


