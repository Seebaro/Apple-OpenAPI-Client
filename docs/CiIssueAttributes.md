# CiIssueAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**issue_type** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**file_source** | [**FileLocation**](FileLocation.md) |  | [optional] 
**category** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_issue_attributes import CiIssueAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiIssueAttributes from a JSON string
ci_issue_attributes_instance = CiIssueAttributes.from_json(json)
# print the JSON string representation of the object
print(CiIssueAttributes.to_json())

# convert the object into a dict
ci_issue_attributes_dict = ci_issue_attributes_instance.to_dict()
# create an instance of CiIssueAttributes from a dict
ci_issue_attributes_from_dict = CiIssueAttributes.from_dict(ci_issue_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


