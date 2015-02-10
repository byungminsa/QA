<h3>Adding a Device: </h3>
<ul>
<li>Go to developer.apple.com</li>
<li>Click Member Center (top right)</li>
<li>Click Certificates and Identifiers</li>
<li>Click Devices (under iOS Apps)</li>
<li>Click the “+” button to add a device</li>
<li>Enter the name with the following Format <COMPANY> <PERSON’S NAME> <DEVICE TYPE></li>
<li>Copy and paste the UDID from the users testflight information</li>
<li>Click Continue</li>
<li>Click Register</li>
</ul>
 
<h3>Updating Apple’s Provisioning Profile:</h3>
<ul>
<li>Back to the Certificates and Identifiers page</li>
<li>Click Development under Provisioning Profiles</li>
<li>Select the Development profile used for Testflight builds (you may need to ask your developer which one to use, 
but as a rule of thumb it wont be one of the ones that says “Active (Managed by Xcode))</li>
<li>Click Edit</li>
<li>Select the check box for the device(s) you just added</li>
<li>Click Generate</li>
<li>Let your developer know that you updated the Provisioning Profile so they can get the new one before making any new 
builds. This will allow you to ignore the following steps for future builds 
(as long as you aren’t adding more devices to a already available build)</li>
</ul>


<h3>Updating an Existing Testflight build to include the new devices:</h3>
<ul>
<li>Download the provisioning profile you just edited in the previous step</li>
<li>Go to the newest build on testflight for the app you want to update</li>
<li>Go to Permissions (left side)</li>
<li>Click Update Profile>></li>
<li>Choose the file you just downloaded from Apple</li>
<li>Click Upload</li>
<li>You should now see the person(s) you just added show up under the “Teammates in the provisioning profile” section</li>
<li>Select the user(s) and then scroll all the way down to “Update & Notify” and press it.</li>
</ul>
