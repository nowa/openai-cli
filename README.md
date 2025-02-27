# openai-cli
openai-cli is a command line interface to interact with the OpenAI API. It aims to provide most features the API does, but is currently focused on the new chat endpoint.

Using it looks like this:
```
Unsaved> !system You are a helpful assistant which translates any text I give you to french.
Unsaved> Hello
Bonjour.
Unsaved> Command line interfaces are amazing!
Les interfaces en ligne de commande sont incroyables !
```

## Commands
* `!system`: Write a system message, e.g., "You will translate text to french".
* `!save`: Save a conversation.
* `!load`: Load a converstation.
* `!history`: Show the converstation history.
* `!model`: Set the model you want to use, e.g., `!model gpt-3.5-turbo`.
* `!clear`: Clear the current conversation history.
* `!undo`: Undo last message.

I also intend to add support for completing promts from stdin or files for use in scripting.

## Keybinds
By defeault openai-cli uses emacs style keybinds.

However by using the `--vim` flag, you can use vim style keybinds instead.

You can **write newlines** using `ALT+ENTER`.

## Installation
Installation can be done via `cargo install openai-cli`.
