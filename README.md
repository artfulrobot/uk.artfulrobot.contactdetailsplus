# ContactDetailsPlus: Adds Photo and Notes to the Contact Details Report.

This extension adds a new report type, "ContactDetailsPlus" which is a direct
copy of the 4.4.2 version of the "Constituent Report (Detail)" report, except:

- it prints the Contact's name (`sort_name`) as a heading between records. This
  is useful, I found, because otherwise it's hard to tell when one contact ends
  and the next one starts.

- it adds two more checkboxes, one for **Photo** and one for **Notes**.

## Photo

Really simple. Outputs the photo if there is one in the main contact fields section.

CSS tames photo size, since CiviCRM just outputs a link to the original image
which could be huge. (This extension does not do anything nice like
thumbnailing.)

## Notes

Adds a notes section (like you get an Activity section etc.) which lists all the
notes on the contact's record.


# Installation

Install and enable the extension. Then it works like a normal report. If you don't
use new reports much you might not realise you need to create a 'report' from a
'report template' before you'll see it in the 'Reports » All Reports' listing
page. To do this choose:  
**Administer Menu » CiviReport » Create New Report from Template**

You'll then see **ContactDetailsPlus** listed. Click the name and you'll see the
usual massive form, now even massiver, with its two extra checkboxes. If after
playing around with the criteria and using the **Preview** button you hit the
**Create Report** button and it will then appear in the All Reports listing.

Use as any normal CiviCRM Report.
