# Auto-Play Case Study - Suggested Documentation

This case study shows what documentation might look like that describes how to use and configure an auto-play video option. To give an insight into the thought processes applied when creating documentation, it also contains some information about approach, tools and so on.

**Note:** It is worth mentioning, I think, that a sample of writing does not let you see the most important skill of the writer; that is, ensuring that the content is accurate and appropriate. This skill (of understanding and then re-presenting) is undervalued, but is the key to  successful communications.

## Case Study Details

Many video services have an auto-play feature. This enables a user to watch the next episode of the current show (or other relevant piece of content) automatically when the current video ends.

Please document how this feature works with the following conditions in mind:
* There are multiple users of the documentation:
  * Sales representatives who need to know what value the feature will bring to the owner of the service.
  * The service owner who needs to know how the feature will work for consumers.
  * The service operator who needs to know whether it’s possible to configure the feature to achieve desired behavior and how to do so.
  * Developers and testers who need to know how this consumer-level behavior is derived from an API call.
* The solution must cover at least desktop web, mobile native (Android or iOS) and smart TV (any) applications.

### Notes about the Solution

* I have assumed that the functionality will follow YouTube autoplay. 
* I have assumed that content will be single-sourced to be presented in the format that is most applicable to the device in question, and to present information that is applicable to the device being used by default (if there are alternate steps for other device types, they should be hidden by default). 

## Sample Documentation

Type | Link | Notes
--- | --- | --- 
User Guide | [Auto-Play Videos](autoplay.md) | Describes Auto-play functionality, including limitations. Describes how to configure auto-play on and off. Instructions are tabbed to reflect different device types where applicable.
API Guide | [Enable Auto-play Videos](autoplay_api.md) | Describes how to use the API to set auto-play on for a particular user (accompanies code-level documentation, for example in swagger).
Release Information | [New and Modified Features: Auto-Play](autoplay_rn.md) | Notifies the user that the new auto-play feature is available. 

Possible additional documentation requirements: 
* If your tool is re-badged by other companies, you may need to communicate how to make this feature available to the development users at those companies (depending on implementation). 
* You may also need to provide press releases or blogged information about this new feature, to engage customers and drive uptake. 

I think these additional items aren't needed because of the nature of auto-play. 




