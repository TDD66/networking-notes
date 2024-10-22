# Mutual Transport Layer Security (mTLS)

In TLS, once the client establishes that they can trust the server, encrypted communication is initiated.

However, in mTLS the server must also establish that they can trust the client. So their must be mutual trust between the client and the server. 

TLS Steps:
1. Client connects to the server.
2. Server presents its certificate.
3. Client trusts certificate as it is signed by an intermediate which links back to root CA.
4. Client and server generate shared secret and commence encrypted communication.

mTLS Steps:
1. Client connects to server.
2. Server presents its certificate.
3. Client trusts certificate as it is signed by an intermediate which links back to root CA.
4. **Client presents its certificate.**
5. **Server trusts certificate as it is signed by and intermediate which links back to root CA.**
6. Client and server generate shared secret and commence encrypted communication.