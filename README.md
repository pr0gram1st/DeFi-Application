1) Download Repository Files
2) Download Metamask
	https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn
3) Download Ganache
	https://trufflesuite.com/ganache/
	a. QuickStart -> Etherium -> Choose The first account and press the key button. In the window opened, copy the private key.
	b. Go to MetaMask -> Add Network
		Network Name: Ganache
		New RPC URL: (same as ganache RPC SERVER, you can see it on the top of Ganache app window)
		Chain ID: 1337
		Currency symbol: GNC
	c. Save
	d. MetaMask -> Import Account:
		Select type: Private Key
		Enter your private key string here: <your copied key>
4) Download VsCode
	https://code.visualstudio.com/download
5) Open project in VsCode
6) In terminal(Cmd + ') write 
	npm install
	sudo npm install --g truffle@5.1.39
	truffle compile
	truffle migrate
	npm start
7) To get the reward balance, first stake some tokens, and then run this command in the new terminal window(you should be in the project directory):
	truffle exec scripts/issue-token.js
