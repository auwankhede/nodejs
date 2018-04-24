# nodejs

Node installation redhat7
For Latest Release:-

step 1:

sudo yum install -y gcc-c++ make

sudo curl -sL https://rpm.nodesource.com/setup_9.x | sudo -E bash -

Step 2 – Install Node.js and NPM

sudo yum install -y nodejs

Step 3 – Check Node.js and NPM Version

node -v 

npm -v

Step 4 – Create Demo Web Server (Optional)

vim demo_server.js

var http = require('http');
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end('Welcome Node.js');
}).listen(3001, "127.0.0.1");
console.log('Server running at http://127.0.0.1:3001/');


node --inspect demo_server.js


debugger listening on port 5858
Server running at http://127.0.0.1:3001/
terminal log:
 300  yum install -y gcc-c++ make
  301  sudo yum install -y gcc-c++ make
  302  sudo curl -sL https://rpm.nodesource.com/setup_9.x | sudo -E bash -
  303  sudo yum install -y nodejs
  304  node -v
  305  npm -v
  306  vi demo_server.js
  307  node --debug demo_server.js 
  308  node --inspect demo_server.js 

