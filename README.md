This project is not done yet, but you can test its main functionnalities. 

Clone the project with :   

git clone -b DeFi https://github.com/CalineB/Training.git  
' npm install react-scripts '  
' npm i '  
  
### 1 - Clone the project
### 2 - Download Metamask and Ganach
 Create a new workspace in Ganach,  
 Use Ganach RPC to connect to Metamask local host  
 Use the address indexted [1] private key to export Ganach account to Metamask testnet  

### 3 - npm install
### 4 - npm install truffle -g
### 5 - truffle compile (in your terminal)
### 6 - truffle migrate (or "truffle migrate --reset" if needed) (in your terminal)
### 7 - Use "truffle test" (in your terminal to run Moch and Chai testing suite)


 run the app with ' npx nodemon '


 _ You can try "truffle console" (in your terminal), to test the development with :
 "tether = await Tether.deployed()"  
 then  
 "tether"  
 also :  
 "tether.name()"  
 or :  
 "tether.address"  
 and so on..._  

 _You can try still in the truffle console :  
 "rwd = await RWD.deployed()"  
 "rwd.address"  
 "rwd.name()"  

_You can fin the list ouf your Ganach workspace with :  
 "accounts = await web3.eth.getAccounts()"  

After setting your tether account with "tether = await Tether.deployed()" if you want to verify any account balance you can as follows :   
"balance = await tether.balanceOf(accounts[1])" (for the balance of the second wallet). 
"balance.toString"  
"convertBalance = web3.utils.fromWei(balance)"  
(the app is programmed to send only to the second account, the first balance being the bank account).  
