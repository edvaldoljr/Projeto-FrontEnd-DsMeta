

# **Projeto DSM Meta**

![](https://github.com/edvaldoljr/Projeto-FrontEnd-DsMeta/blob/main/img/img-projeto.gif?raw=true)

Este código é um documento HTML que descreve um site chamado "DSMeta". O site inclui um cabeçalho com um logotipo, um título e um link para a página do Instagram do desenvolvedor. A seção principal da página exibe dados de vendas em um formato de tabela, incluindo data, fornecedor, número de visitas e vendas, valor total e um botão de notificação. O código CSS vinculado a este documento HTML define a fonte padrão como "Roboto" e define o estilo padrão para elementos como margem e preenchimento.

## Para desenvolver o projeto DSM Meta, são necessários os seguintes requisitos:

- Conhecimento básico de HTML e CSS
- Entender a estrutura de uma página web.
- Conhecer as propriedades de estilo CSS para customizar a aparência da página.
- Testar o projeto em diferentes dispositivos e navegadores para garantir compatibilidade.

## Index.hml

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="styles.css" />
    <title>DSMeta</title>
  </head>
  <body>
    <header>
        <div class="dsmeta-logo-container">
            <img src="logo.svg" alt="DSMeta" />
            <h1>DSMeta</h1>
            <p>
              Desenvolvido por
              <a href="https://www.instagram.com/programando.dev/" target="_blank">@programando.dev</a>
            </p>
        </div>
    </header>
    <main>
        <section id="sales">
            <div class="dsmeta-container">
                <div class="dsmeta-card">
                    <h2 class="dsmeta-sales-title">Vendas</h2>
                    <div>
                        <div class="dsmeta-form-control-container">
                            <input class="dsmeta-form-control" type="text">
                        </div>
                        <div class="dsmeta-form-control-container">
                            <input class="dsmeta-form-control" type="text">
                        </div>
                    </div>
                    <div>
                        <table class="dsmeta-sales-table">
                            <thead>
                                <tr>
                                    <th class="show992">ID</th>
                                    <th class="show576">Data</th>
                                    <th>Vendedor</th>
                                    <th class="show992">Visitas</th>
                                    <th class="show992">Vendas</th>
                                    <th>Total</th>
                                    <th>Notificar</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td class="show992">#341</td>
                                    <td class="show765">03/04/1994</td>
                                    <td>Anakin</td>
                                    <td class="show992">15</td>
                                    <td class="show992">11</td>
                                    <td>R$ 55300.00</td>
                                    <td>
                                        <div class="dsmeta-red-btn-container">
                                            <div class="dsmeta-red-btn">
                                                <img src="notification-icon.svg" alt="Notificar">
                                            </div>
                                        </div>
                                        </td>
                                </tr>
                                <tr>
                                    <td class="show992">#341</td>
                                    <td class="show765">03/04/1994</td>
                                    <td>Anakin</td>
                                    <td class="show992">15</td>
                                    <td class="show992">11</td>
                                    <td>R$ 55300.00</td>
                                    <td>
                                        <div class="dsmeta-red-btn-container">
                                            <div class="dsmeta-red-btn">
                                                <img src="notification-icon.svg" alt="Notificar">
                                            </div>
                                        </div>
                                    </td>
                                </tr>
                                <tr>
                                    <td class="show992">#341</td>
                                    <td class="show765">03/04/1994</td>
                                    <td>Anakin</td>
                                    <td class="show992">15</td>
                                    <td class="show992">11</td>
                                    <td>R$ 55300.00</td>
                                    <td>
                                        <div class="dsmeta-red-btn-container">
                                            <div class="dsmeta-red-btn">
                                                <img src="notification-icon.svg" alt="Notificar">
                                            </div>
                                        </div>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </section>
    </main>
  </body>
</html>



```

Este código HTML cria uma página web que mostra informações sobre vendas. O código está estruturado com uma tag <header> para criar um cabeçalho com uma imagem e um título do site, seguido de uma seção <main> que contém uma seção <section id="sales"> que exibe as informações de vendas.

Dentro da seção de vendas, há um contêiner com uma classe "dsmeta-container" e uma classe "dsmeta-card". O contêiner inclui duas caixas de entrada de formulário com classe "dsmeta-form-control-container" e uma tabela com informações sobre as vendas. A tabela tem uma classe "dsmeta-sales-table" e inclui uma linha de cabeçalho e várias linhas de dados para cada venda.

As colunas da tabela incluem "ID", "Data", "Vendedor", "Visitas", "Vendas", "Total" e "Notificar". A coluna "Notificar" contém um botão com uma imagem de notificação.

O código também está estilizado com um arquivo CSS externo "styles.css".

## Style.css

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap");

* {
  font-family: "Roboto", sans-serif;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body,
html {
  background-color: #000;
  color: #ffffff;
}

a,
a:hover,
a:visited {
  color: unset;
  text-decoration: none;
}

header {
  background: linear-gradient(180deg, #102347 0%, #181818 100%);
  height: 220px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.dsmeta-logo-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.dsmeta-logo-container img {
  width: 235px;
}

.dsmeta-logo-container h1 {
  margin-top: 15px;
  font-size: 24px;
}

.dsmeta-logo-container p {
  font-size: 14px;
  font-weight: 300;
}

.dsmeta-card {
  background-color: #283142;
  border-radius: 10px;
  padding: 30px 10px;
}

.dsmeta-container {
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
}

#sales {
  padding: 40px 10px;
}

.dsmeta-sales-title {
  color: #676fff;
  font-size: 24px;
  margin-bottom: 20px;
}

.dsmeta-form-control-container {
  margin-bottom: 16px;
  max-width: 300px;
}
.dsmeta-form-control {
  width: 100%;
  height: 46px;
  background-color: #1b2531;
  border: 1px solid #384459;
  border-radius: 5px;
  color: #9aaabe;
  padding: 0 20px;
  font-size: 18px;
}

.dsmeta-sales-table {
  width: 100%;
  border-spacing: 0;
  border-collapse: collapse;
}

.dsmeta-sales-table thead {
  height: 55px;
  font-size: 16px;
  color: #e9e9e9;
  font-weight: 700;
}

.dsmeta-sales-table tbody {
  font-size: 14px;
  font-weight: 400;
  color: #cfcfcf;
  text-align: center;
}

.dsmeta-sales-table tbody tr {
  height: 74px;
  border-top: 1px solid #5f6e82;
}

.dsmeta-sales-table tbody tr:hover > td {
  background-color: #384459;
}

.dsmeta-sales-table tbody tr:nth-child(odd) {
  background-color: #242c3b;
}

.dsmeta-red-btn-container {
    display: flex;
    justify-content: center;
}

.dsmeta-red-btn {
  height: 45px;
  width: 45px;
  background: rgba(255, 107, 114, 0.1);
  border: 1px solid #ff6b72;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.dsmeta-red-btn img {
    width: 19px;
}

.show576 {
    display: none;
}

.show992 {
    display: none;
}

@media (min-width: 576px) {
    .show576 {
        display: table-cell;
    }

.dsmeta-card {
    padding: 35px;
    }

.dsmeta-sales-table tbody tr {
    height: 55px;
    }

.dsmeta-sales-table tbody {
    font-size: 18px;
    }
}

@media (min-width: 992px) {
.show992 {
    display: table-cell;
}
}


```

Este é um trecho de código CSS, que é uma linguagem usada para estilizar elementos HTML na web. Este código define a aparência e formatação de um site. Ele inclui definições de fontes, cores, espaçamentos, bordas, tamanhos de texto, etc. Além disso, o código inclui também regras de responsividade, ou seja, como o site se adapta a diferentes tamanhos de tela, usando a media query.

## Acesso o Link e confira: https://edvaldoljr.github.io/Projeto-Devsuperior-Aquecimento-Semana-Spring-React/


# ⭐️**Deixe um Star** ⭐️

Obrigado por conferir meu repository! É muito gratificante saber que alguém está interessado no meu trabalho. Se você gostou do que viu, deixar um star seria uma grande ajuda no meu crescimento e me motivaria a continuar fazendo projetos. O apoio de pessoas como você é fundamental para que eu possa seguir evoluindo e produzindo conteúdos cada vez melhores. Obrigado mais uma vez e espero que você possa acompanhar meus futuros projetos!
