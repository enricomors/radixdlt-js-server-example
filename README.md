# radixdlt-js-server-example
An example server using Express.js

Install dependencies using `npm install` or `yarn install`

Start the server by running `npm run serve` or `yarn serve`

The default port is set to 3000

The server will generate a new address on each startup

After running the server, you can see your address by going to `http://localhost:3000/`
Check you balance at `http://localhost:3000/balance`
See the list of transactions `http://localhost:3000/transfers`

### Edit
This example doesn't work. It is necessary to change line 67 in RadixKeyPair.js to:
```
return bs58_1.default.encode(Buffer.from(addressBytes));
```
