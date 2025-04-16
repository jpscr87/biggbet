<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://i.ibb.co/t84wtb7/p6-UVIf-Jyzbp-Sz-Bt-Kl-Xdg-P4i34-An-NOAp3rmck-DUe-S.png" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Viper Pro

>Viperpro é um projeto de código aberto desenvolvido em PHP utilizando o Framework Laravel 10 e Vue 3,
com várias integrações com diferentes provedores de iGaming. Este projeto é destinado para fins de estudo.
Use-o com responsabilidade e consciência, e não o utilize para fins fraudulentos. 

>Viperpro is an open-source project developed in PHP using the Laravel 10 Framework and Vue 3,
featuring multiple integrations with different iGaming providers. This project is intended for educational purposes.
Use it responsibly and ethically, and do not use it for fraudulent activities.

## PLATAFORMAS DE QUALIDADES
>Se você busca plataformas de qualidade com excelente custo-benefício, acesse nosso site! Lá, você encontrará soluções completas e avançadas, incluindo documentação detalhada. 
E o melhor: ao adquirir o código-fonte, você ganha 90 dias de suporte gratuito. Aproveite!

>If you're looking for high-quality platforms with excellent cost-effectiveness, visit our website! There, you'll find complete and advanced solutions, including detailed documentation.
And the best part: when you purchase the source code, you get 90 days of free support. Take advantage of it!

Site Oficial:

https://viper.casino 

Instagram:

https://www.instagram.com/venix.app/

## Login Admin
> Para acessar o painel de administração, basta acessar a URL que termina com /admin e inserir suas credenciais de acesso.
> To access the admin panel, simply navigate to the URL ending with /admin and enter your login credentials.
```php
E-mail: admin@demo.com
Senha: 123456
```
## Trocando a rota do admin

Se você deseja alterar a rota do painel administrativo, é muito simples: basta acessar o arquivo de configuração correspondente e modificar o caminho desejado.
```
app/Providers/Filament/AdminPanelProvider.php
```

Altere:
```php
->id('admin')
->path('admin')
```

## ATUALIZAÇÔES
### Versão 1.6.1
Esta versão conta com diversas correções e melhorias, deixando a plataforma totalmente pronta para o seu uso. Já está integrada ao nosso provedor de jogos Venix, com jogos carregados, e também com o gateway de pagamento da Sharkpay, que já está configurado. Basta acessar o site, criar sua conta e dar o start.

This version includes several fixes and improvements, making the platform fully ready for you to start. It is already integrated with our game provider Venix, with games loaded, and the payment gateway from Sharkpay is also configured. Just visit the website, create your account, and get started.

>Caso queiram novos gateway e provedores, fazemos também esse tipo de serviço, consulte em nosso site https://viper.casino

## BAIXEM A VERSÂO RELEASE AO LADO -------------->


### Versão 1.6.0

### SISTEMA DE VIP

#### O que é?
O **Sistema VIP** foi reformulado e agora possui uma mecânica que contabiliza bônus com base na quantidade de pontos VIP. Esses pontos são acumulados de acordo com as definições de multiplicação estabelecidas na seção Configurações/Bônus VIP, onde cada ponto é equivalente a 1 real depositado.

#### Como funciona?
O **Sistema VIP** é uma mecânica de bônus promocional oferecida aos jogadores, permitindo definir um valor de bônus para cada quantidade de pontos acumulados.

#### Implementação
Para integrar facilmente, adicione o seguinte trecho de código no método de finalização de pagamento.
```php
 \App\Helpers\Core::payBonusVip($wallet, $price);
```

### HISTÓRICO DE AÇÃO
Foi criado um novo módulo que permite monitorar detalhadamente as ações no seu painel administrativo. Dessa forma, você terá um relatório completo das atividades da sua equipe.

Coloque o código abaixo onde deseja monitorar
```php
 \App\Helpers\Core::CreateReport($action, $description)
```

### DETALHES PARA AFILIADOS
Agora, quando o administrador visualiza um usuário, ele pode ver detalhes das indicações, como depósitos (confirmados ou pendentes) e suas quantidades, tanto do afiliado quanto dos indicados.

<hr>

### 1.5.2
* Detalhes de usuário foram melhorados, agora você pode ver a lista de depositos de indicações.
* Pasta do Filamentphp foi organizada, e também seus namespaces.

<hr>

## Baixar os jogos da Venix Games
Para baixar nossos jogos, é bem simples. Basta acessar o terminal da sua VPS ou hospedagem e, no diretório do projeto, digitar o comando php artisan venix:games. Você também pode configurar o CRON para isso, seguindo o exemplo abaixo.

Primeiro você precisa configurar a fila, defina no tempo que desejar:
```
/usr/bin/php8.3 /home/caminho/artisan queue:work 1>> /dev/null 2>&1
```

Depois para baixar os jogos, você pode definir uma vez por dia.

```
/usr/bin/php8.3 /home/caminho/artisan venix:games 1>> /dev/null 2>&1
```
[Precisa de recarga? Clique aqui](https://venix.games/)


#

## CUIDADO COM UM NOVO GOLPISTA
**Eu há um tempo após alguns haters, mudei o meu usuário do instagram, porem não sei como fizeram isso, pra mim não era
possivel, alguem trocou, pegou o mesmo usuário meu anterior. Já denunciei, e peço a vocês que façam o mesmo, por que esse
bandido está dando inumeros golpes utilizando meu nome e meu produto.**

ESSE PERFIL NÂO SOU EU. DENUNCIEM!!!

https://www.instagram.com/victormsalatiel

## Recursos:

- Autenticação com Google.
- Sistema de Afiliados com RevShare e CPA.
- Integração com Games Slotegrator.
- Integração com Games Salsa.
- Integração com Games Ever.
- Integração com Games Worldslote.
- Integração com Games Fivers, método Seamless
- Sistema de Notificação.
- Painel de Controle.
- Painel Administrativo.
- Painel de Afiliados.
- Sistema de customização
- Gateway de Pagamento DigitoPay. 
- Customização dos Banners e Slide.

Muitas pessoas buscam desenvolvedores para trabalhar em projetos e acabam sendo vítimas de golpes. 
Ao procurar um programador, solicite referências e um portfólio para garantir a segurança e a qualidade do serviço. Ou
Solicite um orçamento com nossos [Desenvolvedores Oficiais](https://viper.casino/)

## Melhorias e Correções

O Viper Pro está passando por diversas melhorias para prevenir ataques hackers e proteger os usuários contra ações maliciosas.
Caso você detecte algum bug ou falha de segurança, por favor, entre em contato através do site oficial. Resolveremos
o problema imediatamente e sem nenhum custo. Algumas falhas, listadas abaixo, já foram corrigidas.

### Problemas com rotas do admin, sendo acessadas pelo painel de afiliados.

Esse problema ocorria devido à ausência de uma validação separada, permitindo que algumas páginas do 
administrador fossem acessadas pelo painel de afiliado usando a mesma sessão e função. A seguir, explicamos as 
medidas que tomamos para resolver essa questão.

#### Novos middlewares foram criados para permitir bloqueios e validações individuais nos painéis.
- CheckAdmin 
- CheckAffiliate

#### Envio de Requisições no Provedor Ever, Worldslot e PlayGaming
Para evitar que dados de vitória sejam enviados via requisição e o saldo seja fraudado, implementamos um sistema 
de tokens para validar as transações recebidas.

#### Gateway de Pagamento - Digito Pay

1. Mudanças 
Anteriormente, enviávamos apenas o ID da transação para o front-end para consulta de status. Agora, enviamos tanto o ID da 
transação quanto o ID de verificação, o que permite realizar a chamada da transação com maior segurança.

2. Melhorias
Agora, na confirmação de depósito pelo webhook, realizamos uma verificação adicional para garantir que o pagamento foi realmente aprovado.

3. Webhook automaticado
Agora o webhook da digitopay é automaticamente configurado.


## [VIPER PRO 2.0](https://viper.casino/)
O projeto Viper Pro foi totalmente reformulado pela nova equipe Viper, da qual não faço mais parte. No entanto, posso garantir que vocês estão em boas mãos, com os melhores profissionais do iGaming.

SE VOCÊ NÃO É DESENVOLVEDOR E DESEJA UMA PLATAFORMA DE ALTA QUALIDADE, COM ATUALIZAÇÕES E MELHORIAS CONSTANTES, TANTO NO VISUAL QUANTO NO BACKEND, ADQUIRA SUA WHITE LABEL AGORA MESMO.

[COMPRAR AQUI](https://viper.casino/)

CLIENTES VIPER PRO V1 NÃO PAGAM PELA LICENÇA NA AQUISIÇÃO DA VIPER PRO 2.0. VALE A PENA MIGRAR, FICOU INCRIVEL
O NOVO PROJETO.

## Correções
Para qualquer dúvida ou relato de bugs, por favor, deixe-os aqui no GitHub. Farei o possível para resolver o mais rápido possível.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
