
**This program is ONLY FOR EDUCATIONAL PURPOSES.**

This script provides a basic framework for continuously generating and checking Litecoin wallets.


Process:
    Continuous Generation: The main function runs an infinite loop to continuously generate new Litecoin wallets.
    Check Balance: For each generated wallet, it checks the balance using the BlockCypher API.
    Save to File: If a wallet with a positive balance is found, it writes the wallet details (private key, public key, address, and balance) to a file called found.txt.
    Delay: A delay of 1 second between iterations to prevent overwhelming the API and to manage the rate limit. Adjust this as necessary based on API limitations and performance needs.


Ensure you have the necessary libraries installed:
pip install ecdsa base58 requests

Also please note:
    API Rate Limits: Be aware of the rate limits of the BlockCypher API or any other API used. Adjust the time.sleep() delay accordingly.
    Security: Keep the found.txt file secure as it contains private keys.
    Usage: Ensure this script is used responsibly and ethically.
