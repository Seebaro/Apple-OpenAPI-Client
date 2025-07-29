# CiBuildRunCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**CiBuildRunCreateRequestDataAttributes**](CiBuildRunCreateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**CiBuildRunCreateRequestDataRelationships**](CiBuildRunCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run_create_request_data import CiBuildRunCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunCreateRequestData from a JSON string
ci_build_run_create_request_data_instance = CiBuildRunCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunCreateRequestData.to_json())

# convert the object into a dict
ci_build_run_create_request_data_dict = ci_build_run_create_request_data_instance.to_dict()
# create an instance of CiBuildRunCreateRequestData from a dict
ci_build_run_create_request_data_from_dict = CiBuildRunCreateRequestData.from_dict(ci_build_run_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


