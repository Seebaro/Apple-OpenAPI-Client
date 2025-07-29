# AppBetaFeedbackScreenshotSubmissionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppBetaFeedbackScreenshotSubmissionsLinkagesResponseDataInner]**](AppBetaFeedbackScreenshotSubmissionsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_beta_feedback_screenshot_submissions_linkages_response import AppBetaFeedbackScreenshotSubmissionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppBetaFeedbackScreenshotSubmissionsLinkagesResponse from a JSON string
app_beta_feedback_screenshot_submissions_linkages_response_instance = AppBetaFeedbackScreenshotSubmissionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppBetaFeedbackScreenshotSubmissionsLinkagesResponse.to_json())

# convert the object into a dict
app_beta_feedback_screenshot_submissions_linkages_response_dict = app_beta_feedback_screenshot_submissions_linkages_response_instance.to_dict()
# create an instance of AppBetaFeedbackScreenshotSubmissionsLinkagesResponse from a dict
app_beta_feedback_screenshot_submissions_linkages_response_from_dict = AppBetaFeedbackScreenshotSubmissionsLinkagesResponse.from_dict(app_beta_feedback_screenshot_submissions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


