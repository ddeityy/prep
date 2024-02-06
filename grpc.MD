# gRPC

## Pros & Cons
* Pros
    * Fast & Compact
    * One Client Library
    * Progress Feedback (upload)
    * Cancel Request (HTTP2)
    * H2/Protobuf
* Cons
    * Thick Client
    * Schema
    * Proxies
    * No error handling
    * No native browser support
    * Timeouts (pub/sub)

## Modes

1. Unary
    ```
    Request - Response
    Example: database query
    ```

2. Server streaming 
    ```
    Server sends data, client receives
    Example: yt video, twitch stream
    ```
3. Client Streaming 
    ```
    Client sends data, server receives
    Example: uploadig a file
    ```

4. Bidirictional streaming RPC
    ```
    Ad-hoc bidirectinal communication
    Example: yt video, twitch stream
    ```


## Structure
<img src="https://ecm.capitalone.com/WCM/tech/grpc-3.png" alt="alt text" width="800"/>
