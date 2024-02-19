
    <h1>TCP Server for String Reversal</h1>

    <p>This is a simple TCP server written in Java that allows multiple clients to connect simultaneously and reverses strings sent by clients. The server limits the maximum number of clients to 10 and introduces a delay using <code>Thread.sleep()</code> to simulate processing.</p>

    <h2>Usage</h2>

    <h3>Prerequisites</h3>
    <ul>
        <li>Java Development Kit (JDK) installed on your system.</li>
    </ul>

    <h3>Running the Server</h3>
    <ol>
        <li>Compile the Java source code:</li>
        <pre><code>javac TCPServer.java</code></pre>
        <li>Run the server:</li>
        <pre><code>java TCPServer</code></pre>
        <li>The server will start listening on port 12345 by default.</li>
    </ol>

    <h3>Connecting Clients</h3>
    <p>You can connect clients to the server using any TCP client application. Here's an example of connecting using Telnet:</p>
    <pre><code>telnet localhost 12345</code></pre>

    <h3>Sending Strings</h3>
    <p>Once connected, you can send strings to the server. The server will reverse each string and send the reversed string back to the client. A delay of 1 second is introduced for processing each string.</p>

    <h3>Exiting</h3>
    <p>To exit the server, simply terminate the process.</p>

    <h2>Customization</h2>
    <ul>
        <li>You can customize the server port by modifying the <code>PORT</code> constant in the <code>TCPServer</code> class.</li>
        <li>Adjust the maximum number of clients allowed by changing the <code>MAX_CLIENTS</code> constant in the <code>TCPServer</code> class.</li>
        <li>Modify the processing delay by changing the argument of <code>Thread.sleep()</code> in the <code>ClientHandler</code> class.</li>
    </ul>

    <h2>Contributors</h2>
    <ul>
        <li><a href="https://github.com/yourusername">Your Name</a></li>
    </ul>

    <h2>License</h2>
    <p>This project is licensed under the MIT License - see the <a href="LICENSE">LICENSE</a> file for details.</p>
