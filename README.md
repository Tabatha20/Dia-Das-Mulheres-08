body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #fff;
    margin: 0;
    padding: 0;
}

header {
    background: #ff4081;
    color: white;
    padding: 15px;
}

#btn-chat {
    background: #d81b60;
    color: white;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    font-size: 16px;
    margin-top: 10px;
}

#chat-container {
    width: 300px;
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: #ffc0cb;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.hidden {
    display: none;
}

.chat-header {
    background: #d81b60;
    color: white;
    padding: 10px;
    font-weight: bold;
    border-radius: 10px 10px 0 0;
}

.chat-box {
    padding: 10px;
    max-height: 200px;
    overflow-y: auto;
    text-align: left;
}

.chat-message {
    background: #ff4081;
    color: white;
    padding: 8px;
    border-radius: 5px;
    margin-bottom: 5px;
}

.chat-input {
    display: flex;
    padding: 10px;
    background: white;
    border-radius: 0 0 10px 10px;
}

.chat-input input {
    flex: 1;
    padding: 5px;
    border: 1px solid #d81b60;
    border-radius: 5px;
}

.chat-input button {
    background: #d81b60;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    margin-left: 5px;
}
body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #fff;
    margin: 0;
    padding: 0;
}

header {
    background: #ff4081;
    color: white;
    padding: 15px;
}

#btn-chat {
    background: #d81b60;
    color: white;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    font-size: 16px;
    margin-top: 10px;
}

#chat-container {
    width: 300px;
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: #ffc0cb;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.hidden {
    display: none;
}

.chat-header {
    background: #d81b60;
    color: white;
    padding: 10px;
    font-weight: bold;
    border-radius: 10px 10px 0 0;
}

.chat-box {
    padding: 10px;
    max-height: 200px;
    overflow-y: auto;
    text-align: left;
}

.chat-message {
    background: #ff4081;
    color: white;
    padding: 8px;
    border-radius: 5px;
    margin-bottom: 5px;
}

.chat-input {
    display: flex;
    padding: 10px;
    background: white;
    border-radius: 0 0 10px 10px;
}

.chat-input input {
    flex: 1;
    padding: 5px;
    border: 1px solid #d81b60;
    border-radius: 5px;
}

.chat-input button {
    background: #d81b60;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    margin-left: 5px;
}document.getElementById("btn-chat").addEventListener("click", function () {
    document.getElementById("chat-container").classList.toggle("hidden");
});

document.getElementById("send-btn").addEventListener("click", function () {
    let userInput = document.getElementById("user-input").value;
    if (userInput.trim() !== "") {
        let newMessage = document.createElement("div");
        newMessage.classList.add("chat-message");
        newMessage.textContent = userInput;
        document.getElementById("chat-box").appendChild(newMessage);
        document.getElementById("user-input").value = "";
    }
});
