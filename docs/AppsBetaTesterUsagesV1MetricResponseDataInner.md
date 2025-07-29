# AppsBetaTesterUsagesV1MetricResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data_points** | [**AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints**](AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints.md) |  | [optional] 
**dimensions** | [**AppsBetaTesterUsagesV1MetricResponseDataInnerDimensions**](AppsBetaTesterUsagesV1MetricResponseDataInnerDimensions.md) |  | [optional] 

## Example

```python
from openapi_client.models.apps_beta_tester_usages_v1_metric_response_data_inner import AppsBetaTesterUsagesV1MetricResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppsBetaTesterUsagesV1MetricResponseDataInner from a JSON string
apps_beta_tester_usages_v1_metric_response_data_inner_instance = AppsBetaTesterUsagesV1MetricResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(AppsBetaTesterUsagesV1MetricResponseDataInner.to_json())

# convert the object into a dict
apps_beta_tester_usages_v1_metric_response_data_inner_dict = apps_beta_tester_usages_v1_metric_response_data_inner_instance.to_dict()
# create an instance of AppsBetaTesterUsagesV1MetricResponseDataInner from a dict
apps_beta_tester_usages_v1_metric_response_data_inner_from_dict = AppsBetaTesterUsagesV1MetricResponseDataInner.from_dict(apps_beta_tester_usages_v1_metric_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


