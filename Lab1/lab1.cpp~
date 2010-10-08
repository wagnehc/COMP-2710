#inlude <iostream>
using namespace std;

class User;
class Chatroom;
class Message;
class Connection;
class System;
class Menul;

class User {
    string userName;
    Connection[] connects;
}

User::getUserName(){
    return userName;
}

User::setUserName(string name){
    this.userName = name;
}

User::addConnection(Connection newConnect){
    for(int i = 0; i < connects.size; i++){
	if( !(this.connects[i].isEmpty() ){
	    continue;
	}
	else{
	    this.connects[i] = newConnection;
	}
    }
}


class Chatroom {
    User[] currentUsers;
    string surrentMsg;
}

Chatroom::addUser(string userName){
    for( int i = 0; i < currentUsers.size; i++){
	if( !(currentUsers.isEmpty() )
	    continue;
	else
	    currentUsers[i] = userName;
    }
}

Chatroom::broadcastMsg(string msgToSend) {
    for(int i = 0; i < currentUsers.size; i++){
	currentUsers[i].getConnection().addMsg(msgToSend);
    }
}




class Message {
private:
    string userName;
    string msgTxt;
public:
    toString();
}

Message::Message(string userName, string msgTxt){
    this.userName = userName;
    this.msgTxt = msgTxt;
}

string Message::toString(){
    string formattedMsg;
    formattedMsg = userName + ": " + msgTxt;
    return formattedMsg;
}



class Connection {
    string newMsgs;
    string msgHistory;
    string userNames[];
}

void Connection::addNewMsg(Message newMsg){
    this.newMsgs += "\n" + newMsg;
}

string Connection::showMsgs(){
    
}

class System {
    string currentUser, currentRoom;
    User users[];
    Chatroom chatrooms[];
}

System::System() {
    currentUser ="";
    currentRoom ="";
}

void System::addUser(User newUser) {
    for(int i = 0; i < 3; i++){
	if(users[i] == null) 
	    users[i] = newUser;
    }
}

bool System::addRoom(Chatroom newRoom) {
    for(int i = 0; i < 2; i++){
	if(chatrooms[i] == null){
	    chatrooms[i] = newRoom);
	    return true;
	}
	else
	    return false
    }
}

void System::setCurrentRoom(String currentRoom) {
    this.currentRoom = currentRoom;
}

void System::setCurrentUser(String currentUser) {
    this.currentUser = currentUser;
}

String System::getCurrentUser(){
    return currentUser;
}

String System::getCurrentRoom(){
    return currentRoom;
}

class Menu {
    private:		
	int menuSelection;
	System currentSystem;
    public:
	getCurrentSys();
	setCurrentSys(System);
	getMenuSelection();
	setMenuSelection(int);
}

Menu::Menu (System primary){
    currentSystem = primary;
}

void Menu::setMenuSelection(int select){
    menuSelection = select;
}

int Menu::getMenuSelection(){
    return menuSelection;
}

void Menu::setCurrentSys (System current){
    currentSystem = current;
}

System Menu::getCurrentSystem(){
    return currentSystem;
}
