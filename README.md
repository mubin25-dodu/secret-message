# Custom Cipher Web Application

This repository contains a web application that allows users to encode and decode messages using a custom cipher. The application is hosted at https://mubin25-dodu.github.io/secret-message/.

## Features

* **Encode Messages**: Input any message, and the application will encode it using the custom cipher.
* **Decode Messages**: Input an encoded message, and the application will decode it back to the original message.
* **Copy to Clipboard**: Easily copy the encoded or decoded text to your clipboard.

## Usage

1. Open the web application in your browser.
2. To encode a message:
   * Enter the message you want to encode in the "Enter The Message to Encode" input field.
   * Click the "Encode" button.
   * The encoded message will be displayed in the "Encoded Message" section.
   * Click the "Copy Encoded" button to copy the encoded message to your clipboard.
3. To decode a message:
   * Enter the encoded message you want to decode in the "Enter The Message to Decode" input field.
   * Click the "Decode" button.
   * The decoded message will be displayed in the "Decoded Message" section.
   * Click the "Copy Decoded" button to copy the decoded message to your clipboard.

## Implementation

The application is implemented using HTML, CSS, and JavaScript. The main file is `index.html`, which contains the structure and styling of the web page, as well as the JavaScript functions for encoding, decoding, and copying text.

### Encoding and Decoding

The encoding and decoding functions use a custom cipher based on the position of each character in the message. The shift value for each character is calculated using the formula `2^n`, where `n` is the position of the character modulo 5. The functions handle both uppercase and lowercase letters, as well as spaces and other characters.

### Copying Text

The `copyText` function uses the Clipboard API to copy the encoded or decoded text to the user's clipboard. If the copy operation is successful, an alert is displayed to inform the user.
