1. Можно замедлять змейку без дублирования кода (правда, с созданием ещё одного поля): 
```
if ((length - oldLength) = 10) {
    let speed = speed - (speed / 4);
    let oldLength = length;
}
```
# (done)

2. Можно просто методы x() и y(). (Block.jack)
```
method int getCoord(boolean x) {
    var int retCoord;
    if (x) {
        let retCoord = xCoord;
    } 
    else {
        let retCoord = yCoord;
    }
    return retCoord;
  }
``` 

3. Можно просто do Screen.setColor(color); (Block.jack)
```
if (color) {
      do Screen.setColor(true);
    } else {
      do Screen.setColor(false);
    }
```
# (done)

4. Во многих классах можно писать "length" вместо одной буквы "l": (Snake.jack)
```
function boolean seeIfLose(int l, Snake snake, int dir)
```

5. Можно без лишней переменной restart. (main.jack)
```
while (view.move()) {
    do view.dispose();
    let view = View.init(5);
}
```
# (done)