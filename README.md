# 🚀 Projeto Versionamento SENAI

## 📄 Descrição
Este projeto tem como objetivo praticar o uso de ferramentas de **controle de versão** (Git e GitHub) para gerenciar alterações de código, criar branches, realizar merges e resolver conflitos. A atividade simula situações reais de desenvolvimento colaborativo, mostrando a importância do versionamento para organização, segurança e colaboração.

## 🗂 Estrutura do projeto
- `index.txt` — arquivo HTML utilizado para demonstrar alterações em diferentes branches.

## 🎯 Objetivo
- Compreender como criar um repositório local e remoto.  
- Criar e gerenciar branches para desenvolvimento paralelo.  
- Realizar merge de branches e resolver conflitos.  
- Aplicar boas práticas de versionamento de código.

## 🛠 Passos realizados

### 1️⃣ Inicialização do repositório
```bash
git init
git status
```
- Criado repositório local vazio.
- Adicionado o arquivo `index.txt` ao versionamento:
```bash
git add index.txt
git commit -m "Adiciona arquivo index.txt"
```

### 2️⃣ Conexão com o repositório remoto
```bash
git remote add origin https://github.com/monnikys/versionamento-senai.git
git branch -M main
git push -u origin main
```
- Repositório remoto criado no GitHub.
- Primeira versão do arquivo publicada na branch `main`.

### 3️⃣ Criação da branch `feature1`
```bash
git checkout -b feature1
git push -u origin feature1
```
- Branch criada para simular desenvolvimento paralelo.
- Modificações realizadas no `index.txt` na branch `feature1`:
```bash
  <H1> GIT </H1>
```

### 4️⃣ Alterações na branch main
- Alteração realizada na branch `main`:
```bash
<H1> VERSIONAMENTO </H1>
```
- Commit realizado:
```bash
git add index.txt
git commit -m "Atualiza título para VERSIONAMENTO"
git push
```

### 5️⃣ Merge da branch `feature1` na `main`
```bash
git checkout main
git merge feature1
```

- ⚠️ Conflito detectado no arquivo `index.txt`.
- Resolução do conflito manualmente, consolidando as duas alterações:
```bash
<H1> VERSIONAMENTO E GIT </H1>
```
- Commit final:
```bash
git add index.txt
git commit -m "Resolve conflito entre main e feature1"
git push
```

## ✅ Boas práticas aplicada
* 📝 Commits pequenos e frequentes.
* ✏️ Mensagens de commit claras e descritivas.
* 🌿 Uso de branches para novas funcionalidades.
* 🔄 Atualização do repositório local antes de trabalhar (`git pull`).
* ⚡ Resolução cuidadosa de conflitos.
* 📂 Organização do histórico de versões.

## 🎉 Resultado final
O arquivo `index.txt` consolidou as alterações de ambas as branches,
mostrando como o Git permite conciliar mudanças diferentes de maneira segura e organizada.

## 🏁 Conclusão
Esta atividade demonstrou a importância do versionamento de código para o desenvolvimento de projetos colaborativos.
A prática permitiu compreender como trabalhar com branches, commits, merge e resolução de conflitos,
além de reforçar boas práticas essenciais para manter o projeto organizado, seguro e colaborativo.
