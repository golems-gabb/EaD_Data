# Encrypt And Decrypt Data on golang.
To start using "ead_data" you need:
* Install and configure the latest version of Golang
* To use "ead_data", add in import - "github.com/pifagor87/EaD_Data".
* Example


func main() {

	ciphertext := ead_data.encrypt([]byte("Hello World"), "password")

	plaintext := ead_data.decrypt(ciphertext, "password")

	ead_data.encryptFile("sample.txt", []byte("Hello World"), "password1")

	ead_data.decryptFile("sample.txt", "password1")

}