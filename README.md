# Redirecionamento de URL externa | Tray
O ecommerce tray não possuí redirecionamento de sub pasta (exemplo.com/sub-pasta/) para uma url externa.
> **Obs.:** Por motivos de segurança a Tray removeu a possibilidade de grande quantidade de código HTML. Bloqueando um simples redirect em páginas internas. Ou a utilização do JavaScript internamente.

## Como Funciona?
Toda vez que criar uma página interna com a classes mencionadas, o código irá verificar se essa classe existe, se existir vai pegar a url dentro do href e redirecionar após 1,3 segundos.

## Instalação
A instalação pode ser feita por dois caminhos descritos abaixo. Onde será necessário carregar um código JavaScript em todas as páginas da loja.

### Via Google Tag Manager
1. Acesse o [Google Tag Manager](https://tagmanager.google.com/) crie um container e um WorkSpace (_Caso já tenha só seguir para o passo 2_). [Como criar um Google Tag Manager Loja Tray](https://basedeconhecimento.tray.com.br/hc/pt-br/articles/6762108858139-Como-Integrar-o-Google-Tag-Manager-).
2. Adicionar uma nova tag.
3. em **Configuração da Tag** adicione a tag **HTML Personalizado**.
4. Copie e cole o código [redirecionador-url.html](https://github.com/murjunior/tray-toff/blob/main/redirecionador-url.html).
5. Em **acionamento** adicione "**All Pages**".
6. Dê um nome a Tag e salve ela.
7. Por último, você precisa ir a página "Visão Geral" no menu a esquerda, para "Publicar" as alterações realizadas e funcionar.

### Via Tema | Loja Tray
Em breve...

## Utilização
1. Crie uma página interna. [Como criar página Interna Loja Tray](https://basedeconhecimento.tray.com.br/hc/pt-br/articles/6735669122971-Como-Configurar-as-P%C3%A1ginas-Internas-).
2. No conteudo da página, clique no icone de inserir código.
3. Insira o código abaixo, alterando para a URL que deseja redirecionar. No exemplo abaixo estamos redirecionando para www.google.com.br.

```ruby
<div class="redirecionou veirificaclasse">
<a class="linkdosite" href="https://www.google.com.br/">Carregando...</a>
</div>
```

> O código não deve ser alterado, só altere especificamente o que está dentro das aspas (") a url.
