```bash
git checkout --orphan nova-branch
git add -A
git commit -m "coloque-algo-aqui"
git branch -D main
git branch -m main
git push -f origin main
```

Se você já está familiarizado com o processo de clonagem de repositórios e navegação pelo terminal, mas quer saber o comando, ai está. Substitua `coloque-algo-aqui` pela mensagem que deseja para o novo commit.

---
Neste tutorial, vou explicar como limpar todo o histórico de commit de um repositório Git, mantendo apenas a última alteração. Esse processo é útil quando você deseja iniciar um novo histórico de commit a partir do último estado do seu projeto.
## Pré-requisitos:

- Git instalado no seu sistema.
- Acesso ao terminal ou prompt de comando.
## Clone o Repositório

Se você ainda não possui uma cópia do repositório em seu computador, clone-o seguindo estas etapas:

No terminal, navegue até o diretório onde deseja clonar o repositório, usando o comando `cd`.

```bash
cd caminho/para/onde/quer/clonar
```

Substitua `caminho/para/onde/quer/clonar` pelo diretório desejado em seu sistema.

Em seguida, clone o repositório usando o comando `git clone` seguido da URL do repositório:

```bash
git clone cole-a-url-aqui
```

Substitua `cole-a-url-aqui` pela URL do repositório que você deseja clonar. Por exemplo:

```bash
git clone https://github.com/secwired/LABS.git
```

![](https://img001.prntscr.com/file/img001/mG2Kw2GuTQW7s2a721gnrQ.png)
![](https://img001.prntscr.com/file/img001/8_aqD6nxSPyZNC-pX1dI5g.png)
![](https://img001.prntscr.com/file/img001/paxrZ5hHRbihthOF-OuiOQ.png)

Note que eu tenho **47 Commits** nesse repositório.

## Executando o comando
Vá até a pasta que está o repositório clonado, clique com o botão direito no espaço vazio e abra no Terminal ou Git Bash e cole o comando:

```bash
git checkout --orphan nova-branch
git add -A
git commit -m "coloque-algo-aqui"
git branch -D main
git branch -m main
git push -f origin main
```

![](https://img001.prntscr.com/file/img001/SNbU5pIRQT2DC6r9Ped-AQ.png)

Ao abrir o **terminal** e colar o comando, vai aparecer um aviso, clique em "Colar mesmo assim" e confirme você vai precisar dar enter mais uma vez para terminar.

![](https://img001.prntscr.com/file/img001/bjcM7zlWQaqTA_j6p2omhA.png)
![](https://img001.prntscr.com/file/img001/zASQvkExQneoB72rEKq-kA.png)

Se for abrir no **Git**, basta colar e dar enter.

![](https://img001.prntscr.com/file/img001/HzABvGmvTuC_DDvyK0pGNA.png)

Prontinho.

![](https://img001.prntscr.com/file/img001/fONV3s3IQSye4d-9JYuzTQ.png)

Note que agora só ficou **1 Commit**.

**O que o comando faz?**
- `git checkout --orphan nova-branch`: Cria uma nova branch sem histórico.
- `git add -A`: Adiciona todos os arquivos ao novo commit.
- `git commit -m "coloque-algo-aqui"`: Cria um novo commit com todos os arquivos.
- `git branch -D main`: Exclui a antiga ramificação `main`.
- `git branch -m main`: Renomeia a ramificação atual para `main`.
- `git push -f origin main`: Força o envio do novo histórico para o repositório remoto.
## Material complementar:

- [Playlist: Curso de Git e GitHub - Curso em Vídeo](https://www.youtube.com/playlist?list=PLHz_AreHm4dm7ZULPAmadvNhH6vk9oNZA)
- [Entendendo GIT | (não é um tutorial!) - Fabio Akita](https://youtu.be/6Czd1Yetaac)
- [Usando Git Direito | Limpando seus Commits! - Fabio Akita](https://youtu.be/6OokP-NE49k)