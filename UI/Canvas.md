Each scene has GameManager object, its managing the whole game, and contains the UI.
```
GameManager/Canvas
```
Is the canvas object.

Usaly in playing mode, player UI is located in `{canvas}/Game UI`.  
Thats what [WK-Stamina-Slider](https://github.com/overmet15/WKStaminaSlider) uses.

You can create any UI objects and etc in canvas, or even apply scripts to already existing ones.

For some reason, each scene has mostly same UI elements and names, for example, Win Screen exists in main menu, even tho its broken for some reason.

The UI mostly uses DOTween for animations, if you can capture the moment when it runs the animation, you can cancel it with `{object}.DOKill();`, and then apply your animation.
