<h1 align="center">Renderprime</h1>

A fast and serverless prerenderer built as a GCP _[Cloud Function](https://cloud.google.com/functions?hl=en)_.

# Environment Variables

`USER_AGENT`: The `navigator.userAgent` string that will be injected to the browser during rendering (default: `Prerender`).

`WAIT_AFTER_LAST_REQUEST`: The number of milliseconds to wait after the last request before snapshotting the DOM. This has tight correlation to the CPU power (default: `200`).

`WAIT_AFTER_LAST_REQUEST_TIMEOUT`: For how many milliseconds should the browser wait for the last request to return before giving up and snapshotting the DOM anyway (default: `5000`).

# Recommended Function Setup

`Memory allocated`: 1GB
`CPU`: 1
`Maximum concurrent requests per instance`: 1
