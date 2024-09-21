###  Test Installation
7. Create a test Go program:
   - Open a terminal and create a new file called `hello.go`:

     ```bash
     nano hello.go
     ```

   - Add the following content to the file:

     ```go
     package main

     import "fmt"

     func main() {
         fmt.Println("Hello, World!")
     }
     ```

   - Save the file (`Ctrl + O`), then exit (`Ctrl + X`).

8. Run the program:

   ```bash
   go run hello.go
   ```

   You should see the output:

   ```
   Hello, World!
   ```
