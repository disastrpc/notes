Sources:
NTLM Protocol Explanaition [source](http://davenport.sourceforge.net/ntlm.html#theNtlmMessageHeaderLayout)

NTLM is a challenge-response scheme protocol consisting of three messages:

- Type 1 (negotiation)
- Type 2 (challenge)
- Type 3 (authentication)

1- The client sends a Type 1 message to the server. This primarily contains a list of features supported by the client and requested of the server.
2- The server responds with a Type 2 message. This contains a list of features supported and agreed upon by the server. Most importantly, however, it contains a challenge generated by the server.
3- The client replies to the challenge with a Type 3 message. This contains several pieces of information about the client, including the domain and username of the client user. It also contains one or more responses to the Type 2 challenge.
