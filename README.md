# 📡 Erlang Inter-Process Communication: Alice and Bob

Welcome to the Erlang project demonstrating inter-process communication using concurrent processes. This example showcases Erlang's powerful concurrency model and message-passing capabilities through the interaction between Alice and Bob processes.

## 📜 Project Description

In this project, we have two processes:

- **Alice**: Waits for messages and responds back.
- **Bob**: Sends messages to Alice a specified number of times and waits for a response each time.

## 🛠️ Modules and Functions

### `talk.erl`

- `alice/0`: The Alice process waits for messages and responds back to Bob.
- `bob/2`: The Bob process sends messages to Alice and waits for responses. It stops after a specified number of messages.
- `run/0`: Starts both Alice and Bob processes.
- `startAlice/0`: Starts the Alice process.
- `startBob/1`: Starts the Bob process, taking Alice's node as an argument.

## 📦 How to Use

### 1. Compile the Module

```erlang
c(talk).
2. Run the Processes
To start both Alice and Bob:

erlang
Copy code
talk:run().
To start Alice and Bob separately:

erlang
Copy code
talk:startAlice().
talk:startBob(node_name). % replace node_name with the actual node name
Example Output
erlang
Copy code
Alice got a message
Bob got a message
Alice got a message
Bob got a message
Alice got a message
Bob got a message
Alice is finished
Bob is finished
🚀 Key Highlights
Concurrency: Erlang’s lightweight processes make it easy to handle concurrent operations.
Message Passing: Processes communicate seamlessly through message passing, ensuring efficient inter-process interaction.
Fault Tolerance: The design is inherently resilient, handling failures gracefully.
📚 Learn More
Erlang Documentation
Learn You Some Erlang for Great Good!
```
