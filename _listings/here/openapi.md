swagger: "2.0"
x-collection-name: HERE
x-complete: 1
info:
  title: Weather API
  description: the-here-weather-api-provides-weather-forecasts-and-reports-on-current-weather-conditions-provides-information-on-severe-weather-alerts-provides-information-about-when-the-sun-and-moon-rise-and-set-and-the-phase-of-the-moonthis-example-set-works-with-version-1-2-4-or-higheradditional-information-can-be-found-on-developer-here-comhttpsdeveloper-here-comrestapisdocumentationweather
  version: 1.0.0
host: weather.cit.api.here.com
basePath: /weather/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getlinkinfo.json:
    get:
      summary: Link Information using linkId
      description: "*Request detailed information about a path segment in the routing
        network given a linkid*\n\nLink information can be retrieved using the `getlinkinfo`
        endpoint, by specifying one or more comma separated linkIds using the `linkids`
        parameter. The `linkids` have been generated from a previous request. Note
        that positive direction '+' in link Ids has to be URL encoded.\n  \n  \n\n\n\n*
        **linkids**  `text`\n \\- Link identifiers for which the detailed information
        is being requested.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe
        encoded string used for the authentication of the client application.    You
        must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\-
        A 20 byte Base64 URL-safe encoded string used for the authentication of the
        client application.    You must include an `app_code` with every request."
      operationId: GetlinkinfoJsonGet2
      x-api-path-slug: getlinkinfo-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: linkids
      responses:
        200:
          description: OK
      tags:
      - Link
      - Information
      - Using
      - LinkId