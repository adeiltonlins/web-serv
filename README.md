# web-serv
//Para funcionar é preciso instalar o pacote express no diretório #npm install express

const express = require('express') //aqui estamos fazendo a importação da biblioteca
const app = express() //criando uma instância para a constante app

app.get('/', (req, res) => {
    const result = { name: 'ana', instagram: 'anajose' };
    return res.json(result);
  });

app.listen(8080,() =>{
    console.log("Servidor funcionando ") //o que aparece no terminal
})
