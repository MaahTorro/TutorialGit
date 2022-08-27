## Conceitos e dicionario

### Remote
Damos o nome de remote ao servidor git de origem que guarda o nosso repositorio (github por exemplo), um mesmo repositorio git local pode suportar varios remotes por incrivel que pareça, na maioria das vezes usamos uma so mesmo

### Branch
Branch eh uma bifurcacao do nosso repositorio, podemos ter infinitas e elas sao separadas por nome, geralmente a branch padrao se chama “master” ou “main”, 

“master” eh o nome padrao do git enquanto “main” eh o nome padrao do github, no seu caso configurei para q o padrao seja main no git tambem

Exemplos de branch para entender um pouco melhor:
- main
- dev (vamos supor que aqui se concentra alteracoes que estao em desenvolvimento)
- release_v_1_0_0 (vamos supor que aqui esta a versao 1.0.0 desse projeto)
- add_readme (vamos supor que essa foi uma branch criada especificamente para adicionar um README para o projeto)

Vale lembrar que ao criar uma branch ela usara SEMPRE como base a branch em que voce estava antes

### Commit
Um/cada commit representa um ponto no historico de alteracoes do git ele alem de te apresentar quais arquivos foram alterados e quais alteracoes foram feitas tambem mostra quem foi o autor e uma breve descricao desse autor sobre oq foi alterado

### Fazer um Pull
Chamamos de pull a acao de puxar as alteracoes para o nosso git local, por exemplo, outro contribuidor do projeto fez um commit para a mesma branch que voce esta trabalhando, ai para pegar as alteracoes que ele fez vc tem que puxar as alteracoes

### Fazer um Push
Ao contrario do pull, nesse caso estamos enviando as nossas alteracoes do nosso git local para o remote

### Fazer um Merge ou realizar conflitos de Merge
Chamamos de merge quando queremos juntar uma branch na outra, por exemplo, se fizermos um merge da branch “main” para a branch “production” a branch production recebera todas as alteracoes que a “main” possue

As vezes quando realizamos um merge pode ocorrer de existir um “merge conflict” isso significa que um ou mais arquivos presentes em ambas as branchs tiveram alteracoes diferentes e o git nao consegue juntar-las automaticamente, para esse caso o git abrira o editor de texto para merge conflict escolhido para que o autor do merge resolva o conflito manualmente (no seu caso configurei para que seja o VS Code). Nisso basta ver as 2 versoes do mesmo arquivo e, escolher um dos 2 ou ambos, organizando como o arquivo final deve ficar.

Tenha muita calma e atencao ao fazer resolver um Merge Conflict

### Repositorio
Repositorio representa uma pasta em que o git esta atuando, basicamente nosso projeto ou codigo

### Stage ou staging
Essa palavra aparece quando nossos arquivos estao em staging, quando nossos arquivos estao em staging quer dizer que o proximo commit tera esses arquivos como suas alteracoes