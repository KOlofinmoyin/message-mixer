# Message Mixer
![super-encoder](https://user-images.githubusercontent.com/33905131/132507161-b1fb441d-4118-4b1a-9f12-d4960ab8b13b.gif)


Message Mixer Inc. offers a message-encryption service that transforms input text, using various ciphers, and displays the encrypted message to the console.

There are three encryption methods provided by this service:

+ A `Caesar Cipher` in which the characters of the input message are shifted alphabetically by a given amount.
+ A `Symbol Cipher` in which select characters from the input message are replaced with visually similar symbols.
+ A `Reverse Cipher` in which each word of the input message is reversed in place.

To use this service, run the command below:

```
node message-mixer.js ['caesar'|'symbol'|'reverse'] [amount]
```

Here are some examples of running this program:

```
$ node message-mixer.js caesar 4
Enter the message you would like to encrypt...
> hello world

Here is your encrypted message:
> lipps asvph
```

```
$ node message-mixer.js 'reverse'
Enter the message you would like to encrypt...
> hello world

Here is your encrypted message:
> olleh dlrow
```

At present, Message Mixer Inc. sells their encryption service as a program in a single file called message-mixer.js. This single file includes:

+ The functions that perform the encryptions listed above.
+ The code for retrieving the user input.
+ The code for displaying the output back to the user.

Message Mixer Inc. now wants to join the open-source community by packaging its encryption functions in a module and allowing other developers to import these encryption functions into their own projects.

### Objective:
In this project, you will help Message Mixer Inc. extract and isolate its encryption functions into a module, called encryptors.js, and then refactor message-mixer.js to use this module’s functions.
