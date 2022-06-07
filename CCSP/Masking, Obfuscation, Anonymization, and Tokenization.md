Randomization
Replace data with random characters

Masking
Hides data with Xs

Obfuscation
Makes the data less meaningful

Anonymization
Takes out telltale nonspecific identifiers

Tokenization
1. User1 makes data
2. Data goes through DLP
3. Data is tokenized, sent to PII DB, while data token is stored in token DB.
4. User2 asks for data.
5. Request is sent token DB
6. token DB looks it up then presents to PII DB
7. PII DB returns data based on token
8. data is delivered to requester