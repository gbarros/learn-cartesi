
# Requirements

You should have:

- python3
- nodejs 
- yarn
- docker desktop

if on windows, you should have wsl2 installed and running. 

# Instructions

## 1. Environment Setup

1. install sunodo @ sunodo.io

    > npm install -g @sunodo/cli


2. install project dependencies

    > yarn 

3. run your node for the 1st time

    > sunodo run

4. Lets inform it of its own ethereum address on the base layer

    > sunodo send dapp-address

    Check the logs to see that it worked.

    The payload should be the address of the application you used to send the transaction.

5. Send a generic message to the node

    > sunodo send generic input="Your Msg Here"

    Use the this [online tool](https://string-functions.com/hex-string.aspx) to convert the payload from hex to string 

    There are many other options with the `sunodo send` command, explore them using `sunodo send --help`.

## 2. Learning about "no-backend" option flag

You can run your application directly from your machine (bare metal) so it's easier to debug and quicker on the re-lauching cycles. Here's how:

>   sunodo run --no-backend


## 3. Installing Deroll

1. Install the deroll app libraries

    >   yarn add @deroll/app @deroll/router @deroll/wallet


