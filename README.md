# Blog do código
> Um blog simples em Node.js

npm install express nodemon body-parser sqlite3

// TESTE DE CUSTO DE TEMPO PARA BCRYPT 

const bcrypt = require('bcrypt');    
for (let custo = 6; custo < 18; custo++) {
  const tempoInicial  = Date.now();
  bcrypt.hash('A', custo).then(
    () => console.log(`custo: ${custo}; tempo: ${ Date.now() - tempoInicial} ms`)
  );
} 