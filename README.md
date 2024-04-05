# Simple-chatbot

# Define a dictionary of responses
responses = {
    "hello": "Hello! How can I assist you today?",
    "bye": "Goodbye! Have a great day!",
    "thanks": "You're welcome!",
    "default": "I'm sorry, I didn't understand. Can you please rephrase?"
}

# Main chat loop
while True:
    user_input = input("You: ").lower()  # Convert user input to lowercase
    if user_input == "exit":
        print("Chatbot: Goodbye!")
        break
    response = responses.get(user_input, responses["default"])
    print(f"Chatbot: {response}")
