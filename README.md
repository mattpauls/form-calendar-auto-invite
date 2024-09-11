# Automatically send Google Calendar event invite from RSVP Google Form

Automatically send a Google Calendar event invite when someone registers/RSVPs using a Google Form.

## Setup

1. Create a new Google Calendar event for your regional group meeting with all the details you'd like.
   a. Ensure that the title of your event is unique in your Google Calendar. One suggestion is to add the year and month to the end of the event to make it easy to identify, like "CITE Regional Group Meeting 2024.09".
2. Copy or create a Google RSVP Form ([our template is here](https://docs.google.com/forms/d/1E4hfXTtIQUVu9rUqPS2vfu8-kndwxxPMBD_-j7CzMb4/template/preview) if you'd like to use it).
   a. If you are not using our template, ensure that there is a field titled "Email Address" or that you are collecting email addresses through the form's built-in feature.
3. In the Google Form, click **Responses -> Link** to Sheets and create a new spreadsheet.
4. In the linked spreadsheet, click **Extensions -> Apps Script**.
5. Copy/paste all the code from the _Code.gs_ file into the _Code.gs_ file that pops up, and modify the variables to match your form and Google Calendar event:
   a. FORM_ID - copy/paste the ID of the Google Form from the URL bar
   b. EVENT_TITLE - copy/paste the title of your Google Calendar event here
6. In the Google Apps Script window, click **Project Settings**, and tick the box to _Show "appsscript.json" manifest file in editor_
7. Click on **Editor**, and copy/paste the code from the _appsscript.json_ into the appsscript.json file.
8. Click on Code.gs, then ensure the _setup_ function is selected, then click run and allow any permissions that are requested.
9. At this point, everything should be set up, but I would recommend running a test to ensure it works expected.

Original Walkthrough and code [here](https://medium.com/@stephane.giron/manage-event-registration-with-apps-script-google-calendar-and-google-forms-745ba49dffec)
