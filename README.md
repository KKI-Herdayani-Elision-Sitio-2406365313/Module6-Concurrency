## MODULE6

### Commit 1
Inside the handle_connection function, I add BufReader to read the data from the TCP stream.
By using the .lines() method and collecting them into a Vec, I am able to see the raw HTTP request sent
by the browser in the console.
This helped me understand that a request is basically just a series of text lines containing information about
what the browser wants.