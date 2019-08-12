# OmniStack

<p align="center">
	<img src="https://img.shields.io/badge/Language-JavaScript-orange.svg">
	<img src="https://img.shields.io/badge/Latest%20Update-07/03/2019-brightgreen.svg">
</p>

## Funcionamento

- Criar projeto node init
- Criar arquivo server.js 
	- Nele é configurado acesso ao banco, formato Json, Rotas, Porta de acesso.
- Criar Models(Entidades) com Mongo e exporta passando O nome e o Schema [module.exports = model('Dev', DevSchema);]
- Criar Classe de rota(Routes) 
	- Nela é configurado as rotas da aplicação a partir de qual link e para onde será encaminhado para um controller
	- [const routes = express.Router();]
	- [routes.post('/devs', DevController.store);]
- Criar classes de controller
	- Nela só deverá existir os seguintes métodos [INDEX, SHOW, STORE, UPDATE, DELETE], saindo disso é uma boa prática criar um novo controller

## Code scaffolding

Application create for week omniStack

Made in the [Semana OmniStack](https://www.rocketseat.com.br/) course by [Diego Fernandes](https://github.com/diego3g)

Author: [Douglas Dias](https://github.com/douglasjava)

## License ##

[MIT](LICENSE)