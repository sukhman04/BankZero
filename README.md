# BankZero

Connect BankZero with an Auth0 database so people can sign in with a username and password.

## Acceptance criteria

The proof of concept meets this spec when each check below can be shown:

1. A new user can sign up with a username and password stored in the Auth0 database connection.
2. A user who already signed up can sign in again with that same username and password.
3. The Auth0 Lock sign-in screen is customized so the experience matches the bank's brand. Brand details are still open (see Open questions).
4. A user can sign in with Google.
5. A user can sign in with one additional social provider. Which provider is still open (see Open questions).
6. A whitelist allows sign-in only for email addresses on the named domain. This spec uses `examplewidgets.com`. Replacing that domain is allowed (see Open questions).
7. The Auth0 Authorization extension defines two roles for the demonstration application, each with its own permissions:
   - Employee
   - Manager

   The permission names are still open (see Open questions).
8. Two different users can sign in to the demo application: one assigned the employee role, and one assigned the manager role.
9. For each of those users, the demo shows the authorization information associated with that user, and how an application would read it.

## Open questions

- Which social provider is enabled alongside Google?
- Does the whitelist domain stay `examplewidgets.com`, or is it replaced with another domain?
- Which permissions belong to the employee role, and which belong to the manager role?
- What should the Lock screen use for the bank's brand (colors, logo, copy)? This repository has no brand assets.
