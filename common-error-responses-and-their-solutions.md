# Common Error Responses and their solutions

## 400 Bad Request

- `invalid_parameters`: The request contains invalid or missing parameters.

- `invalid_amount`: The specified top-up amount is not valid.

- `invalid_type`: The specified type is not supported.

- `invalid_recurrence`: The specified recurrence type is not valid.

- `invalid_source`: The selected incentive source is not supported.

- `user_not_found`: The user ID specified in the request does not exist.

## 401 Unauthorized

`authentication_failed`: The user's authentication has failed.

## 403 Forbidden

`forbidden_action`: The user is not authorized to get incentive.

## 404 Not Found

`source_not_found`: The selected docs-in source is not found or not available.

## 405 Method Not Allowed

`method_not_allowed`: The HTTP method used is not allowed for this endpoint.

## 422 Unprocessable Entity

`top-up_failed`: The top-up could not be processed.

## 429 Too Many Requests

`rate_limit_exceeded`: The rate limit for making incentive requests has been exceeded.

## 500 Internal Server Error

`internal_server_error`: An unexpected error occurred on the server.
