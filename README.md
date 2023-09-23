# Redirecionamento de URL externa | Tray
O ecommerce tray não possuí redirecionamento de sub pasta (exemplo.com/sub-pasta/) para uma url externa.
> **Obs.:** Por motivos de segurança a Tray removeu a possibilidade de grande quantidade de código HTML. Bloqueando um simples redirect em páginas internas. Ou a utilização do JavaScript internamente.

## Como Funciona?
Toda vez que criar uma página interna com a classes mencionadas, o código irá verificar se essa classe existe, se existir vai pegar a url dentro do href e redirecionar após 1,3 segundos.

## Instalação
A instalação pode ser feita por dois caminhos descritos abaixo. Onde será necessário carregar um código JavaScript em todas as páginas da loja.

### Via Google Tag Manager
1. Acesse o [Google Tag Manager](https://tagmanager.google.com/) crie um container e um WorkSpace. [Como criar um Google Tag Manager Loja Tray](https://basedeconhecimento.tray.com.br/hc/pt-br/articles/6762108858139-Como-Integrar-o-Google-Tag-Manager-).
2. Adicionar uma nova tag.
3. em **Configuração da Tag** adicione a tag **HTML Personalizado**.

### Via Tema | Loja Tray
Em breve...
