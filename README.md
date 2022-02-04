# Bitcoin core mod dirty
SOON UPDATE  <br>
<img src="https://github.com/bekli23/v0.17.0.1-g-01xploid-development-dirty/blob/main/bitoins-to-bits-2.jpg?raw=true" alt="Get all the lost bitcoin :)">
*🏆PROGRESS UPDATE 🏆<br>
Generate new address✅ * <br>
import privatekey must start 5...exemple (5KK6mwkX27SgBvhN1pdC1z2dstrJ4vn5UgffYoexC1ySmAV1fMa)✅* <br>
create tx (core stay on , not shutdown) ✅<br>
unlock by change hash hex master key ✅(contact me for info) <br>
dump private key keymeta!  ✅successful <br>
dump private key ckey ⏳ *unsuccessful(work progress) <br>
Fixed private key import Uncompressed\Compressed ✅<br>
dump private key which I import✅<br>

👀 Hi, I'm a normal person and for about 3 years I've learned a lot about cryptography and cryptocurrencies. <br>
👀Normally you will say that it is not possible for me to do this project.<br>
👀In the first part I will make a major change in bitcoin core ,<br>
basically I want to stop signing transactions only with private key.<br>

------------------------------------------------------------------------------------------------------------------------------------------------<br>
     So an example of what I will do.
Bob has his private key.<br>
Eve sends a message to Alice, together with a "confirmation" calculated using Bob's public key.<br>
Alice receives the message and Bob's public key, calculates confirmation == signature => Message was sent by Bob <br>
How is it different from Bob sending his message and a signature calculated using his private key?<br>
Problem 1: I have  code when you transferred it from the example. This line<br>
hash = message**65537 % 2**8  # incorrect<br>
should use multiplication instead of the power function<br>

hash = message*65537 % 2**8  # correct<br>
<br>

I will switch to the regular case of signing with a private key and checking with a public key to make sure the algorithm works.<br>

🌱 Attention !!!!!!! this is an experimental project so don't put your real wallet with money !!!
