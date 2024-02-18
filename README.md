# irc_server
IRC (Internet Relay Chat) - an application-level Protocol for exchanging messages in real-time. Designed primarily for group communication, it also allows you to communicate via private messages and exchange data, including files. IRC uses the TCP transport protocol and cryptographic TLS (optional). IRC began to gain particular popularity after Operation "Desert Storm" (1991), when messages from all over the world were collected in one place and broadcast on-line to IRC. Due to the technical simplicity of implementation, the IRC protocol was used in the organization of botnets as a means of transmitting control commands to the computers participating in the botnet from the owner. 🌎 IRC network According to the protocol specifications, an IRC network is a group of servers connected to each other. The simplest network is a single server. The network should have the form of a connected tree, in which each server is the central node for the rest of the network. A client is anything that is connected to the server, except for other servers. There are two types of customers: custom settings; service stations. Forwarding messages in the IRC network IRC provides both group and private communication. There are several possibilities for group communication. A user can send a message to a list of users, and a list is sent to the server, the server selects individual users from it, and sends a copy of the message to each of them. More efficient is the use of channels. In this case, the message is sent directly to the server, and the server sends it to all users in the channel. In both group and private communication, messages are sent to clients via the shortest path and are visible only to the sender, recipient, and incoming servers. It is also possible to send a broadcast message. Client messages regarding changes in the network state (for example, channel mode or user status) must be sent to all servers that are part of the network. All messages originating from the server must also be sent to all other servers.

# Author
[iragusa](https://github.com/IvanaRagusa)

# Usage

# :notebook_with_decorative_cover: Table of Contents

- [About the Project](#star2-about-the-project)


## :star2: About the Project

## :toolbox: Getting Started

### :bangbang: Prerequisites

- install Konversation : is a user-friendly Internet Relay Chat (IRC) client by KDE. It provides easy access to standard IRC networks such as Libera, where the KDE IRC channels can be found.<a href="https://snapcraft.io/konversation"> Here</a>


### :running: Run Locally

Clone the project

```bash
https://github.com/IvanaRagusa/irc_server
```
Go to the project directory
```bash
cd irc_server
```
compile
```bash
make
```
make the server listen
```bash
./ircserv <port number> <password>
```
the shell shows you a message like this
```bash
Server started and listening on IP <ip> port <port>
```
open konversation, up left side click on file-> server list-> new
choos a name for you server and click add under field Servers
insert the listening ip of the server message, and port and password choosed on launching
save and select your server in teh list and click connect
Now you're connected as client and you're on welome channel
you can use some command:
To create a channel
```bash
/JOIN #<name_of_channel>
```
you can send prv message or chat in the channel
You can moderate channel (User modes: +o, Channel modes: +b+l+i+k+t -b-l-i-k-t) you can use single or combinate mode commands
example of user mode to give operator privilages
```bash
/MODE #CHANNEL +o user_name
```
example of channel mode to set a password to enter in channel
```bash
/MODE #CHANNEL +k password
```
You can chat also with bot in WELCOME channel, try to write in the channel !WE followed by one of this words: -ciao -ping -aiuto -Gabry -Beppe -Nelly -Simo -Alegre -Niz -Victor -Ste -Btani -Lupe -Pacci -Dip -Fratm
```bash
!WE ciao
```
you can kick someone frome a channel if you are operator
```bash
/KICK #CHANNEL username
```
fun with other command like: /PART /INVITE /PRIVMSG /QUIT /TOPIC
