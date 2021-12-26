# learn.svelte.js
Svelte.js Learning Project

Tutorial
[https://svelte.dev/tutorial/basics][1]

Documentation
[https://svelte.dev/docs][2]

Examples
[https://svelte.dev/examples][3]

REPL
[https://svelte.dev/repl][4]
---- 

# Start Svelte.js
## Install Home-brew
## Install Node.js

## Create Svelte App Directory
```bash
~/learn.svelte.js/ $ mkdir svelte-app
~/learn.svelte.js/ $ cd svelte-app 
```

## Clone Svelte.js Template
```bash
~/svelte-app/ $ npx degit sveltejs/template           
Need to install the following packages:
  degit
Ok to proceed? (y) 
> cloned sveltejs/template#HEAD
~/svelte-app/ $ 
```

## NPM Install
```bash
~/svelte-app/ $ npm install

added 97 packages, and audited 98 packages in 13s

6 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
~/svelte-app/ $ 
```

# NPM Run
```bash
~/svelte-app/ $ npm run dev

> svelte-app@1.0.0 dev
> rollup -c -w

rollup v2.62.0
bundles src/main.js → public/build/bundle.js...
LiveReload enabled
created public/build/bundle.js in 106ms

[2021-12-26 13:35:45] waiting for changes...

> svelte-app@1.0.0 start
> sirv public --no-clear "--dev"


  Your application is ready~! 🚀

  - Local:      http://localhost:5000
  - Network:    Add `--host` to expose

────────────────── LOGS ──────────────────

```

# Test
```bash
~/svelte-app/ $ curl localhost:5000
~/svelte-app/ $ 								<- Error 403

~/svelte-app/ $ curl 127.0.0.1:5000
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset='utf-8'>
	<meta name='viewport' content='width=device-width,initial-scale=1'>

	<title>Svelte app</title>

	<link rel='icon' type='image/png' href='/favicon.png'>
	<link rel='stylesheet' href='/global.css'>
	<link rel='stylesheet' href='/build/bundle.css'>

	<script defer src='/build/bundle.js'></script>
</head>

<body>
</body>
</html>
~/svelte-app/ $ 
```

---- 


[1]:	https://svelte.dev/tutorial/basics
[2]:	https://svelte.dev/docs
[3]:	https://svelte.dev/examples
[4]:	https://svelte.dev/repl