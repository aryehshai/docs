---
title: Logout
overview: |
  Logs a user out immediately, and
  performs a redirect.
parameters:
  -
    name: redirect
    type: string
    description: >
      Where the user should be redirected
      after logging out. Defaults to the home
      page.
id: 3604bfe9-89be-42af-8163-4b378279026a
---

## Example {#example}

```
{{ if should_logout_for_whatever_reason }}
  {{ user:logout redirect="/somewhere" }}
{{ /if }}
```

This will immediately log a user out and redirect to `/somewhere` if the condition is met.

If you'd like to just output a link, use the [`user:logout_url`](/docs/tags/user-logout_url) tag.
