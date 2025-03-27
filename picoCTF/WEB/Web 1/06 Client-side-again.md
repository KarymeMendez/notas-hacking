#### Description

Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/6353/` ([link](https://jupiter.challenges.picoctf.org/problem/6353/)) or http://jupiter.challenges.picoctf.org:6353



#### Hints



### Solución
1. Entramos al link
2. Ctrl U a la pagina
3. Visualizamos que hay una lineas de codigo, lo pasamos a JS NICE
```
 var _0x5a46=['0a029}','_again_5','this','Password\x20Verified','Incorrect\x20password','getElementById','value','substring','picoCTF{','not_this'];(function(_0x4bd822,_0x2bd6f7){var _0xb4bdb3=function(_0x1d68f6){while(--_0x1d68f6){_0x4bd822['push'](_0x4bd822['shift']());}};_0xb4bdb3(++_0x2bd6f7);}(_0x5a46,0x1b3));var _0x4b5b=function(_0x2d8f05,_0x4b81bb){_0x2d8f05=_0x2d8f05-0x0;var _0x4d74cb=_0x5a46[_0x2d8f05];return _0x4d74cb;};function verify(){checkpass=document[_0x4b5b('0x0')]('pass')[_0x4b5b('0x1')];split=0x4;if(checkpass[_0x4b5b('0x2')](0x0,split*0x2)==_0x4b5b('0x3')){if(checkpass[_0x4b5b('0x2')](0x7,0x9)=='{n'){if(checkpass[_0x4b5b('0x2')](split*0x2,split*0x2*0x2)==_0x4b5b('0x4')){if(checkpass[_0x4b5b('0x2')](0x3,0x6)=='oCT'){if(checkpass[_0x4b5b('0x2')](split*0x3*0x2,split*0x4*0x2)==_0x4b5b('0x5')){if(checkpass['substring'](0x6,0xb)=='F{not'){if(checkpass[_0x4b5b('0x2')](split*0x2*0x2,split*0x3*0x2)==_0x4b5b('0x6')){if(checkpass[_0x4b5b('0x2')](0xc,0x10)==_0x4b5b('0x7')){alert(_0x4b5b('0x8'));}}}}}}}}else{alert(_0x4b5b('0x9'));}}
```
4. Lo ordena y sale lo siguiente
```
/** @type {Array} */
var _0x5a46 = ["0a029}", "_again_5", "this", "Password Verified", "Incorrect password", "getElementById", "value", "substring", "picoCTF{", "not_this"];
(function(paths, opt_attributes) {
  /**
   * @param {number} val
   * @return {undefined}
   */
  var setter = function(val) {
    for (;--val;) {
      paths["push"](paths["shift"]());
    }
  };
  setter(++opt_attributes);
})(_0x5a46, 435);
/**
 * @param {string} key
 * @param {?} dataAndEvents
 * @return {?}
 */
var _0x4b5b = function(key, dataAndEvents) {
  /** @type {number} */
  key = key - 0;
  var label = _0x5a46[key];
  return label;
};
/**
 * @return {undefined}
 */
function verify() {
  checkpass = document[_0x4b5b("0x0")]("pass")[_0x4b5b("0x1")];
  /** @type {number} */
  split = 4;
  if (checkpass[_0x4b5b("0x2")](0, split * 2) == _0x4b5b("0x3")) {
    if (checkpass[_0x4b5b("0x2")](7, 9) == "{n") {
      if (checkpass[_0x4b5b("0x2")](split * 2, split * 2 * 2) == _0x4b5b("0x4")) {
        if (checkpass[_0x4b5b("0x2")](3, 6) == "oCT") {
          if (checkpass[_0x4b5b("0x2")](split * 3 * 2, split * 4 * 2) == _0x4b5b("0x5")) {
            if (checkpass["substring"](6, 11) == "F{not") {
              if (checkpass[_0x4b5b("0x2")](split * 2 * 2, split * 3 * 2) == _0x4b5b("0x6")) {
                if (checkpass[_0x4b5b("0x2")](12, 16) == _0x4b5b("0x7")) {
                  alert(_0x4b5b("0x8"));
                }
              }
            }
          }
        }
      }
    }
  } else {
    alert(_0x4b5b("0x9"));
  }
}
;
```
5. Copiamos lo siguiente y pegamos en la consola
```
var _0x5a46 = ["0a029}", "_again_5", "this", "Password Verified", "Incorrect password", "getElementById", "value", "substring", "picoCTF{", "not_this"];
```
6. Armamos la bandera analizando las posiciones
```
picoCTF{not_this_again_50a029}
```