#### Uncaught Error: listen EADDRINUSE: address already in use :::3000

node:events:502 Uncaught Error: listen EADDRINUSE: address already in use :::3000
at Server.setupListenHandle [as _listen2] (node:net:1912:16)
at listenInCluster (node:net:1969:12)
at Server.listen (node:net:2074:7)
at Function.listen (/Users/visheshparab/Developer/NodeJS Lessons/4-natours/node_modules/express/lib/application.js:635:24)
at Object.<anonymous> (/Users/visheshparab/Developer/NodeJS Lessons/4-natours/server.js:34:5)
at Module.\_compile (node:internal/modules/cjs/loader:1565:14)
at Object..js (node:internal/modules/cjs/loader:1708:10)
at Module.load (node:internal/modules/cjs/loader:1318:32)
at Function.\_load (node:internal/modules/cjs/loader:1128:12)
at TracingChannel.traceSync (node:diagnostics_channel:322:14)
Emitted 'error' event on Server instance at:
at emitErrorNT (node:net:1948:8)
at process.processTicksAndRejections (node:internal/process/task_queues:90:21)

#### Solution

- First, you would want to know which process is using port 3000
- cmd: sudo lsof -i :3000
- this will list all PID listening on this port, once you have the PID you can terminate it with the following:
- cmd: kill -9 <PID>
- where you replace <PID> by the process ID, or the list of process IDs, the previous command output.
