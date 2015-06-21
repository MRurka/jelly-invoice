# Jelly Invoice

<a href="http://jekyllrb.com/" target="_blank">Jekyll</a> Based Invoice generator for designer/developer freelancers who want a fully customizable and brandable, efficient solution to generating invoices.


## Launch Jelly
1. Download Jelly
2. `gem install jekyll` (Install Jekyll. If fails, use "sudo gem install jekyll")
3. `cd path/to/jelly/folder`
4. `jekyll serve --watch`
5. Slap the generated sever address in a browser


## Personalize Jelly
- Populate the `_config.yml` file with your info. Changes to the `_config.yml` file require a fresh compile to update (re-do step 3, above).
- Change the `logo.png` image in the img folder.


## Create an invoice
- Create a new file in the `_posts` directory. Name of file must follow format: `YEAR-MONTH-DAY-title.MARKUP`. Example: `2015-05-19-Special-Invoice-AB1234.markup`. See example files in folder.

**Reference list of default configurables for your invoice**
``` yaml
---

layout: hourly _or_ fixed # hourly means the "rate:" AND "hours:" configurables will need values. See them just below.
date: 2015-11-26 # must be YYYY-MM-DD
tags: 2015 # the invoice year
client-username: GoogleInc # must be a valid username found in one of the client profiles. See next section (Create client profiles).

title: Apple Watch iOS Design # title of your invoice
invoice-number: 001-RU-20150412 # however you personally number your invoices.
rate: 125 # Only necessary if the "layout:" value is "hourly" 

item_X: Website Design # Title of the item(s)
hours_X: 12 # Necessary only if the "layout:" value is "hourly"
price_X: 50 # Necessary only if the "layout:" value is "fixed"

---
```

## Create client profiles
What? Why? So you won't have to re-enter client info per invoice. One time deal.
- Create a new `.yml` file in the `_data/clients` directory. See below and example files in folder.
``` yaml
username: googleinc
name: Google Incorporated
billing: "Google Incorporated <br>111 Richmond St W, <br>Toronto, Ontario, <br>Canada, M5H 2G4"
```
