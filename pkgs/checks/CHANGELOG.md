# 0.2.1-dev

# 0.2.0

-   **Breaking Changes**
    -   `checkThat` renamed to `check`.
    -   `nest` and `nestAsync` take `Iterable<String> Function()` arguments for
        `label` instead of `String`.
    -   Async expectation extensions `completes`, `throws`, `emits`, and
        `emitsError` no longer return a `Future<Subject>`. Instead they take an
        optional `Condition` argument which can check expectations that would
        have been checked on the returned subject.
    -   `nestAsync` no longer returns a `Subject`, callers must pass the
        followup `Condition` to the nullable argument.
    -   Remove the `which` extension on `Future<Subject>`.
    -   `matches` renamed to `matchesPattern` and now accepts a `Pattern`
        argument, instead of limiting to `RegExp`.
-   Added an example.
-   Include a stack trace in the failure description for unexpected errors from
    Futures or Streams.

# 0.1.0

-   Initial release.
