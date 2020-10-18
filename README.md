# Go Chat 
[![GoDoc](http://img.shields.io/badge/go-documentation-blue.svg?style=flat-square)](https://godoc.org/github.com/taylorflatt/go-chat)
[![Code Coverage](https://img.shields.io/badge/CodeCoverage-99p-F01F7A?style=plastic&logo=CodeCov)](https://github.com/social-learning/TensorMap)
[![Github](https://img.shields.io/badge/GitHub-TensorMap-181717?style=plastic&logo=GitHub)](https://github.com/social-learning/TensorMap)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-CodeForAll-0077B5?style=plastic&logo=LinkedIn)](https://www.linkedin.com/company/codeforall/)


A client-server chat app implemented in Go using gRPC.

## Usage
### Server
Start the server by running `go run server.go`. Alternatively, you can run `go build` while in the Server directory.
### Client
Start the client(s) by running `go run client.go menu.go`. Alternatively, you can run `go build` while in the Client directory.

To run navigate the client: 
* First enter the server ip:port exactly. It is likely `localhost:12021` unless the port at the top of server.go has changed.
* Then you'll enter a username that is yours for the session.
* Finally, you are greeted by the menu system which will allow you to create, join, or view other members and groups.

## Known Bugs
* None currently. If you run into any problems, please don't hesistate to create an issue.

## Notes
* To disconnect from the server, press ctrl+c or type `!exit` (hit enter) and the client will disconnect from the server.
* To move backwards in the menu system, you can type `!back` (hit enter).
* This client/server assumes a 12021 server port. This can be changed in the server.go file near the top.

## Future Ideas
* The !leave function to leave a chat and go back to the main menu.
* Encryption on chat channels.
* Ability to send files.
* Complete server re-write to be more extendible and understandable.
