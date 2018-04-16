# Medio homogeneo

Ejecucion:
```
cp system/setFieldsDict.const system/setFieldsDict
setFields
porousFieldSimpleFoam
```
## Solucion analitica

![equation1](http://www.sciweavers.org/tex2img.php?eq=%5CDelta+P+%3D+%28+%5Cmu+%2A+D+%2B+%5Cfrac%7B1%7D%7B2%7D+%5Crho+%2A+U+%2A+F%29+%2A+%5CDelta+L+%2A+U&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![equation2](http://www.sciweavers.org/tex2img.php?eq=%28+0.000003774+%2A+1643133150+%2B%5Cfrac%7B1%7D%7B2%7D.2+%2A+894.3699319+%29+%2A+5x10%5E%7B-5%7D%2A.2+%3D+0%2C062906215&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)

## Resultados

Metodo                  | Caida de presión
---                     | ---
Analitico               | 0,062906215
porousFieldSimpleFoam   | 0.0628532
porousSimpleFoam        | 0.0628532

# Gradiente

Ejecucion:
```
funkySetFields -latestTime
porousFieldSimpleFoam
```

## Solucion analitica
![equation3](http://www.sciweavers.org/tex2img.php?eq=%5CDelta+P+%3D+%28+%5Cmu+%2A+D+%2B+%5Cfrac%7B1%7D%7B2%7D+%5Crho+%2A+U+%2A+F%29+%2A+%5CDelta+L%5E2+%2A+U&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![equation4](http://www.sciweavers.org/tex2img.php?eq=%280.000003774%2A1643133150%2B%5Cfrac%7B1%7D%7B2%7D.2%2A894.3699319%29%2A5x10%5E%7B-5%7D%2A.2+%3D+0%2C000003143&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

## Resultados

Metodo                  | Caida de presión
---                     | ---
Analitico               | 0,000003143
porousFieldSimpleFoam   | 0.00000314264