# Configure Autoplay Countdown

Unlike the other topics, this topic two different pieces of documentation
1. The API Reference section is the content that would be present in the Interfaces Guide. 
1. The Example: Autoplay Countdowm 

## API Reference 

## Example: Autoplay Countdown

```
---
  swagger: "2.0"
  info: 
    version: "1.0.0"
    title: "Swagger Autoplay API"
    description: >
      This documentation describes the endpoints that can be used to XXX
  host: "auto.swagger.io"
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
      description: Sets countdown period for autoplay in seconds.
      operationId: autoplayCountdown
      parameters:
        - name: countdown
          in: path
          description: Time, in seconds, that the countdown between a video ending and the next starting should last for. 
          required: true
          type: integer
          format: int64
      responses:
       ...
```

## ?? 

* Document Type: Interfaces Guide
* This document complements an annotated API information, for example,  
* This content re-uses the description of what auto-play actually is from the User Materials. 
