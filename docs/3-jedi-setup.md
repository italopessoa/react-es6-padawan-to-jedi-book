# Configurando o React como mestre Jedi

Aprendemos até agora que o React é uma biblioteca de JavaScript, criada pelo Facebook, que é usada para construir interfaces de usuário. Quando eu comecei, uma das coisas que me incomodou foi que a maioria dos tutoriais sobre o React pulavam a configuração do ambiente. É tanto que vimos na seção anterior como fazer isso. Mas aquela configuração serve apenas a nível de aprendizado. No mundo real, não fazemos dessa forma. Nesta seção iremos criar um ambiente de desenvolvimento com React do zero. Vamos usar o seguinte:

1. Webpack - `Module bundler`
2. Babel - Compilador Javascript
3. ES6 - Nova especificação Javascript
4. Yarn - Um gerenciador de pacotes(usaremos ele no lugar do npm)
5. React

## Pré-Requisitos
Antes de mais nada, vamos precisar do Node e do Yarn instalados antes de configurar o nosso ambiente.

Como mencionado acima, usaremos o `yarn` como Gerenciador de Pacotes. É bastante semelhante ao `npm` e tem quase os mesmos comandos fornecidos pelo `npm`. Ele também vem com alguns recursos extras que `npm` não fornece. Algumas razões são:

1. Se você já instalou um pacote antes, você pode instalá-lo novamente sem qualquer conexão com a Internet.
2. Além do fato de que você pode instalar pacotes offline, isso também aumenta a velocidade de suas atualizações.
3. As mesmas dependências são instaladas em qualquer máquina. Isto significa essencialmente que uma instalação em uma máquina funcionará da mesma maneira em qualquer outra máquina.

Para obter mais informações, você pode consultar a documentação do `yarn`.

Para usuários de Mac OS, os comandos abaixo serão suficientes para instalar o `yarn`. Para outros sistemas operacionais, por favor visite a página de instalação do  [yarn](https://yarnpkg.com/en/docs/install#mac-tab) para ver as instruções de instalação.

```javascript
brew update
brew install yarn
```

## Observações
1. Nessa seção iremos configurar um ambiente para o projeto React e precisaremos criar um projeto bem simples para testar nossa configuração. Se não entender o código React que vamos fazer, não se preocupe. Não é o papel dessa seção focar no React em si, mas sim na criação de uma configuração que pode ser usada para iniciar um projeto no mundo real.
