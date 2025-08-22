# Repositorio-GetStarted-K1-T1
O Git é uma ferramenta de controle de versão que ajuda a rastrear e gerenciar alterações no código-fonte. Desevolvido pelo famoso Linus Torvalds tambem criador do sistema operacional Linux.


### **Iniciando um Repositório**

* `git init`: Inicializa um novo repositório Git no diretório atual.
* `git clone <url>`: Cria uma cópia local de um repositório remoto.

### **Salvando Alterações (Commiting)**

* `git status`: Exibe o estado da árvore de trabalho e do *staging area*, mostrando arquivos modificados, novos ou que ainda não foram rastreados.
* `git add <arquivo>`: Adiciona um arquivo para o *staging area*, preparando-o para o próximo *commit*. Use `git add .` para adicionar todos os arquivos.
* `git commit -m "Mensagem"`: Salva as alterações do *staging area* no histórico do repositório. A mensagem deve ser descritiva.
* `git commit -am "Mensagem"`: Combina `git add .` e `git commit -m` para arquivos que já estão sendo rastreados.

---

### **Gerenciando o Histórico e Ramificações (Branches)**

* `git log`: Exibe o histórico de *commits* do repositório.
* `git branch`: Lista todas as ramificações locais.
* `git branch <nome-da-branch>`: Cria uma nova ramificação.
* `git checkout <nome-da-branch>`: Muda para uma ramificação existente. Use `git checkout -b <nova-branch>` para criar e mudar para uma nova ramificação de uma vez.
* `git merge <nome-da-branch>`: Integra o histórico de uma ramificação na ramificação atual.
* `git diff`: Mostra as diferenças entre a árvore de trabalho e o *staging area* ou entre *commits*.

---

### **Sincronizando com Repositórios Remotos**

* `git remote add origin <url>`: Associa um repositório remoto local a uma URL.
* `git push -u origin <nome-da-branch>`: Envia os *commits* locais para o repositório remoto. O `-u` define o *upstream branch*, para que os próximos `git push` não precisem de argumentos.
* `git pull`: Baixa e integra as alterações do repositório remoto para o repositório local.
* `git fetch`: Baixa as alterações do repositório remoto, mas não as integra ao repositório local, permitindo que você as revise primeiro.

---

### **Desfazendo Alterações**

* `git reset <arquivo>`: Remove um arquivo do *staging area*.
* `git restore <arquivo>`: Desfaz as alterações feitas em um arquivo na sua árvore de trabalho.
* `git revert <hash-do-commit>`: Cria um novo *commit* que desfaz as alterações de um *commit* anterior, mantendo o histórico.

https://git-scm.com/doc