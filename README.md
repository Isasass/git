# git

## git init
Inicializacao de um projeto:
```bash
git init
```

## Configuracoes iniciais
```bash
git config --global user.name "username"
it config --global user.email "user@email.com"
```

## controle de alteracoes
Para visualizar as alteracoes feitas, vamos usar:
```bash
git status
```

## criando commits
primeiramente precisamos adicionar as mudancas e enfim 'commitar': 
> utilize o ponto para adicionar todas as alteracoes do projeto.
```bash
git add .
git commit - "descricao das alteracoes" 
```

## Branches

- Podemos ramificar o codigo usando branches para criar uma nova, executamos:
```bash
git switch --create <nome-da-nova-branch>
# or
git chekout -b <nome-da-nova-branch>
```

- Listando branches criadas: 
```bash
git branch
```

- Apagando branch
```bash
git branch -D <nome-da-branch>
```

### GitHub
- adicionando um remote origin:
```bash
git remote add origin https://github.com/user/repo-name.git
```
-Subindo alteracoes: 
```bash
git push origin <nome-da-branch>
# caso a branch nao exista no GitHub use: 
git push -u origin <nome-da-branch> # ele criara a branch no GitHub
```