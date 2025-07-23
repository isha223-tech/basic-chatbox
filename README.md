# basic-chatbox
here i am sharing a exciting and helpful chatbox to everyone using python language.

# why its helpful?
1. Great for beginners learning python.
2. Helps covering various concepts of python (eg if-elif, functions, loops, input/output)

# Define a function to get chatbot reply
def get_reply(user_input):
    user_input = user_input.lower()  # make input lowercase

    if user_input == "hello":
        return "Hi"
    elif user_input == "how are you":
        return "I am fine, thanks!"
    elif user_input == "bye" or user_input == "goodbye":
        return "Goodbye!"
    else:
        return "I don't understand that."

# Main loop
print("Chatbot: Type 'bye' to end the chat.")
while True:
    user_message = input("You: ")
    reply = get_reply(user_message)
    print("Bot:", reply)

    if user_message.lower() == "bye" or user_message.lower() == "goodbye":
        break


