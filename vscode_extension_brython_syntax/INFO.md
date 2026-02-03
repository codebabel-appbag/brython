#  [![](https://i.postimg.cc/wBPhM5Lv/jackal-11-24-v2-32-inverted.png)]()  CODEBABEL

### *codebabel-brython-syntax : syntax highlight inside html 🐍*
___
## 📃 Description / Descrição
~~~
codebabel-brython-syntax > brython on html syntax highlight
inside html file by codeBabel for vscode. 
~~~
[![](https://i.postimg.cc/m2rsyX8k/shield-vscode-115x20.png)]()

[![](https://i.postimg.cc/Wp99RxZT/banner.png)]()

## 🌐 Content / Conteúdo
* [Installation](#installation)
* [Change log](#changelog)
* [brython code](#brython)
* [brython site](#site)
* [Screenshot](#screenshot)

### installation
## 💻 Installation / Instalação

## 🧭 Minimum Requirements/Requisitos Mínimos.
```
{PTBR}
Observação: será instalada a extensão Jinja (wholroyd.jinja)
para que funcione corretamente.

{FR}
Remarque : L'extension Jinja (wholroyd.jinja)
devra être installée pour que cela fonctionne correctement.

{SP}
Nota: Será necesario instalar la extensión Jinja (wholroyd.jinja)
para que funcione correctamente.

{ZH}
注意：需要安装 Jinja 扩展程序 (wholroyd.jinja) 才能正常工作。

{JA}
注意: 正しく機能するには、Jinja 拡張機能 (wholroyd.jinja) をインストールする必要があります。

{EN}
Note: The Jinja extension (wholroyd.jinja)
will need to be installed for it to function correctly.
```
## Manual Link: (wholroyd.jinja)

[![](https://i.postimg.cc/HsN6zgbG/Who-Iroyd-Jinja.png)]()
___
[🔗 https://marketplace.visualstudio.com/items?itemName=wholroyd.jinja](https://marketplace.visualstudio.com/items?itemName=wholroyd.jinja)
___

~~~~
{BR}
🐍 Na guia de extenções, procure por "cbbl" ou "codebabel-brython-syntax",
instale, crie um documento *.html usando brython.
🐍 Instalação fácil
🐍 A extensão "codebabel-brython-syntax" desenvolvida para facilitar a
codificação usando brython, ao criar o index.html, na tag script ao
inserir código python a extensão fará o restante.

{EN}
🐍 In the extensions tab, search for "cbbl" or "codebabel-brython-syntax",
install it, and create an *.html document using Brython.
🐍 Easy installation
🐍 The "codebabel-brython-syntax" extension is designed to make coding
easier using Brython. When creating the index.html file, insert Python
code into the script tag; the extension will handle the rest.
~~~~

### changelog
## 🚨 Change Log
|Version|       Version Name       | Upgrade Latency |
|-------|--------------------------|-----------------|
| 0.0.1 | codebabel-brython-syntax |    ON DEMAND    |
| 0.0.2 | codebabel-brython-syntax | wholroyd.jinja  |

### brython
## 🐍 Brython code
~~~html
<!DOCTYPE html><html lang="en"><!-- brython ajax demo -->
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
    <link rel="stylesheet" href="style.css">
    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/brython@3.13.2/brython.min.js">
    </script>
    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/brython@3.13.2/brython_stdlib.js">
    </script>
    <title>brython.ajax</title>
</head>
<body>
<script type="text/python">
    from browser import document, ajax

    url = "http://api.open-notify.org/iss-now.json"
    msg = "Position of the International Space Station at {}: {}"

    def complete(request):
        import datetime
        data = request.json
        position = data["iss_position"]
        ts = data["timestamp"]
        now = datetime.datetime.fromtimestamp(ts)
        document["zone10"].text = msg.format(now, position)

    def click(event):
        ajax.get(url, oncomplete=complete, mode="json")
        document["zone10"].text = "waiting..."

    document["button10"].bind("click", click)
</script>
</body></html>
~~~

### screenshot
## 📸 Screenshot
#### Example Code...

[![](https://i.postimg.cc/52vTV1L3/screenshot.png)]()

___
### site
## 🐍 brython site
🔗 [https://brython.info/index.html](https://brython.info/index.html)

___
## 💜 Thank's 🧡
~~~
{PTBR}
Valeu por usar a extensão codebabel-brython-syntax.
tmj!

{EN}
Thanks for using the codebabel-brython-syntax extension.
see ya!

extension by codesofty@codebabel.
~~~
© Copyright 2026, codebabel from brython users.
