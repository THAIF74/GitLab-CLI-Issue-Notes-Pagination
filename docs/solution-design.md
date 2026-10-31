# Solution Design
The contribution uses the project's shared pagination helper, `gitlab.ScanAndCollect`, to retrieve issue notes across pages.
The implementation also:
- Initializes missing pagination options.
- Applies the default page size when required.
- Starts from page 1 when no starting page is specified.
- Uses a context with a two-minute timeout.
- Passes the context into the API request.
This follows the project's existing pagination approach rather than introducing a separate manual pagination loop.
