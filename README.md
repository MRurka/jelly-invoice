# Jelly Invoice

<a href="http://jekyllrb.com/" target="_blank">Jekyll</a> Based Invoice generator for designer/developer freelancers who want a fully customizable and brandable, efficient solution to generating invoices.


## Launch Jelly
After downloading Jelly, in Terminal, enter:  
1. `gem install jekyll` (Install Jekyll. If fails, use "sudo gem install jekyll")
2. `cd path/to/jelly/folder`
3. `jekyll serve --watch` (Start server and watch for file changes)
4. Slap the generated sever address in a browser (see image for example)


## Personalize Jelly
- Populate the `_config.yml` file with your info. Changes to the `_config.yml` file require a fresh compile to update (re-do step 3, above).
- Change the `logo.png` image in the img folder. 


## Create an invoice
- Create a new file in the `_posts` directory. Name of file must follow format: `YEAR-MONTH-DAY-title.MARKUP`. Example: `2015-05-19-Special-Invoice-AB1234.markup`. See example file.

**Reference list of default configurables for your invoice**
```
layout: hourly _or_ fixed //hourly means the "rate:" AND "hours" configurables will need values. See them just below.
date: 2015-11-26 //must be YYYY-MM-DD
tags: 2015 //the invoice year
client-username: clientX //must be a valid username found in one of the client profiles. See next section (Create client profiles).

title: Apple Watch iOS Design //title of your invoice
invoice-number: 001-RU-20150412 //however you personally number your invoices.
rate: 125 //What your hourly rate is

item_1, item_2, item_3 ... : Title of the items
hours_1, hours_2, hours_3 ... Hours of the item. Necessary if the "layout:" value is "hourly"
price_1, price_2, price_3 ... FIXED price of the item. Include this ONLY if the above `layout:` value is `fixed`
```

## Create client profiles
What? Why? So you won't need to re-enter client info per invoice. One time deal.
- Create a new file in the `_data/clients` directory. File must be `.yml` file type. See example file.
