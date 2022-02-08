Currently the datatracker stores and retrieves documents (submissions, drafts, charters, minutes, slides, etc.) directly on IETFA's filesystem.
The www.ietf.org website is configured to serve from many of the locations these documents are stored.

This makes separating the datatracker and the website more difficult than it should be, and makes running multiple copies of the datatracker even harder.

One path forward that we are considering is having the documents live in blobs, at a service like amazon's or on our own. Applications like the datatracker and the website can be given access tokens to the blobs with read/write permissions as make sense for the application.
