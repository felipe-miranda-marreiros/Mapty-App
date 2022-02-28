# Mapty-App

Mapty App faz parte do repositório <a href="https://github.com/felipe-miranda-marreiros/JavaScript">JavaScript</a>.

## Sobre 

O objetivo desse projeto é a utilização de <strong>Programação Orientada a Objetos</strong> em JavaScript. Nela, foi aplicado conceitos com base em <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes">ES6 Classes</a> - criação de classes, objetos, herança entre classes, polimorfismo, abstração, encapsulamento e proteção de propriedades e métodos.

Se você está procurando por Constructor Function, Prototype ou Object.create(), acesse o repositório <a href="https://github.com/felipe-miranda-marreiros/JavaScript/tree/main/POO">POO</a>.

### App

![image](https://user-images.githubusercontent.com/91689754/155927118-a280b90c-41c0-41c1-99ee-4af20f3e2c5d.png)

Mapty App é um site que tem como objetivo mostrar local do usuário de acordo com as informações do navegador. Você pode fazer isso com <a href="https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API">Geolocation API</a> e o método:

```js
_getPosition() {
    if (navigator.geolocation) {
      navigator.geolocation.getCurrentPosition(
        this._loadMap.bind(this),
        function () {
          alert("Could not get your position");
        }
      );
    }
  }
```
É necessário que o usuário permita compartilhar a informação. Caso contrário, terá como erro:

```js
alert("Could not get your position");
```

### Leaflet

![image](https://user-images.githubusercontent.com/91689754/155927959-98d58f34-c096-4e36-a414-11119089e474.png)

Para que o mapa seja renderizado, foi utilizado a biblioteca Leaflet. Ela disponibilza o mapa mundial, popups, zoom, auto-zoom, set-location. Então, a maior parte do trabalho fica para o Leaflet.

O mapa em si fica localizado em uma DIV vazia:

```html
<div id="map"></div>
```

### Descrição

![image](https://user-images.githubusercontent.com/91689754/155929747-2fa72bcb-d6c7-41df-abbe-9adaf0ff23c2.png)

Maptty App funciona como track no qual você pode guardar os treinos que fez durante o dia. Especificar o tipo de treinamento como running(corrida) ou bicycling (ciclismo); duração de cada etapa em minutos, distância e cadência (quantidade de passos por minuto).

### Como usar?

Basta permitir que o aplicativo utilize sua localidade, então o mapa carregará automaticamente. Clique em qualquer parte dele e um pop-up será aberto pedindo informações a respeito do tipo de treino realizado.

### Ferramentas Utilizadas

* HTML
* CSS
* JavaScript
* Leaflet

### Referencias

* https://www.udemy.com/course/the-complete-javascript-course/
* https://leafletjs.com/SlavaUkraini/ (site pode mudar de endereço por causa da situação da Ucrania - 28/02/2022)
