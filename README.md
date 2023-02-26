## Discuss one challenge you overcame during your academic development. What was the challenge, was it technical, nontechnical, or both, and how did you overcome it?

The first 7 lines are importing libraries in order to get the functionality we need in our program. Line 9 declares the namespace as std, which is more efficient when using the iostream library. Line 13 declares important variables that we will use in the program. Line 14 declares the struct we will be using to hold information about the socket. In line 15 we declare the cstrings we will be using to temporarily hold information about the socket. Line 16 declares addr_size. Lines 17-23 declare more variables that we will use later in the program. In line 25, socket sets the socket we want with the parameters. In line 26, setsockopt lets us set the socket options that we want, which is detailed in the parameters. Line 27, sets one of the ServerAdd struct’s members. In line 28, we ask for the server address on the screen using cout. In line 29 we get an input from the user in the format that we detail. In line 30, we ask for the user’s server port on the screen by using cout. In line 31, we get an input from the user by using cin.getline which retrieves inputs from the user in a specific way. In lines 32-36, we use the inputs given to us by cin and store information about the socket accordingly. In line 37, we ask the user for a file name using cout. In lines 38-40, we get the input of a file name with cin, and open the file with fopen. In line 42, we check to make sure pFile isnt empty. In line 45,  we set nBytes equal to the length of the filename. In 46, we set resend to false. In lines 47-63 we will run a loop that will continue until resend is set to false. This loop sends a message on the socket in line 49 containing information like the filename and addr_size. The next line sets nBytes to what it receives on the socket. The purpose of this section is to get information about the socket and file over to the server. Lines 65-67 set variables to start reading the bytes. 
On lines 68-99, the loop runs until there is no more data to read. The loop on lines 70-96 runs until the resend variable is set to false. The purpose of this loop is to start reading messages coming from the server. Line 74 sets the starting location in the file. Line 76 goes to the asking position. Lines 78-83 read 1000 bytes of data, the for loop on 80 reads until the index reaches the read_size which we set at 1000. The next lines send the information over, and receive the information. Memset on line 98 clears the buffer. The else on 103 is if the pFile has no information stored in it. Lines 107-109 stops writing to the buffer, sends the information over through the socket, and then closes the socket. Line 111 returns 0 to the main function, which ends the program.


## Discuss a situation where you worked with a team. How would you describe yourself as a teammate? Where can you improve your team skills? Be specific.



## What type of career in CS do you believe you are most suited for? Why this field and not another? Be specific.



## What professional organizations would you like to join? What professional development would you like to be a part of in the next five years? Be specific and don't consider places of employment.



## What are the ways you can use the skills you have learned in CS to serve your community? Be specific.
