## **Usage**

You can use pyfiglet in one of two ways. First, it operates on the commandline as C figlet does and supports most of the same options. Run with --help to see a full list of tweaks. Mostly you will only use -f to change the font. It defaults to standard.flf.                                                                                                                                                              `tools/pyfiglet 'text to render'`                                                 

### Pyfiglet is also a library that can be used in python code:

```py
from pyfiglet import Figlet
f = Figlet(font='slant')
print(f.renderText('text to render'))
```

or   

```py
import pyfiglet
f = pyfiglet.figlet_format("text to render", font="slant")
print(f)
```

If you have found some new fonts that you want to use, you can use the command line interface to install your font file as follows:                                                                                                                      
`pyfiglet -L <font file>`

The font file can be a ZIP file of lots of fonts or just a single font. Depending on how you installed pyfiglet, you may find that you need root access to install the font - e.g. sudo pyfiglet -L <font file>.   
