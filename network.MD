# OSI

| Уровни        	| Данные   	| Функции                                                  	              | Протоколы            	|
|---------------	|----------	|------------------------------------------------------------------------ |----------------------	|
| Физический    	| Биты     	| Передача двоичных<br>данных                              	              | Bluetooth, WiFi      	|
| Канальный     	| Фреймы   	| Физическая адресация                                     	              | Ethernet, MAC        	|
| Сетевой       	| Пакеты   	| Определение маршрута<br>Логическая адресация            	              | IP                  	|
| Транспортный  	| Сегменты 	| Прямая связь между<br>конечными пунктами<br>и надёжность<br>Буферизация | TCP, UDP, Порты      	|
| Сеансовый     	| Данные   	| Управление сеансом связи                                 	              | gRPC                 	|
| Представления 	| Данные   	| Представление и<br>шифрование данных                     	              | ASCII, SSL, gzip     	|
| Прикладной    	| Данные   	| Доступ к сетевым службам                                 	              | HTTP, FTP, Websocket 	|

</br>

# TCP
![Sequence-Diagram-for-Opening-a-TCP-Connection](https://github.com/ddeityy/prep/assets/97681057/34343b9d-5265-4884-b9cf-b3b0289d2ae2)

</br>

# UDP
![how-udp-works](https://github.com/ddeityy/prep/assets/97681057/0c2ea07a-6a4c-4798-bd01-8c1021edae03)

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
