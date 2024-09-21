To install Go (Golang) on Linux/Ubuntu, follow these steps:

### Step 1: Download the Latest Go Version
1. Open a terminal.
2. Download the latest version of Go for Linux (check the [official Go download page](https://go.dev/dl/) for the latest version). Here, we'll use Go 1.21.1 as an example:

   ```bash
   wget https://go.dev/dl/go1.21.1.linux-amd64.tar.gz
   ```

### Step 2: Extract the Archive
3. Once downloaded, extract the tarball and move it to `/usr/local`:

   ```bash
   sudo tar -C /usr/local -xzf go1.21.1.linux-amd64.tar.gz
   ```

### Step 3: Set Up Go Environment Variables
4. Add Go’s bin directory to your `PATH` by modifying your shell profile (`.bashrc`, `.zshrc`, or another file depending on your shell):

   - For `bash` (the default shell on Ubuntu), append the following line to your `~/.bashrc` file:

     ```bash
     echo "export PATH=$PATH:/usr/local/go/bin" >> ~/.bashrc
     ```

   - For `zsh`, add the line to `~/.zshrc` instead:

     ```bash
     echo "export PATH=$PATH:/usr/local/go/bin" >> ~/.zshrc
     ```

### Step 4: Apply the Changes
5. Apply the changes by sourcing your profile:

   - For `bash`:

     ```bash
     source ~/.bashrc
     ```

   - For `zsh`:

     ```bash
     source ~/.zshrc
     ```

### Step 5: Verify Installation
6. Check if Go is installed correctly by running:

   ```bash
   go version
   ```

   You should see something like this:

   ```
   go version go1.21.1 linux/amd64
   ```

### Step 6: Test Installation
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

BOOM, Now you're done, U can Start Working with it!
