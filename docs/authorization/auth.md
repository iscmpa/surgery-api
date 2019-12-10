---
tags: [login, access token, authentication]
---

# Get Access Token

This API follows the standard protocol OAuth2 for authentication.
For more information on how to generate an access token see: [OAuth2 - Client Credentials](https://www.oauth.com/oauth2-servers/access-tokens/client-credentials/)

The `client_id` and `client_secret` will be provides by the ISCMPA.

OAuth2 Token URL: https://megical.santacasa.org.br/oauth/token

<!--
type: tab
title: Schema
-->

```json json_schema
{
  "title": "Auth",
  "type": "object",
  "properties": {
    "grant_type": {
      "type": "string",
      "description": "client_credentials"
    },
    "client_id": {
      "type": "string",
    },
    "client_secret": {
      "type": "string"
    }    
  },
  "required": [
    "grant_type",
    "client_id",
    "client_secret"
  ]
}
```

<!--
type: tab
title: Example
-->

```json
{
    "grant_type": "client_credentials",
    "client_id": "88df2445-...-y456jjd5567d",
    "client_secret": "sdfkj22FDG...689KJDs234o"
}
```

<!-- type: tab-end -->