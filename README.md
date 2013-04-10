#morse.js#

Easy JavaScript morse encoder and decoder.

**Usage:**

    var str = "Hello World",
        encoded = morse.encode(str),
        decoded = morse.decode(encoded);

    console.log(encoded); // ".... . .-.. .-.. --- / .-- --- .-. .-.. -.."
    console.log(decoded); // "HELLO WORLD"

-----

**Error handing:**


	var str = "Special String & +",
        encoded = morse.encode(str),
        decoded = morse.decode(encoded);

    console.log(encoded); "... .--. . -.-. .. .- .-.. / ... - .-. .. -. --. / /"
    console.log(decoded); "SPECIAL STRING  "

    // Using morse.silent(false);
    morse.silent(false);

    morse.encode(str); // Uncaught Error: morse.encode: Can't handle &
