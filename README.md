# Ethereal Escrow Buyer Dashboard


## Getting Started
Ethereal Escrow is a static html/css/javascript/ReactJS site and a client-side interface to the ethereal escrow smart contract. No special hosting environment is required as the blockchain itself acts as the escrow database

## Layout of source files

### Public > Index.html
Content of the Dapp is served within the root div. Any content added above this root div will show above the Dapp, like a header. Any content added below will display like a footer.

### src > Index.css
Css file for modifying styles.

### src > BuyerHome.js
The buyer dashboard page you see when visiting https://escr/

### src > SellerHome.js
The seller dashboard page

### src > NewTransactionRS.js
When you click "Initialize new transaction" on the dashboard, the right side changes to this page. This page should be modified if you wish to hardcode your address as the escrow agent or seller.

![newtx](https://user-images.githubusercontent.com/24837709/31051404-cfbd440a-a699-11e7-9c97-0f9134f3cdaf.jpg)

### src > SpecificTx.js
The right side of the dashboard changes to this page when an existing transaction is clicked.
![tx](https://user-images.githubusercontent.com/24837709/31041943-3ef37698-a5d0-11e7-87bc-f15ca9d95e04.jpg)

## Adding your header & footer

Under Public > Index.html, the Dapp is rendered within the root div. Custom header and footers can be added above and below this div.


## Hardcoding Escrow Agent address
If you look to be the escrow agent for your site (example: Real estate agents, classified sites), you can remove the escrow agent input field and hardcode your address as the escrow agent.

To do this, 

1) Open Source Files > src > NewTransactionRS.js.

2) Hardcode your address. In line 306, replace this.state.escrowAddress with your own address as follows:
![Orignal](https://user-images.githubusercontent.com/24837709/32013863-fb55a59a-b9ee-11e7-867b-437a1f67526f.png)

![New](https://user-images.githubusercontent.com/24837709/32013861-fb290e9a-b9ee-11e7-8754-fa4f7cdca610.png)

3) Remove the Escrow Address input field

Line 425 to 434 and 368 to 377 contains the Escrow Address input field. Remove both of them.

![Remove](https://user-images.githubusercontent.com/24837709/32030707-6ec46738-ba2f-11e7-8fe3-5dd84c7a6181.png)

4) Your address will then be the Escrow Agent for all transactions on your site.

## Further questions
If you need assistance integrating/modifying EsrowMyEther for your site, feel free to raise a github issue or contact me at escrowmyether[at]gmail[dot]com.

## Authors

Cheung Ka Yin 
escrowmyether[at]gmail[dot]com

