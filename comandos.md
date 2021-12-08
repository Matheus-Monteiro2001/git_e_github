////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
--****

--Inicializar repositorio vazio

git init

--Adiciona um arquivo à área de teste do Git
(Esta área contém uma lista de todos os arquivos que você alterou recentemente.)
(Seu repositório será atualizado na próxima vez que você criar um commit com suas mudanças.)
(Portanto, executar o comando git add não altera seu trabalho no repositório Git)

git add NOME_DO_ARQUIVO_QUE_VC_QUER_MANDAR

-> Nesse caso é adicionado tudo que esta no seu diretorio(pasta e conteudo dento da pasta)

git add .

--Mostra os status do commit

git status

--Iniciar o primeiro commit

git commit -m "MENSAGEM DO COMMIT"

--Renomear a branch master para main

git branch -M "main"

--Para adicionar um origin para o repositório se não existe nenhum.
(Isso é útil quando se deseja iniciar um repositório localmente com "git init" e, em seguida, é necessário enviá-lo para um repositório remoto mais tarde.)

git remoto adicionar origem https://github.com/CAMINHO_PARA_A_PASTA_CRIADA_NO_GITHUB. git

--
(O comando git push é mais usado para publicar modificações locais a um repositório central. Após um repositório local ter sido modificado, um comando push é executado para compartilhar as modificações com membros da equipe remota.)
(Origin é o nome padrão do repositório git remoto do qual você clonou.) 

git push -u origin main

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
--**Ou crie um novo repositório na linha de comando**

echo "# -NOMA_DA_PASTA_NO_GITHUB" >> README.md 
git init 
git adicionar README.md 
git commit -m "primeiro commit" 
git branch -M principal 
git remoto adicionar origem https://github.com/CAMINHO_PARA_A_PASTA_CRIADA_NO_GITHUB. git
 git push -u origin main

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
--**Ou envie um repositório existente a partir da linha de comando**

git remote add origin https://github.com/CAMINHO_PARA_A_PASTA_CRIADA_NO_GITHUB. git
git branch -M main 
git push -u origin main

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
--**Se realizou alteracoaes no projeto e deseja atualizar no repositorio**

git add .

git status

git commit -m "MENSAGEM DO 2 COMMIT"

git push origin main

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
--**Criar nova ramificacao do projeto(branches)**

git checkout -b "NOME_DA_RAMIFICACAO"

git add .

git commit -m "MENSAGEM DO 3 COMMIT(RAMIFICACAO)"

git push origin NOME_DA_RAMIFICACAO

--para voltar a branche desejada

git checkout NOME_DA_BRANCHE

--para juntar as 2 branche

git merge NOME_DA_BRANCHE

--mandar todas as alteracoes

git push origin main

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
--**Clonar repositorio do github**

git clone https://github.com/CAMINHO_PARA_A_PASTA_CRIADA_NO_GITHUB. git

--para atualizar para a versao mais nova

git pull

