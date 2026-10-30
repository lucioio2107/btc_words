# btc_words
Search Mnemonic words for BTC address (offline check in file). Python3 implementation Using _multi cpu_.
The script could be helpful to target the BTC Puzzle Transaction >100 BTC unsolved currently. 

# Info
The script generate randomly the English Mnemonic words and calculates the BTC derivation path BTC address and compare them in the input btc address file. If match is found the script will stop and print the corresponding mnemonic words on screen along with the matching btc Address.

Default Value used, can be changed if required. Currently they are set to make 12 words, using 4 cpu and checking the first address only in the derived path of the words.
``
_entropy_bits_to_mnemonic_ function can be modified if any other language words are needed. Currenly the default is English Words only.

# p2sh
The script p2sh_brute, try to operate on only HASH160 collision where p2sh address could be redeemed using the correct redeem script. It avoids the EC operation of privatekey -> Pubkey.

# Run
(base) C:\anaconda3>python bip44_words_mcpu.py
[+] Starting.........Wait.....
[+] Loaded 256 address from file: btc_address.txt
Starting thread:  2
Starting thread:  1
Starting thread:  3
Starting thread:  0
[+] Program Starting ... Please Wait
[+] Loaded 7644366 p2sh Address.
[+] Converted back to HASH160 bytes and loaded in a SET...
Completed    100200000]  [238399.81 Key/s]  Script=     
SIGINT or CTRL-C detected. Exiting gracefully.
# Tips
BTC:	bc1q39meky2mn5qjq704zz0nnkl0v7kj4uz6r529at
ETH:	0xa74fC23f07A33B90d6848dF0bb409bEA5Ac16b28
DOGE:	D5Wh5bQMc3XVGdLbjJbGjryjNom5tZY6dD

