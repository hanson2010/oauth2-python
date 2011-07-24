OAuth 2.0 Python module

Usage:
1) Prepare 5 variables;
   Authorization endpoint uri
   Token endpoint uri
   Client ID
   Client secret
   Redirect URI
2) To authenticate a user, redirect the user to get_authorization_uri();
3) If successful, the OAuth provider will redirect the user back to "Redirect URI" with a variable "code" in the GET parameter;
4) Call get_access_token(code), which sends another request to the OAuth provider in REST style. Access token is included in the returned dictionary if successful.

OAuth 2.0 doc
http://oauth.net/2/
