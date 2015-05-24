# Jelly Invoice

Jekyll Based Invoicing Software for freelancers who are slightly tech savvy, or simply comfortable with technical instructions.

#### Left to do
- <s>Add PDF Print buttons on Index Page & Single Page</s>
- <s>Sort by Year on Index Page</s>
- Hide / Show invoices by year (jQuery)
- Format + Style actual invoice page (Design virtually complete)
- Create Stylesheet layout for accountants
- Add Paid/Unpaid filter to Invoices
- Optimize current JS mathematical operations
- Optimize current Jekyll custom field loops


### Getting Started
You can watch the walk-through video for beginners or the quicker version for terminal familiar users.

1. Download Jelly, put the Jelly Invoice folder somewhere, and name it something like *MoneyMaker*, or anything you'd like.
2. Open your Terminal App (Mac). **Spotlight search for Terminal, or find it in Applications/Utilities folder.**
3. In the Terminal App, type in `cd path/to/folder` and press `Enter`. **Meaning: If you put *MoneyMaker* in a folder called "Business", on your desktop, you would type `cd Desktop/Business/MoneyMaker`.**
4. Then type `jekyll serve --watch` in Terminal and press `Enter`. **Basic translation: "jekyll serve" means start the server, and "--watch" makes the server watch the files for any changes (new invoices, edits, etc).**


### Personalize your Jelly Invoice
1. Directly inside *MoneyMaker* (whatever your folder name is) you'll find a file called `_config.yml`. Open that in any text editor and input your business info (billing address, business name, etc).
2. Change Logo: replace the `logo.png` file found in the `img` folder.
3. That's it! 


### Inputting Clients
1. Find the `clients` folder in `MoneyMaker/_data/clients`, where you will find an example client file (example-client.yml). Duplicate it, open it and edit it.

### Creating Invoices
