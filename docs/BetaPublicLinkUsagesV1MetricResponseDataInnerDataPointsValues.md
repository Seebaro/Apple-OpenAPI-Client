# BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**view_count** | **int** |  | [optional] 
**accepted_count** | **int** |  | [optional] 
**did_not_accept_count** | **int** |  | [optional] 
**did_not_meet_criteria_count** | **int** |  | [optional] 
**not_relevant_ratio** | **float** |  | [optional] 
**not_clear_ratio** | **float** |  | [optional] 
**not_interesting_ratio** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.beta_public_link_usages_v1_metric_response_data_inner_data_points_values import BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues

# TODO update the JSON string below
json = "{}"
# create an instance of BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues from a JSON string
beta_public_link_usages_v1_metric_response_data_inner_data_points_values_instance = BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues.from_json(json)
# print the JSON string representation of the object
print(BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues.to_json())

# convert the object into a dict
beta_public_link_usages_v1_metric_response_data_inner_data_points_values_dict = beta_public_link_usages_v1_metric_response_data_inner_data_points_values_instance.to_dict()
# create an instance of BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues from a dict
beta_public_link_usages_v1_metric_response_data_inner_data_points_values_from_dict = BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues.from_dict(beta_public_link_usages_v1_metric_response_data_inner_data_points_values_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


