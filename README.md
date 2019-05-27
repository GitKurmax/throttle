# throttle

Реализовать декоратор throttle:

Так чтобы текущие координаты мышки в консоли при движении печатались раз в секунду
1 раз когда мышь только шевельнулась
дальше каждую секунду
После остановки дождаться очередную секунду и напечатать координаты в последний раз
Функция onMove должна получать тот же this и аргументы, что и обёртка
Codepen

function onMove(event) {
  console.log(event.clientX)
}

function throttle(f, delay) {
  // ...
}

let wrapper = throttle(onMove, 1000);

document.addEventListener('mousemove', wrapper);
