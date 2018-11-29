### Instructions: 

1. Upload 'blackboardXSSPayload.html' to some host that accepts .js files (github gists will work just fine)

2. Take the url where you just uploaded 'blackboardXSSPayload.html' to and insert it into the second link tag 'href' attribute of the 'contentCollectionXSSFile.html'

3. Upload 'contentColllectionXSSFile.html' to somewhere in your blackboard content collection and set the file to publicly viewable.

4. Click the uploaded 'contentCollectionXSSFile.html' you just uploaded and copy the url it brings you to, save that url for a second.

5. Encode that url and insert it onto the end of this URL: **https://blackboard.newhaven.edu/webapps/bb-auth-provider-cas-bb_bb60/execute/casLogin?cmd=login&authProviderId=_111_1&redirectUrl=**

6. Send that url to anyone and they will directed to login if they aren't and then the xss will work the magic. Since we are just logging the data we get to the user's browser console it won't do anything malicious. 