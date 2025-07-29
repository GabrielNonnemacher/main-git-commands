# 📘 Principais Comandos Git
Para mais informações consulte a documentação oficial: https://git-scm.com/docs

## 🔧 Configuração Inicial
Define o nome e email do usuário para todos os repositórios locais.
<pre><code>git config --global user.name "Seu Nome"</code></pre>

<pre><code>git config --global user.email "seu@email.com"</code></pre>


## 🆕 Iniciar e Clonar Repositórios
Cria um novo repositório Git vazio no diretório atual.
<pre><code>git init</code></pre>

Clona um repositório remoto para o seu computador.
<pre><code>git clone https://github.com/usuario/repositorio.git</code></pre>


## 📁 Status e Histórico
Mostra arquivos modificados, adicionados, não rastreados e o branch atual.
<pre><code>git status</code></pre>

Exibe o histórico de commits.
<pre><code>git log</code></pre>

Exibe o log resumido (um commit por linha).
<pre><code>git log --oneline</code></pre>


## ➕ Adicionar e Confirmar Alterações
Adiciona arquivos ao stage (prepara para commit).
<pre><code>git add nome-do-arquivo</code></pre>
<pre><code>git add .</code></pre>

Cria um commit com os arquivos adicionados.
<pre><code>git commit -m "Mensagem do commit"</code></pre>


## 🔁 Branches
Lista todas as branches locais.
<pre><code>git branch</code></pre>

Cria uma nova branch.
<pre><code>git branch nome-da-branch</code></pre>

Troca para outra branch.
<pre><code>git checkout nome-da-branch</code></pre>

Cria e troca para a nova branch.
<pre><code>git checkout -b nova-branch</code></pre>

Mescla a nome-da-branch na branch atual.
<pre><code>git merge nome-da-branch</code></pre>

Deleta uma branch local.
<pre><code>git branch -d nome-da-branch</code></pre>


## 🌐 Repositórios Remotos
Adiciona um repositório remoto.
<pre><code>git remote add origin https://github.com/usuario/repositorio.git</code></pre>

Envia a branch main para o repositório remoto e define como upstream.
<pre><code>git push -u origin main</code></pre>

Envia commits locais para o repositório remoto.
<pre><code>git push</code></pre>

Baixa alterações do repositório remoto e mescla na branch atual.
<pre><code>git pull</code></pre>


## 🔄 Sincronização
Busca alterações do repositório remoto, mas não mescla.
<pre><code>git fetch</code></pre>

Reaplica os commits locais sobre os commits do repositório remoto (útil para manter histórico limpo).
<pre><code>git rebase origin/main</code></pre>


## 🧼 Desfazendo Alterações
Remove o arquivo do stage (não desfaz mudanças).
<pre><code>git reset nome-do-arquivo</code></pre>

Desfaz alterações locais em um arquivo (restaura do último commit).
<pre><code>git checkout -- nome-do-arquivo</code></pre>

Descarta todas as mudanças e volta ao último commit.
<pre><code>git reset --hard</code></pre>


## 🧪 Stash (Guardar Mudanças Temporariamente)
Guarda alterações não commitadas.
<pre><code>git stash</code></pre>

Restaura as alterações salvas.
<pre><code>git stash apply</code></pre>


## 🔍 Visualização e Diferenças
Mostra as diferenças entre os arquivos modificados e o último commit.
<pre><code>git diff</code></pre>

Mostra as mudanças feitas em um commit específico.
<pre><code>git show <commit></code></pre>


## 🔚 Outros Úteis
Remove um arquivo e marca a remoção para o próximo commit.
<pre><code>git rm nome-do-arquivo</code></pre>

Renomeia um arquivo.
<pre><code>git mv antigo.txt novo.txt</code></pre>
