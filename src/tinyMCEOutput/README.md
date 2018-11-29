### Instructions

1. Upload 'blackboardXSSPayload.html' to some host that accepts .js files (github gists will work just fine)

2. Take the url where you just uploaded 'blackboardXSSPayload.html' to and insert it into the second link tag 'href' attribute of the 'tinyMCEContextFile.html'

3. Upload 'tinyMCEContextFile.html' to somewhere in your blackboard content collection and set the file to publicly viewable.

4. Click the uploaded 'tinyMCEContextFile.html' you just uploaded and copy the url it brings you to, save that url for a second.

5. Copy that url into the 'entryContent.html' file as the value for the "data" attribute on the "object" tag.

6. Find a place on blackboard where you can make a post with the tinyMCE Editor that other people will visit to view the post.

7. Open the post/journal entry/whatever tinyMCE Editor, expand the toolbar, click 'html' and paste the html from the 'entryContent.html' file, then press 'save' or whatever it is.

8. Public the content and when users view it the XSS Payload will run in the context of their user. Since it is only currently logging the student's ID to the console it's harmless.
