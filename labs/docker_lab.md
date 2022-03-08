# Verify Docker installation
- Our sample code is written in NodeJs so we will first download node image
to verify that docker is installed and working
- Run the following command in the shell
  ```bash
    docker run node
  ```

## Building our NodeJs server
- Now let’s add some code to this server and run it.
- Follow the below commands to create the server file
  ```bash
    # Create the desired folder
    mkdir hellodocker
    # Switch to the created directory
    cd hellodocker
    #
    # Create our server code file (copy the code into this file)
    #
    # Open the server.js file for edit
    vi server.js
    # 1. Set the file into edit mode by clicking on the letter [i] in your keyboard
    # 2. Copy the code
    # 3. Paste the code
    # 4. Save and exit by typing [`ESC` + `:` + ‘wq!` + ‘ENTER’]
    ```
- This is content of our server file
    ```js
    // import the HTTP module
    var http = require('http');
    // Define a port we want to listen to
    const PORT=8080;
    // We need a function which handles requests and send response
    function handleRequest(request, response){
    response.end('It Works!! Path Hit: ' + request.url);
    }
    // Create a server
    var server = http.createServer(handleRequest);
    // Start our server
    server.listen(PORT, function(){
    //Callback triggered when server is successfully listening. Hurray!
    console.log("Server listening on: http://localhost:%s", PORT);
    });
    ```
- Test our server code
  ```bash
  # Start the server with:
    node server.js
  ```

- Click on the most left icon (web preview) and open port 8080 which is
our server port