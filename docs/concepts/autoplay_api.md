# Configure Autoplay Countdown

Unlike the other topics, this contains two different pieces of documentation
1. The *API Reference section* should be present in the Interfaces Guide. It points the reader to the Swagger file itself. 
1. The *Example: Autoplay Countdowm* is a snippet showing the annotations that I would add to the Swagger file (API contract). In this case, I've shown some descriptions that I would add to a Swagger file. (See `description:`.)

## API Reference 

The REST API for this component is described following the open API Specification (or Swagger Specification). You can find the Open API file (a YAML file) that describes your entire API (endpoints, parameters, authentication methods and document metadata), at the location:

https://&lt;host&gt;:&lt;port&gt;/Service/ 

**Note:** You can use the **Try it Out** button for each of the endpoints, but be aware that you are actually hitting the endpoint.  
  
*In a real topic, you would need to replace the &lt;host&gt; and &lt;port&gt; values with the appropriate values, and the file at that location would look something like this: [http://petstore.swagger.io/](http://petstore.swagger.io/). 

## Example: Autoplay Countdown

```
---
  swagger: "2.0"
  info: 
    version: "1.0.0"
    title: "Swagger Autoplay API"
    description: >
      This documentation describes the endpoints that are associated with the Autoplay functionality. 
      Autoplay allows the next video on your Up Next list to start automatically in your player, after a countdown is complete.
      Autoplay is enabled by default when viewed in a standard browser on a PC or handheld device. 
      Autoplay can be turned off manually by the user. 
      Autoplay will not start the next video if the device has been inactive on the mobile network for a period of 30 minutes, or on WIKI for 4 hours. 
  host: "autoplay.swagger.io"
  basePath: "/api"
  schemes: 
    - "http"
  consumes: 
    - "application/json"
  produces: 
    - "application/json"
  paths: 
    /autoplay/{countdown}: 
     post:
      description: > 
        This endpoint sets the countdown period for autoplay in seconds.
        This is the time window between the last video ending and the next one starting. 
        This value is only used if autoplay is enabled on the given device. 
      operationId: autoplayCountdown
      parameters:
        - name: countdown
          in: path
          description: > 
            Time period, in seconds, for the countdown between one video ending and the next one starting. 
            We recommend a countdown of 10 seconds, but suggest that you should set a maximum delay of 30 seconds. 
            0 indicates that there should be no countdown between the two videos. 
          required: true
          type: integer
          format: int64
      responses:
       ...
```

## Additional Items and Comments

* Document Type: Interfaces Guide
* This document complements an annotated API information, for example,  
* This content re-uses the description of what auto-play actually is from the User Materials. 
