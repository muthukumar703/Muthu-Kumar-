# Muthu-Kumar-
chatbot program 
predefined_replies = {
    "hello": "Hi there! How can I help you?",
    "hi": "Hello! What can I do for you?",
    "how are you": "I'm just a bot, but I'm doing great!",
    "bye": "Goodbye! Have a nice day!",
    "thanks": "You're welcome!",
    "what is your name": "I'm a chatbot created to assist you.",
    "help": "Sure, I'm here to help. Ask me anything!"
}

def chatbot():
    print("Chatbot: Hello! Type 'bye' to exit.")
    while True:
        user_input = input("You: ").lower().strip()
        if user_input == "bye":
            print("Chatbot: Goodbye! Take care.")
            break
        response = predefined_replies.get(user_input, "Sorry, I didn't understand that.")
        print("Chatbot:", response)

chatbot()
