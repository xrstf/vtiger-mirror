== Description on Vulnerability ==

While accepting the company logo we are relaying on the Content-Type and Extension check.
This opens the door for authenticated user to open-attack on the server.

1. We should test for MIME type of received file on server and compare with Content-Type sent by client.
If there is a difference - then act. 
2. Also, review the file-reception against allowed extensions.

This fix should be added to Opensource as well.

== Usage of Patch ==

Patch should be unzipped on the source folder to reflect the bug fix changes.
