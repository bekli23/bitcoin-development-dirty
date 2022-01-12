# Bitcoin core mod dirty
SOON UPDATE  <br>
<img src="https://github.com/bekli23/v0.17.0.1-g-01xploid-development-dirty/blob/main/bitoins-to-bits-2.jpg?raw=true" alt="Get all the lost bitcoin :)">

👀 Hi, I'm a normal person and for about 3 years I've learned a lot about cryptography and cryptocurrencies. <br>
👀Normally you will say that it is not possible for me to do this project.<br>
👀In the first part I will make a major change in bitcoin core ,basically I want to stop signing transactions <strong>only</strong> with private key.<br>
------------------------------------------------------------------------------------------------------------------------------------------------
     So an example of what I will do.
Bob has his private key.<br>
Eve sends a message to Alice, together with a "confirmation" calculated using Bob's public key.<br>
Alice receives the message and Bob's public key, calculates confirmation == signature => Message was sent by Bob <br>
How is it different from Bob sending his message and a signature calculated using his private key?<br>
Problem 1: I have  code when you transferred it from the example. This line<br>
hash = message**65537 % 2**8  # incorrect<br>
should use multiplication instead of the power function<br>

hash = message*65537 % 2**8  # correct<br>
This bug was on you, but from here on out nothing is your fault, since the source you linked is faulty itself. So let's go ahead and fix your code bit by bit.<br>

I will switch to the regular case of signing with a private key and checking with a public key to make sure the algorithm works and then we'll run your attack again.<br>

🌱 Attention !!!!!!! this is an experimental project so don't put your real wallet with money !!!
