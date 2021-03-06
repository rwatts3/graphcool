---
alias: bee4oodood
description: An overview of Graphcool's authentication system.
---

# Overview

Graphcool offers a very flexible authentication system that's based on [serverless functions](!alias-aiw4aimie9).

In general, Graphcool allows you to specify that some of your available API operations should require authentication. This effectively that means the HTTP request that's carrying the operation needs to have a valid [authentication token](!alias-eip7ahqu5o) in its `Authorization` header. If that's not the case, the request will fail with a permission error.

If you want to authenticate requests from your users, you need to generate a token for them. A token always needs to be associated with one particular node from your database.

Tokens are generated inside [`resolver` functions](!alias-su6wu3yoo2). If you want to implement authentication, you first need to setup a corresponding `resolver` in your project that returns an authentication token.

In order to get started quickly with authentication, you can use one of the existing [authentication modules](https://github.com/graphcool/modules/tree/master/authentication).

To learn how to implement authentication with React & Apollo on the frontend, check out the corresponding guides: [email-password-authencation](!alias-cu3jah9ech) and [facebook-login](!alias-yi9jeuwohl).
