# monero-address
0. https://github.com/luigi1111/xmr.llcoins.net
1. fetch the json
https://moneroblocks.info/api/get_transaction_data/2c752e5bbb54c8bc4066404de498d2749b6c0c94343ad7f8c8ead80044ed2798

2. modify checktx.html for convenience
<input class="boxes" type="text" id="txHash" placeholder="64 hex chars" size="66" value="2c752e5bbb54c8bc4066404de498d2749b6c0c94343ad7f8c8ead80044ed2798"/>

<input class="boxes" type="text" id="private" placeholder="64 hex chars" size="66" value="9fc78ed7b30da2d5f5dfbc501c2234406e280b7ee0d2a0ab86999814e1386600"/>

3. Launch checktx.html and choose "Tx Private Key"
4. Assign the json to variable "tx_json_str" (site.js:90)
5. Comment out site.js:858-873
6. site.js:874	res = JSON.parse(tx_json_str);
