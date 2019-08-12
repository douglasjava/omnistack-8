This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### 
- A aplicação é renderizada a partir do arquivo index.js -> o mesmo imbute um componente dentro do html via javaScript
- [  ReactDOM.render(<App />, document.getElementById('root')) ] --> '<App/>' é um componente que por padrão é uma função que retorna um conteúdo HTML

- Instalar dependencia de rotas ==> yarn add react-router-dom
- Criar arquivo Routes.js -> Onde ficaram as rotas da aplicação
- Importar o arquivo Routes no app.js
- É necessário colocar o parametro [exact] no componente Router para que considere todo o caminho colocado na url
- [ e.preventDefault(); ] Previne comportamento padrão de submit de formulário
- Arrow functions ==> [ const handleSubmit = (e) => { ] o mesmo que [ function handleSubmit(e) {]

- Passando informações entre os componentes 
	- No componente posso escrever o 'parametro="x"' ai dentro do componente [ export default function Login(props) { ] que é uma função ai pegaria utilizando [props]
	  props.parametro (o nome do parametro passado)
	- Por padrão é passado um parametro [ history ] que server para fazer navegação
	- o método [push] redireciona-ra para outra rota ex [ history.push('/main') ]

- Instalar o axios [ yarn add axios ] -- responsável para realizar requiciçoes.

- Existe o propriedade [ match ] que consigo recuperar todos os parametros que foram passados para essa rota 

- Observação:
 Para alterar um valor de variável não pode alterar a variável a primeira 
	[ const [ users, setUsers ] = useState([]); ] nesse caso o correto é alterar a função (setUsers) sobreescrevendo o valor para assim refletir na variável que é exibida.