1°
npm init -y

2°
npm i -D typescript
3°
 npx tsc --init

(tscofing = colocar essa configuração

EX: TSCONFIG{
"compilerOptions": {
"target": "ES2020",
"module": "CommonJS",
"strict": true,
"esModuleInterop": true,
"forceConsistentCasingInFileNames": true,
"skipLibCheck": true,
"outDir": "./dist"
},
"include": ["src", "test"]
})


4°
npm i -D tsc
crie uma pasta chamada "src" depois um arquivo "server.ts"

5°
criar um script chamado: "start": "node --import=tsx --watch ./src/server.ts"


6°
npm i express(biblioteca para criar o servidor)


7°
npm i -D @types/experss



//codigo no server.ts

import express from "express"

const server = express()

//rotas
server.get("/", (req,res) => {
   res.send("Olá Everson!")
})

//iniciar o servidor
server.listen(3000,() => {
console.log("Tudo está funcionando no link http://localhost:3000/")
})


8°
ligar o servidor: npm start



9°
npm i helmet



10°
npm i -D @types/helmet

npm uninstall -D tsc (se algo der errado, isso serve para desinstalar)



