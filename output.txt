#!/data/data/com.termux/files/usr/bin/python
import base64

choice = input("Encode (e) or Decode (d)? ")

if choice == 'e':
    text = input("Enter text to encode: ")
    print(base64.b64encode(text.encode()).decode())
elif choice == 'd':
    text = input("Enter base64 to decode: ")
    print(base64.b64decode(text.encode()).decode())
