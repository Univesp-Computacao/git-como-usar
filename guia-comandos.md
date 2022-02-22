# Guia de Comandos

### Escolher o nome que você quer anexar às suas transações de commmit:
```bash
git config --global user.config [digite-seu-nome]
```

### Escolher e-mail que vcê quer anexar aos seus commits:
```bash
git config --global user.config [digite-seu-nome]
```
### Ativar colorização da linha de comandos :
```bash
git config --global color.ui auto
```
### Criar um novo repositório local:
```bash
git init [project-name]
```

### Fazer o download de um projeto e toda história de versões:
```bash
git clone [url] 
```

### Listar todos arquivos novos ou modificações  a serem comitadas (status):
```bash
git status
```

### Mostrar diferenças entre arquivos que ainda não foram adicionados:
```bash
git diff 
```

### "Capturar" o arquivo em preparação para o verisonamento: 
```bash
git add [nome-do-arquivo.html] [outro-arquivo.py] 
```
ou para adicionar todos
```bash
git add .  
```

### Mostrar as diferenças entre arquivos que estão na área de staging e os arquivos da últikma versão:
```bash
git diff --staged 
```




