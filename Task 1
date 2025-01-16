def encrypt(plain_text, shift):
    encrypted_text = ""
    for char in plain_text:
        if char.isalpha():
            shift_base = 65 if char.isupper() else 97
            encrypted_text += chr((ord(char) - shift_base + shift) % 26 + shift_base)
        else:
            encrypted_text += char 
    return encrypted_text


def decrypt(encrypted_text, shift):
    decrypted_text = ""
    for char in encrypted_text:
        if char.isalpha():
            shift_base = 65 if char.isupper() else 97
            decrypted_text += chr((ord(char) - shift_base - shift) % 26 + shift_base)
        else:
            decrypted_text += char  
    return decrypted_text

def main():
    print("Welcome to Caesar Cipher Encryption/Decryption Program")

    
    message = input("Enter the message: ")
    shift = int(input("Enter the shift value: "))
    
    
    encrypted_message = encrypt(message, shift)
    print(f"Encrypted Message: {encrypted_message}")
    
    
    decrypted_message = decrypt(encrypted_message, shift)
    print(f"Decrypted Message: {decrypted_message}")

if __name__ == "__main__":
    main()
