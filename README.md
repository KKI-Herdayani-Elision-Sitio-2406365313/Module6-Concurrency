## MODULE6

### Commit 1
Inside the handle_connection function, I add BufReader to read the data from the TCP stream.
By using the .lines() method and collecting them into a Vec, I am able to see the raw HTTP request sent
by the browser in the console.
This helped me understand that a request is basically just a series of text lines containing information about
what the browser wants.

### Commit 2
![Commit2.png](assets/image/Commit2.png)
I learned that an HTTP response needs a specific format which are a status line, headers, and the message body.
I used the fs module to read the contents of an external HTML file called hello.html.
I then calculated the length of that content and formatted it into a  HTTP response string.
Lastly, i used stream.write_all to send that data back, which allowed the browser to actually render a webpage.

### Commit 3
### Commit 4
### Commit 5
