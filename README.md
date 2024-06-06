Aprendendo desenvolver uma API

Comando para executar cmd após montar a estrutura e testar no Code .

dotnet restore
dotnet build
dotnet run


CRIAÇÃO DO CRUD.

Instalado INSOMNIA.

Deu um pequeno erro mas corrigido com desmancando VALIDATE CERTIFICATES, é necessário no caso de estudo que não há certificações.

Get ler projetos existentes.

Post inserir novos projetos.

Put modificado os projetos.

Delete exclui o projeto 4.


CRIAR CRUD DE USUÁRIOS.

Iniciar criando as classes que faltam e fazendo/adicionando novas linhas e complementos.

Criar classe/Controllers = UsuarioController.cs
Criar classe/Models = Usuario.cs
Criar classe/Repositories = UsuarioRepository.cs
Adicionar/ExoContexts = Controllers - inserir complemento apontando para usuario "Public DbSet<Usuario>Usuarios { get, set, }
Adicionar/Program.cs = builder.Services.AddTransient<UsuarioRepository>();

Após a criação ira gerar = https://localhost:7154
Carregue a pagina e complemente = https://localhost:7154/api/usuarios
No navegador irá aparece a linha = [{"id":1,"email":"email@sp.br","senha":"1234"},{"id":2,"email":"email_dois@sp.br","senha":"1234"}]
Fazer testes do CRUD NO INSOMNIA.
Fazer testes GET/POST/PUT/DELETE.
Lembrando que o numero ou sequência de ID é automático, não sendo necessário adicionar no JASON durante a criação.

[
	{
		"id": 1,
		"email": "email@sp.br",
		"senha": "1234"
	},
	{
		"id": 2,
		"email": "email_dois@sp.br",
		"senha": "1234"
	},
	{
		"id": 5,
		"email": "email_tres@sp.br",
		"senha": "1234"
	}
]

Também é possível buscar usuário por ID= colocando o número desejado.

